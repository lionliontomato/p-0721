# Potato × PTM 整合版

## 內容
- `index.html`：單一入口，可在 Potato 與 PTM 兩個原網站間切換。
- `.nojekyll`：GitHub Pages 靜態檔案設定。

## 上傳 GitHub Pages
1. 將本資料夾內的 `index.html` 與 `.nojekyll` 上傳到新 Repository 根目錄。
2. Repository 設定為 Public。
3. 開啟 Settings → Pages。
4. Source 選擇 Deploy from a branch。
5. Branch 選 `main`，資料夾選 `/(root)`，按 Save。

## 保留原網站的方式
本整合版使用 iframe 直接載入：
- https://lionliontomato.github.io/potato/
- https://lionliontomato.github.io/PTM/

因此不會複製或重寫兩個原網站的 HTML/CSS/JavaScript；原網站的字體、版面、圖片、動畫、功能及各自的試算表更新方式由原網站維持。兩個原網站必須持續公開且可正常使用。

## 網頁圖示
切換時會依序嘗試該網站常見的 Favicon 路徑（favicon.ico、favicon.svg、favicon.png、assets/favicon.*、images/favicon.png、apple-touch-icon.png）。若原網站使用自訂檔名或非標準路徑，請將該圖示路徑補進 `index.html` 對應網站的 `faviconCandidates` 清單。

## 注意
- 此 ZIP 不會修改原本兩個網站或 Google 試算表。
- 若原網站禁止被 iframe 嵌入，請使用頁面上的「另開原網站」連結，或改採取得原始專案檔後將內容放入獨立子資料夾的方式。
- 此環境無法直接連線到 GitHub Pages 檢視線上頁面，因此已檢查本機 HTML/JavaScript 結構與 ZIP 完整性，但尚未完成實際線上視覺與 Favicon 路徑驗證。
