# 土木建築工程提示語生成器（PWA）

台灣土木建築工程現場使用的 AI 提示語生成工具，可安裝至手機主畫面離線使用。

## 檔案說明（全部位於根目錄）

| 檔案 | 用途 |
|---|---|
| `index.html` | 主程式（HTML/CSS/JS 單檔） |
| `manifest.json` | PWA 安裝設定（名稱、主題色、圖標） |
| `sw.js` | Service Worker，提供離線快取 |
| `favicon.ico` | 瀏覽器分頁圖標（16/32/48/64） |
| `favicon-32x32.png` | 瀏覽器分頁圖標（PNG） |
| `apple-touch-icon.png` | iOS 主畫面圖標（180×180，深色底） |
| `icon-192.png`、`icon-512.png` | Android／桌面安裝圖標（透明背景圓形） |
| `icon-maskable-192.png`、`icon-maskable-512.png` | Android 自適應圖標（深色底、安全區留白） |

## 部署至 GitHub Pages

1. 建立新的 repository，將本壓縮檔內**所有檔案直接上傳至根目錄**（不要多包一層資料夾）。
2. 進入 **Settings → Pages**，Source 選 `Deploy from a branch`，Branch 選 `main`／`/ (root)`，按 Save。
3. 約 1–2 分鐘後即可由 `https://<帳號>.github.io/<repository>/` 開啟。

## 安裝至手機

- **Android（Chrome）**：開啟網址後按頁面上的「📲 安裝 App」按鈕，或瀏覽器選單 →「安裝應用程式」。
- **iOS（Safari）**：分享 →「加入主畫面」。

## 更新版本

修改任何檔案後，請將 `sw.js` 第 3 行的 `CACHE` 版本號加 1（例如 `prompt-gen-v2`），使用者重新開啟後即會取得新版。

---
設計：張朝順 PE/PhD
