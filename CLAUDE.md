# Kuroshio Athletics 官網（kuroshio-site）

這是平誠旗下 Kuroshio Athletics（黑潮運動）的對外網站。靜態站，零建置，GitHub Pages 從 main 根目錄發布。服務設計、研究、決策都在 second brain（~/Anson），這裡只管網站本身。

## 品牌硬規則
- 色票只有這五個：Abyss #07253E、Deep #0E3A5C、Tide #186E80、Foam #8FC0C9、Brass #C08A3E；中性色 Paper #FFFDF8、Sand #F6F2E9、Hair #D7D2C6、Muted #5A6D7B。狀態色只用在報告不用在行銷頁。不新增第六個顏色。
- Brass 只當強調與主要行動按鈕，不進 logo。Foam 不能在淺底上當文字。Deep 只當 Abyss 底上的分層。
- 字型：Fraunces（英文標題）、Noto Sans TC（正文）、IBM Plex Mono（標籤數字）。只從 Google Fonts 載。
- Logo 在 assets/，不改色、不拉伸、不旋轉。深底用 lockup-on-dark。

## 文案紅線
- 不寫「保證」「100%」「最少 X 個 offer」「full ride」當預設、「教練網絡 X 萬人」。
- 沒有依據的數字寫【待確認】，不編。
- 語氣：專業、誠實、短句。定位句是「代辦只幫你送件。我們讓他在送件之前就準備好。」
- 不用 emoji，不用破折號。

## 做法
- 單一 HTML 加原生 CSS，不引框架，不加 build step。
- 改文案直接改 index.html，它是唯一來源。
- 每完成一件看得到的事就 commit 並 push，main 就是正式站。
- 價格與方案內容的真相在 ~/Anson/projects/kuroshio/service-design/workshop-notes.md，改價先改那裡再改這裡。

# 來自 Anson（second brain，~/Anson）的 context，開場自動載入
@~/Anson/projects/kuroshio/README.md
@~/Anson/.claude/rules/brand-voice.md
@~/Anson/.claude/rules/communication-style.md
Anson 的 README 有進度、Paul 丟過的想法、給程式端的待辦。做完功能改 docs 或 README，Anson 那邊說「同步程式碼文件」就會收到。

## 做完功能的收尾
每次功能做完或行為改變，更新 README.md 或 docs/ 對應段落再 commit。post-commit hook 只抄文件不抄程式碼，README 沒更新 Anson 就不知道你做了什麼。

## 跟 Paul 工作的方式
Paul 是 founder，不是這個 repo 的全職工程師。目標是讓他清楚知道現在在做什麼，並且能自己往下推。
- 收到指令先盤點再動手，格式照上面 import 的 communication-style「先盤點再動手」。
- 用白話講。技術名詞第一次出現就用一句話解釋（例如「migration，就是改資料庫欄位的腳本」）。不要用縮寫堆疊。
- 不要貼大段程式碼給他看，除非他要。講「改了哪個檔、行為變成怎樣」。
- 做完給三段：改了什麼、怎麼驗證（他可以自己點的步驟或指令）、下一步。
- 對外會影響使用者的改動（上線、寄信、改資料）先問。
- 繁體中文，專有名詞英文，不用 emoji，不用破折號。
