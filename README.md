# NotebookLM 圖片自動打包工具

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Live-brightgreen)](https://你的使用者名稱.github.io/20251105_1330_public_png-to-notebooklm/)

> 一鍵將 Google 雲端硬碟資料夾中的所有圖片打包成一份 Google 文件，完美整合 NotebookLM 使用流程。

## 📋 專案簡介

這是一套「一次性部署」工具，讓你可以快速將 Google 雲端硬碟資料夾內的所有圖片自動彙整成單一 Google 文件。設定完成後，只需點擊書籤列上的按鈕，即可完成圖片打包作業。

### 🎯 主要功能

- **一鍵打包**：透過瀏覽器書籤按鈕，一鍵將資料夾內所有圖片打包成 Google 文件
- **自動化處理**：利用 Google Apps Script 建立個人專屬的 Web App
- **無需重複設定**：一次部署，永久使用
- **安全可靠**：所有資料都在你的 Google 帳號內處理，不經過第三方伺服器

### 🛠️ 系統組成

1. **部署 SOP 網頁**：互動式部署教學面板
2. **圖片快速轉檔工具**：Windows 桌面應用程式（.exe）
3. **Google Apps Script**：後端處理引擎

## 🚀 快速開始

### 線上部署教學

👉 **[立即前往部署面板](https://你的使用者名稱.github.io/20251105_1330_public_png-to-notebooklm/)**

部署面板提供完整的互動式教學，只需跟著步驟操作：

1. **建立引擎**：從範本建立或手動建立 Google Apps Script
2. **部署 Web App**：設定並授權 Web 應用程式
3. **產生書籤**：自動生成專屬書籤代碼
4. **安裝書籤**：將書籤加入瀏覽器書籤列
5. **開始使用**：進入任何 Google Drive 資料夾，點擊書籤即可打包圖片

### 下載工具

📥 **[下載圖片快速轉檔工具 (.exe)](./20251105-1142-圖片快速轉檔.exe)**

此工具可以幫助你在上傳圖片到 Google 雲端硬碟前，快速進行格式轉換或壓縮。

## 💡 使用情境

### 適合以下需求：

- 📚 **學習筆記整理**：將課堂拍攝的白板照片快速整理成文件
- 📊 **會議記錄彙整**：將會議中的簡報截圖統一打包
- 🎨 **設計素材管理**：將設計草圖或參考圖片整理成冊
- 📝 **研究資料整理**：將研究過程中的圖表、數據截圖彙整
- 🤖 **NotebookLM 輸入**：整理好的 Google 文件可直接匯入 NotebookLM 進行 AI 分析

## 🔧 技術架構

```
瀏覽器書籤 (JavaScript)
    ↓
    ↓ 傳送資料夾 URL
    ↓
Google Apps Script (Web App)
    ↓
    ↓ 讀取資料夾內容
    ↓
Google Drive API
    ↓
    ↓ 建立 Google 文件
    ↓
    ↓ 插入圖片
    ↓
完成！(輸出到原資料夾)
```

### 核心技術

- **前端**：HTML5, Tailwind CSS, Vanilla JavaScript
- **後端**：Google Apps Script (JavaScript)
- **API**：Google Drive API, Google Docs API
- **部署**：GitHub Pages

## 📖 詳細說明

### 書籤按鈕運作原理

書籤使用 `javascript:` 協議執行以下流程：

1. 檢查當前頁面是否為 Google Drive 資料夾頁面
2. 提取資料夾 URL
3. 將 URL 作為參數傳送給你的 Web App
4. Web App 處理圖片並建立 Google 文件
5. 在新分頁顯示處理結果

### 安全性說明

- ✅ 所有程式碼開源透明
- ✅ Web App 設定為「僅限我自己」存取
- ✅ 不會將資料傳送到第三方伺服器
- ✅ 所有處理都在你的 Google 帳號內完成

## 🤝 貢獻

歡迎提交 Issue 或 Pull Request！

### 開發建議

如果你想要修改或擴充功能：

1. Fork 本專案
2. 修改 `index.html` 中的部署面板內容
3. 調整 Apps Script 程式碼以增加功能
4. 提交 Pull Request

## 📝 版本資訊

### SOP 4.0 (2025-11-05)

- ✨ 優化部署流程，新增範本選項
- 🎨 改進 UI 設計，採用 Google 風格
- 📱 增強響應式設計，支援行動裝置
- 🔧 新增互動式書籤代碼生成器

### SOP 3.0

- 🚀 引入 Web App 架構
- 📦 整合一鍵打包功能

## 🙋 常見問題

### Q: 需要付費嗎？
A: 完全免費！只需要有 Google 帳號即可使用。

### Q: 支援哪些圖片格式？
A: 支援所有 Google Drive 支援的圖片格式（JPG, PNG, GIF, BMP, WebP 等）。

### Q: 可以處理多少張圖片？
A: 理論上沒有限制，但 Google Apps Script 有執行時間限制（約 6 分鐘），建議一次處理 100 張以內的圖片。

### Q: 書籤無法執行怎麼辦？
A: 請確認：
1. 你在 Google Drive 的資料夾頁面（URL 包含 `/folders/`）
2. 書籤代碼完整複製（以 `javascript:` 開頭）
3. Web App 已正確部署並授權

### Q: 可以用在公司/學校的 Google Workspace 嗎？
A: 可以，但需要確認你的組織管理員允許執行 Apps Script。

---

⭐ 如果這個工具對你有幫助，歡迎給個 Star！

**製作日期**：2025年11月5日
