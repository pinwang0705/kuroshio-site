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
Anson 的 README 有進度、Paul 丟過的想法、給程式端的待辦。做完功能改 docs 或 README，Anson 那邊說「同步程式碼文件」就會收到。
