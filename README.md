# 影像工作台

照片 AI 去背、影片臉部馬賽克、影片轉 GIF、GoPro 影片瘦身，四個工具放在同一頁。所有處理都在你的瀏覽器裡完成，照片和影片不會上傳。

## 怎麼用
打開 GitHub Pages 網址即可（Settings → Pages 開啟後顯示）。

- **照片去背**：選照片 → 自動去背 → 用筆刷修邊 → 存成透明 PNG。手機可存到相簿，電腦可選存檔位置。
- **臉部馬賽克**：選影片 → 逐格分析臉部（動作快也抓得到，空檔自動補上）→ 預覽、用時間軸檢查 → 匯出新影片。
- **影片轉 GIF**：選影片 → 拉出片段 → 調寬度、幀率、色彩數 → 產生 GIF，也能匯出每幀 PNG。
- **影片瘦身**：電腦版 Chrome / Edge，把 GoPro 影片壓小。

## 檔案
- `index.html`：整個工具頁
- `data/`：去背模型（IMG.LY background-removal 1.4.5 / ISNet）與 onnxruntime，切成 4MB 小檔
- `models/`：臉部偵測模型（face-api）

## 使用的開源專案
- [@imgly/background-removal](https://github.com/imgly/background-removal-js)（AGPL-3.0）
- [@vladmandic/face-api](https://github.com/vladmandic/face-api)（MIT）
- [Mediabunny](https://github.com/Vanilagy/mediabunny)（MPL-2.0）
