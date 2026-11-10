# AI 助教與課堂實作｜1112 市北工作坊

國立臺中教育大學 教育學系 阮孝齊 助理教授 工作坊分享網站（純靜態 HTML，可直接放上 GitHub Pages）。

## 網站結構

```
index.html               首頁入口（六個單元、三份學習單、工具與資源連結）
units/unit-01.html ~ 06  六個單元頁：投影片內容改成網頁，提示詞可一鍵複製，每頁可開啟原投影片
worksheets/index.html    學習單分享頁（使用流程、QR code、下載）
worksheets/individual.html  個人學習單（可線上填寫、列印／存 PDF）
worksheets/group.html       小組學習單
worksheets/challenge.html   組間互評・挑戰單
worksheets/files/        三份學習單的 Word 原檔
img/                     從簡報抽出的圖片
slides/                  每張投影片的整頁圖（「原投影片」按鈕使用）
assets/                  樣式與程式（style.css、site.js、worksheet.js、qrcode.js）
```

## 部署到 GitHub Pages

1. 在 GitHub 建立新的 repository（例如 `ai-assistant-workshop`），設為 Public。
2. 把這個資料夾內的所有檔案（含 `.nojekyll`）上傳到 repository 根目錄：網頁上按 **Add file → Upload files**，把檔案拖進去後 Commit。
3. 到 **Settings → Pages**，Source 選 **Deploy from a branch**，Branch 選 `main`、資料夾選 `/ (root)`，按 Save。
4. 約 1–2 分鐘後，網址會是 `https://<你的帳號>.github.io/<repository 名稱>/`。

學習單分享頁的 QR code 會自動依照部署後的網址產生。

## 修改內容

- 文字直接編輯對應的 `.html` 檔即可。
- 學習單的填寫內容只存在使用者自己的瀏覽器（localStorage），不會上傳。
- 學生作答的學號已改為「學生 A–D」。

部分內容整理自劉育隆，AITE「AI 助教」簡報（國立臺中教育大學智慧教育中心）。
