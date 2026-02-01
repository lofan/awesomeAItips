近期在 GitHub 上爆紅的開源 AI Assistant『龍蝦機器人』 助手項目 Moltbot (原名 Clawdbot)。這款工具因其強大的主動性與自動化能力，甚至引發了有人購買 12 部 Mac Mini 來運行它的熱潮。
雖然功能便利，但有幾點安全性建議：強烈建議不要安裝在主力電腦上。 由於該軟體會要求完整的系統最高權限，加上開發背景的考量，建議使用空白新機、閒置電腦或雲端 VPS 進行測試。這款工具對新手來說門檻與風險較高，追求便利的同時，請務必衡量資安風險。」

更接近AGI?
* :pushpin:[燒錢 + 私隱危機！Moltbot (Clawdbot) 實測：點解有人買 12 部 Mac Mini 玩佢？](https://www.youtube.com/watch?v=u0i65fNsl3U)
* :pushpin:[恐佈級驚人AI代理 OpenClaw (前MoltBot/ClawdBot) 實測！超詳細攻略：低成本用頂級模型祕技大公開！｜廣東話｜文恩澄](https://www.youtube.com/watch?v=YZaQGIl-bgE)
* There are over 50+ AI agents, from around the world, autonomously talking to each other about whatever they want right now on [Moltbook](https://www.moltbook.com/)
* [「中翻」如何在 Mac mini 上安裝萬能私人AI 助理 Clawdbot（moltbot）詳細教學](https://www.youtube.com/watch?v=fs6HeBIl8fc)
* [Clawdbot renamed Moltbot](https://clawd.bot/)
* [5分钟上手Clawdbot！风靡硅谷的开源AI神器，到底怎么玩？](https://www.youtube.com/watch?v=u0i65fNsl3U)
* [Shodan results](https://www.shodan.io/search?query=moltbot)

**定位：它是一款強大的 AI 代理（AI Agent），而不僅僅是聊天回答問題，還能主動在你的電腦上執行任務**

什麼是 OpenClaw？
具備行動力的 AI：不同於一般的 AI 助手（如 ChatGPT），OpenClaw 具有「手」的功能，可以操作電腦、執行腳本、管理檔案，甚至是控制軟體（如 Photoshop）

0. 三大核心組件：
大語言模型 (LLM)：作為 AI 的大腦（如 Claude、GPT-4 等）。
通信接口 (Gateway)：讓使用者透過 Telegram、WhatsApp、Discord 或 iMessage 與 AI 溝通。
技能與插件 (Skills/Plugins)：擴展 AI 的能力，例如網頁瀏覽、語音識別、控制特定軟體等。

1. 三大核心特色：
深度集成：能直接在你的電腦上運行，並與 Telegram、WhatsApp、Gmail、Google Drive 等工具連動 。
持久記憶 (Persistent Memory)：它能記住你的習慣與偏好，並在背景處理工作時參考這些記憶。
主動性 (Proactive)：它會主動發訊息給你，例如提醒你有緊急郵件或匯報工作進度，而不僅僅是被動等待指令。

3. 實際應用案例
處理郵件：有人利用它發送 500 封開發信，成功獲得 43 個回覆，大幅節省成本。
程式開發：可自動修復 Bug、執行測試並將代碼 Push 到 GitHub。
自動通訊：甚至有人結合 ElevenLabs 讓它自動打電話或傳送語音訊息給商務夥伴。

4. 為什麼大家要用 Mac Mini 運行？
隱私與安全：為了將 AI 助手與日常使用的電腦隔離，許多人選擇在獨立的設備（如 Mac Mini）上運行，以防止 AI 存取到主機的敏感文件或密鑰 。
多平台支援：雖然 Mac Mini 爆紅，但它其實也支援 Windows、Linux、Raspberry Pie 或 VPS 雲端主機 。

5. 潛在風險與缺點
燒錢風險：由於它是主動運行的，若設定不當（如陷入無限循環），可能會導致 API 費用暴增。有網友曾一天花掉 70 美金 。
安全與隱私危機：
漏洞風險：項目仍處於早期階段，曾爆出 API Key 洩漏的風險。
惡意插件：社群提供的 Skills (插件) 可能包含病毒或惡意代碼，安裝時需非常小心 。
權限過大：一旦授權它存取 Gmail 或 Twitter，它便能以你的身份行事 。

6. 使用建議與防範
環境隔離：建議在獨立的環境（如 Docker 或 專用電腦）運行 。
審查代碼：對於社群開發的 Skill，建議進行 Code Review。
設置審核：在執行任何動作前，設定需要人工審核 (Manual Review) 以確保安全。
