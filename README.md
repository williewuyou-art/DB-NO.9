# 大本9號船舶作業平台

## 上架方式
1. 在 GitHub 建立一個 repository（建議設為 Public，GitHub Pages 通常需要公開 repository，依帳戶方案而定）。
2. 將本資料夾內的所有檔案與 `reports/` 資料夾一起上傳到 repository 根目錄。
3. 確認 `index.html` 位於根目錄。
4. 進入 repository 的 **Settings → Pages**。
5. 在 Build and deployment 選擇 **Deploy from a branch**，分支選 `main`，資料夾選 `/(root)`，按 Save。
6. 等待部署完成，從 Pages 顯示的網址開啟網站並測試各頁面與 PDF 下載。

## 檔案結構
- `index.html`：網站首頁與導覽
- `trim.html`：船舶配載／配平簡化試算（不含新增的自由液面 FSM 功能；保留左右舷座標修正）
- `cat3408-inspection.html`：CAT 3408 檢修示意頁
- `reports.html`：PDF 報告下載中心
- `reports/`：可下載報告 PDF

## 新增報告
將 PDF 放入 `reports/`，再在 `reports.html` 的 `reportFiles` 陣列新增一筆資料，`file` 路徑需與實際檔名完全一致。
