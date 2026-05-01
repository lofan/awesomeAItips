# Use Claude to learn anything 100x faster.

## The only 7 prompts you need:
1. The Anchor Explainer "Explain [topic] as if I'm intelligent but have zero background in it. Use one unexpected real-world analogy that makes the core idea immediately click. Then give me the 3 things I need to understand before I go any deeper."
2. The Socratic Drill "Quiz me on [topic] with 10 progressive questions — start simple, build to expert-level. After every answer I give: tell me what I got right, what I missed, the underlying principle, and one follow-up question to go deeper."
3. The Mental Model Builder "What are the 3–5 foundational principles of [topic] that, once truly understood, make everything else click? For each one: explain it in plain language, show how it plays out in a real example, and tell me the #1 mistake people make when they don't understand it."
4. The Myth Buster "What are the 5 most common misconceptions people have about [topic]? For each: state the myth, explain exactly why it's wrong, share what the evidence or expert consensus actually says, and tell me why smart people still believe it."
5. The Distillation Engine "Distil [book / concept / field] into the 10 ideas that will actually change how I think or act. For each: the core idea in one sentence → why it matters in the real world → one specific thing I can do today to apply it."
6. The Expert Challenger "Act as a world-class [expert]. I'll share my current understanding of [topic]. Your job: challenge my assumptions, expose my blind spots, and teach me how an expert actually thinks about this — not just the facts, but the judgment."
7. The Pressure Test "I've just studied [topic]. Give me a realistic, high-stakes scenario where I must apply this knowledge to solve a problem. After I respond, break down my reasoning: what I applied correctly, what I missed, and what an expert would have done differently."

## Example
1. 錨點解釋法 “解釋[主題]，就好像我很聰明，但背景知識為零一樣。使用一個意想不到的現實世界類比，使核心思想立即產生共鳴。然後在我進一步深入之前，給我需要理解的三件事。”
'''
解釋[Quantum]，就好像我很聰明，但背景知識為零一樣。使用一個意想不到的現實世界類比，使核心思想立即產生共鳴。然後在我進一步深入之前，給我需要理解的三件事。
'''
3. 蘇格拉底式練習 “用 10 個漸進的問題對我進行 [主題] 測試 - 從簡單開始，逐步提高到專家水平。在我給出的每一個答案之後：告訴我我做對了什麼，我錯過了什麼，基本原則，以及一個進一步深入的後續問題。”
'''   
用 10 個漸進的問題對我進行 [主題] 測試 - 從簡單開始，逐步提高到專家水平。在我給出的每一個答案之後：告訴我我做對了什麼，我錯過了什麼，基本原則，以及一個進一步深入的後續問題。
'''   
4. 心智模型建構者 “[主題]的 3-5 個基本原則是什麼，一旦真正理解，其他一切都會變得容易理解？對於每一個原則：用通俗易懂的語言解釋它，展示它在真實示例中的表現，並告訴我人們在不理解它時會犯的第一個錯誤。”
5. 流言終結者 “人們對[主題]最常見的 5 種誤解是什麼？對於每一個誤解：陳述流言，準確解釋其錯誤原因，分享證據或專家共識的實際內容，並告訴我為什麼聰明人仍然相信它。”
6. 蒸餾引擎 “將[書籍/概念/領域]提煉成10個想法，這些想法將真正改變我的思維或行為方式。對於每個想法：一句話中的核心想法→為什麼它在現實世界中很重要→我今天可以做的一件具體事情來應用它。”
7. 專家挑戰者 “扮演世界級的[專家]。我將分享我目前對[主題]的理解。你的工作：挑戰我的假設，暴露我的盲點，並教我專家如何真正思考這個問題——不僅僅是事實，還有判斷。”
8. 壓力測試 “我剛剛學習了[主題]。給我一個現實的、高風險的場景，我必須運用這些知識來解決問題。在我回答之後，分解我的推理：我正確應用了什麼，我錯過了什麼，以及專家會採取什麼不同的做法。”


呢套 Prompt（提示詞）組合簡直係一套 **「深度學習工具箱」**。佢哋唔係叫 AI 隨便俾啲資料你，而係透過唔同嘅思維框架（Frameworks）嚟榨取 AI 嘅知識，幫你由淺入深咁拆解一個主題。

以下係我用廣東話幫你分析呢 7 個 Prompt 點解咁勁，同埋佢哋適合咩場景：

---

### 1. The Anchor Explainer（錨點解釋法）
*   **核心價值：** 避開「低智化」解釋，尊重你嘅理解能力，但同時掃除專業術語嘅障礙。
*   **點解有用：** 嗰個「意想不到嘅比喻」係關鍵。人腦係靠關聯嚟學習嘅，一個好嘅比喻可以幫你喺腦入面起個「錨」，等啲抽象概念有位擺。
*   **適合：** 啱啱接觸新領域（例如：量子計算、區塊鏈），想快速建立初步認知嘅時候。

### 2. The Socratic Drill（蘇格拉底式訓練）
*   **核心價值：** **主動學習（Active Learning）**。
*   **點解有用：** 淨係睇資料好容易有「理解嘅幻覺」。透過 10 個由淺入深嘅問題，AI 會逼你思考。最正係佢會話你知「漏咗乜」同「背後原理」，呢種即時反饋（Feedback Loop）係最快嘅進步方式。
*   **適合：** 準備考試、面試，或者想測試自己係咪真係識。

### 3. The Mental Model Builder（思維模型構建器）
*   **核心價值：** 搵出「第一性原理」（First Principles）。
*   **點解有用：** 任何複雜嘅學問其實都係由幾個核心原則組成。掌握咗呢 3-5 點，你就唔使死記硬背。特別係佢指出埋「最常犯嘅錯」，幫你避開新手最易踩嘅坑。
*   **適合：** 想長期鑽研某個領域，建立扎實根基嘅時候。

### 4. The Myth Buster（迷思破解器）
*   **核心價值：** 糾正錯誤認知，建立批判性思維。
*   **點解有用：** 有時「學錯嘢」比「唔識嘢」更危險。呢個 Prompt 唔單止話你知邊啲係錯，仲會解釋「點解叻人都會信」，呢點好重要，因為佢幫你理解人性弱點同認知偏誤。
*   **適合：** 啲好多資訊污染、充滿爭議嘅話題（例如：理財、健康食譜、心理學）。

### 5. The Distillation Engine（精華提煉引擎）
*   **核心價值：** **執行力導向**。
*   **點解有用：** 好多書或者理論都係「聽完好似好勁，但唔知點做」。呢個 Prompt 將知識轉化為行動（Actionable insights），特別係「今日可以點做」嗰部分，將知識直接落地。
*   **適合：** 睇完一本好厚嘅書，或者想將一個大理論轉化為生活習慣時。

### 6. The Expert Challenger（專家挑戰者）
*   **核心價值：** 消除「達克效應」（Dunning-Kruger effect），即係「唔知自己唔知」。
*   **點解有用：** 佢唔係教你事實（Facts），係教你**判斷力（Judgment）**。專家同新手嘅分別，通常係睇問題嘅維度唔同。呢個 Prompt 係要 AI 嚟「啄」你嘅盲點。
*   **適合：** 當你覺得自己已經掌握咗，想更上一層樓，或者要處理複雜決策時。

### 7. The Pressure Test（壓力測試）
*   **核心價值：** 實戰模擬。
*   **點解有用：** 紙上談兵冇用，放你入一個「高風險情景」先見真章。透過呢種 Case Study 方式，你可以檢視自己喺壓力下會唔會漏咗考慮重要因素。
*   **適合：** 學完一套新嘅管理方法、談判技巧或者技術流程之後嘅總結。

---

### 💡 總結建議
如果你要學一個全新嘅嘢，我建議嘅**「組合拳」**順序係：
1.  先用 **1 (Anchor)** 建立概念。
2.  用 **3 (Mental Model)** 捉住核心。
3.  用 **4 (Myth Buster)** 排除誤解。
4.  最後用 **2 (Socratic Drill)** 或者 **7 (Pressure Test)** 嚟驗收成果。

呢套嘢如果你用得熟，AI 就會由「聊天機械人」變成你專屬嘅「頂級私人補習老師」。

STOP paying for ChatGPT, use DeepSeek
STOP paying for Midjourney, use Nano Banana
STOP paying for Grammarly, use LanguageTool
STOP paying for ElevenLabs, use VoiceBox
STOP paying for Runway, use Syllaby
STOP paying for Grok Imagine, use Qwen
STOP paying for Suno, use Lyria 3
STOP paying for Rundown AI, use Synapze AI
STOP paying for Canva, use Pomelli
STOP paying for Descript, use CapCut
STOP paying for API, use OpenRouter
STOP paying for Notion AI, use NotebookLM
STOP paying for Lovable, use Claude Code
