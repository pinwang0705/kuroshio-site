# kuroshio-site

Kuroshio Athletics（黑潮運動）官網。靜態站，單一 HTML，零建置，GitHub Pages 從 main 根目錄發布。

正式站：https://pinwang0705.github.io/kuroshio-site/

- `index.html`：整站，唯一來源。受眾是家長與選手。價格依 2026-09-06 定版（決定 4.5）。
- `assets/`：logo PNG 五張加 `og-1200x630.png`（LINE / FB 分享預覽圖，Abyss 底加 lockup）。
- `CLAUDE.md`：品牌硬規則與文案紅線，改站前先讀。

## 改對外資料
`index.html` 最底下的 `<script>` 有兩個常數：

```js
var CONTACT_EMAIL = "";
var TAX_ID = "";
```

填了才會顯示（結尾 CTA 與 footer），空字串整段隱藏，不會出現「待補」。

## 尚未定案
- Vanderbilt 校名是否對外用（paul-interview 第 26 題補充）。目前站上寫「NCAA D1 大學」。
- 網域（kuroshio.pinchengco.com 或獨立）。
- 問卷 v2 上線後換 Tally 連結（現在是 v1：tally.so/r/Mepoqk）。

## 本機預覽
`python3 -m http.server 8765` 然後開 http://localhost:8765/

<!-- hook test 1788719781 -->
