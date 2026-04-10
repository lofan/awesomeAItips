# Claude Code
* [Claude Code Doc (Offical)](https://code.claude.com/docs/en/overview)
* [Claude Code: A Highly Agentic Coding Assistant (Deeplearning.ai)](https://learn.deeplearning.ai/courses/claude-code-a-highly-agentic-coding-assistant/lesson/66b35/introduction)
* This might be the wildest AI engineering breakdown on the internet right now 🤯
After the Anthropic leak…

Someone turned the ENTIRE Claude Code system into a readable playbook.
👉 [Claude code](https://claude-code-from-source.com) [github](https://github.com/alejandrobalderas/claude-code-from-source)

呢個網址 `claude-code-from-source.com` 其實係一個深入分析 Anthropic 推出嘅 AI 程式開發工具 **Claude Code** 底層架構同源代碼嘅技術專案。

呢個分析係基於 Claude Code 喺 npm 發佈時意外流出嘅 TypeScript 源代碼（透過 Source Maps 还原）。成份嘢分為 **7 個部分，共 18 個章節**，詳細拆解咗一個「工業級 AI Agent」係點樣運作嘅。

以下係廣東話版本嘅 Chapter by Chapter 內容總結：

---

### 第一部分：核心架構 (Core Architecture)
* **Chapter 1: AI Agent 嘅建築架構** 拆解咗 Claude Code 嘅 6 個核心抽象層，講述數據點樣喺系統入面流動，同埋佢點樣處理權限（Permission）同構建系統（Build system）。
* **Chapter 2: Bootstrap 啟動流程** 分析啟動時嘅 5 個階段。重點在於佢點樣做「模組級 I/O 並行處理」，務求喺極短時間內加載完畢，並劃分清楚「信任邊界」。
* **Chapter 3: 雙層狀態架構 (Two-Tier Architecture)** 講述 Claude Code 點樣管理「對話記憶」同「系統狀態」，確保 AI 喺做緊複雜任務時唔會「斷片」。

### 第二部分：執行模型 (Execution Model)
* **Chapter 4: 以 AsyncGenerator 為核心嘅 Agent Loop** 技術深挖：佢點樣用非同步產生器來處理訊息流，支持 Terminal 嘅即時回傳，仲有自然嘅「背壓（Backpressure）」同埋任務取消機制。
* **Chapter 5: 投機性工具執行 (Speculative Tool Execution)** 呢個係黑科技！AI 喺仲流式輸出（Streaming）緊、未講完嘢之前，就已經預判並開始執行「唯讀類」工具（例如讀取檔案），大大提升反應速度。
* **Chapter 6: 並發安全嘅批次處理 (Batching)** 將工具分為「安全（讀）」同「不安全（寫）」，讀取類會並行跑，寫入類就排隊跑，防止改壞代碼。

### 第三部分：環境與整合 (Environment & Integration)
* **Chapter 7: 終端機模擬 (Terminal Emulation)** 講 Claude 點樣喺你部機模擬一個 Shell，甚至可以處理顏色、進度條等複雜嘅 CLI 輸出。
* **Chapter 8: MCP (Model Context Protocol) 整合** 分析 Claude 點樣透過 MCP 協議去連埋其他工具（好似 Jira, Slack, Google Drive）。
* **Chapter 9: 文件系統監視器 (File Watchers)** 講系統點樣實時監控你嘅代碼變動，令 AI 隨時知你改咗啲乜。

### 第四部分：智能管理 (Intelligence Management)
* **Chapter 10: 提示詞工程與 System Prompts** 公開咗 Claude Code 內部嗰幾千行神秘嘅「系統指令」，揭示 Anthropic 係點樣教 AI 唔好「亂嚟」同埋點樣解決 Bug。
* **Chapter 11: 錯誤修復機制 (Self-Healing)** 當工具執行失敗（例如 Run Test 唔過），AI 點樣自動分析 Error 報告，然後自己出 Patch 修復。
* **Chapter 12: 上下文壓縮 (Context Compaction)** 當對話太長（爆 Token）時，系統點樣自動摘要舊內容，保留最重要嘅資訊。

### 第五部分：安全性與權限 (Security & Safety)
* **Chapter 13: 護欄系統 (The Guardrails)** 拆解防禦性代碼，防止 AI 執行危險命令（例如 `rm -rf /`）。
* **Chapter 14: 人機協作權限 (Human-in-the-Loop)** 分析邊啲操作需要你撳 "y" 確認，邊啲可以自動跑。

### 第六部分：進階功能 (Advanced Features)
* **Chapter 15: 多 Agent 協作 (Coordinator & Sub-agents)** 講 Claude 點樣分身，派一個「細仔（Sub-agent）」去處理特定小任務，大腦（Coordinator）就負責監督。
* **Chapter 16: Git 深度整合** 分析佢點樣自動寫 Commit Message、分 Branch 同埋解決 Merge Conflict。

### 第七部分：性能優化與未來 (Optimization & Beyond)
* **Chapter 17: 二階段加載 (Two-phase Skill Loading)** 啟動時只加載技能個名（Frontmatter），真正用到先加載具體內容，慳 Memory。
* **Chapter 18: 緩存穩定性 (Sticky Latches)** 確保喺一次 Session 入面，AI 嘅行為特徵同埋 Beta 功能開關唔會中途變咗。

---

### **一句話總結：**
呢份嘢係話畀你知，一個頂級嘅 AI 編程助手**唔單止係一個 LLM**，佢背後有一套極其複雜嘅**工程設計**去處理檔案、終端機、權限同埋速度優化。如果你係想自己寫一個 AI Agent，呢度係「教科書級別」嘅參考資料。⁠

We’re talking:
* 500K+ lines of real production AI agent logic
* Broken down into 18 chapters you can actually learn from
* Multi-agent systems, tool pipelines, memory, orchestration… all exposed

This isn’t theory
This is how a top-tier AI coding agent actually works under the hood

Key ideas you’ll steal instantly:
→ Agent loops with async execution
→ Multi-agent “teams” coordinating tasks
→ File-based memory (no DB 🤯)
→ Context compression tricks
→ Tool execution pipelines at scale

Basically…
Instead of guessing how to build AI agents
you now have a blueprint from a real system used by thousands of devs 
http://claude-code-from-source.com

Crazy part?
The whole thing was analyzed + rewritten in HOURS using AI agents 
http://claude-code-from-source.com

If you're building: 
• AI agents
* Dev tools
* LLM products
* or learning MLOps

This is not optional
This is a cheat code
