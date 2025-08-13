# JPY/TWD 換 KRW 判斷器 (PWA)

一個專為外匯兌換決策設計的 Progressive Web App，幫助您快速判斷使用台幣或日幣兌換韓元哪個更划算。

## 🌟 功能特色

- **即時匯率比較**：比較台幣→韓元與日幣→韓元的兌換成本
- **智能判斷**：自動計算門檻匯率並給出最佳兌換建議
- **PWA 支援**：可安裝到桌面，支援離線使用
- **響應式設計**：完美適配手機、平板、桌面設備
- **深色主題**：支援淺色/深色主題切換
- **直觀介面**：簡潔美觀的現代化 UI 設計

## 📱 使用方式

1. **輸入匯率資訊**：
   - 台幣→韓元匯率（現場看板上的 TWD→KRW 數字）
   - 日幣→韓元匯率（現場看板上的 JPY→KRW 數字）
   - 您的日幣成本（預設 0.21 台幣/日圓）

2. **選擇性輸入**：
   - 想兌換的韓元金額（可選，不填則只判斷哪個更划算）

3. **獲取結果**：
   - 系統會計算門檻匯率
   - 比較兩種兌換方式的成本
   - 給出最佳兌換建議
   - 如需兌換，會顯示所需台幣和日幣金額

## 🚀 安裝方式

### 方法一：直接使用
1. 在瀏覽器中開啟 `index.html`
2. 點擊瀏覽器的「安裝」按鈕或「新增到主畫面」

### 方法二：本地部署
1. 下載所有檔案到本地資料夾
2. 使用任何 HTTP 伺服器（如 Live Server）啟動
3. 在瀏覽器中開啟並安裝

## 🛠 技術架構

- **前端**：純 HTML5 + CSS3 + JavaScript
- **PWA 功能**：Service Worker + Web App Manifest
- **響應式設計**：CSS Grid + Flexbox
- **主題系統**：CSS 變數 + localStorage
- **離線支援**：Service Worker 快取策略

## 📁 專案結構

```
jpy_twd_krw_pwa/
├── index.html          # 主應用程式檔案
├── manifest.json       # PWA 設定檔
├── sw.js              # Service Worker
├── favicon.ico        # 網站圖示
├── icons/             # PWA 圖示集
│   ├── icon-48x48.png
│   ├── icon-72x72.png
│   ├── icon-96x96.png
│   ├── icon-128x128.png
│   ├── icon-144x144.png
│   ├── icon-152x152.png
│   ├── icon-192x192.png
│   ├── icon-256x256.png
│   ├── icon-384x384.png
│   └── icon-512x512.png
└── README.md          # 專案說明文件
```

## 💡 使用場景

- **旅遊兌換**：在韓國旅遊時快速決定兌換策略
- **外匯投資**：比較不同幣別的兌換成本
- **即時決策**：在匯率看板前快速做出兌換決定
- **成本分析**：分析不同兌換方式的成本差異

## 🔧 開發說明

### 本地開發
```bash
# 使用 Python 簡易伺服器
python -m http.server 8000

# 或使用 Node.js live-server
npx live-server
```

### 自訂設定
- 修改 `manifest.json` 調整 PWA 設定
- 編輯 CSS 變數自訂主題色彩
- 調整 `sw.js` 優化快取策略


---

**Made for quick on-the-spot exchange decisions.** 💱                