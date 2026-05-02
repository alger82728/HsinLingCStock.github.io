# GitHub Pages 部署方式

這個資料夾內容已經是 build 後的 GitHub Pages / iPhone PWA 版本。

## 上傳方式
1. 到 GitHub 建立一個新的 repository，例如 `stock-pwa`。
2. 將本資料夾內所有檔案上傳到 repository 根目錄。
3. 進入 Settings → Pages。
4. Source 選 `Deploy from a branch`。
5. Branch 選 `main`，Folder 選 `/ (root)`。
6. 等待 GitHub 產生網址。

## iPhone 安裝方式
1. 用 iPhone Safari 開啟 GitHub Pages 網址。
2. 點分享按鈕。
3. 選「加入主畫面」。
4. 從主畫面啟動即可像 App 使用。

## 更新 App
重新 build 後，把新的檔案上傳覆蓋即可。若 iPhone 沒立即更新，可修改 `service-worker.js` 的 `CACHE_NAME` 版本號。

## Gemini API 提醒
此靜態版本未內建 API Key。若要啟用 AI 分析，建議改用後端 API/Serverless Function，不建議把金鑰直接放在前端。
