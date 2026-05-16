# YUIMOM 精選物業 — 測試包（v3 完整版）

## 這版的內容

✓ 中文 5 頁：首頁 + 海邊 / 中山 / 長茁 / 保泰
✓ 英文 5 頁：Overview + Haibian / Zhongshan / Evergreen / Baotai
✓ 業種卡片各頁主推 3 張（保泰 2 張），其他用「亦適合」一行帶過
✓ 地段周邊統一 4 條（手機友善）
✓ 手機版底部固定 CTA Bar
✓ 全站 SEO 完整（hreflang、JSON-LD、FAQ）

## 使用方式

### 1. 開新 GitHub repo 測試
- 名稱建議：`yuimom-landing-test`
- 設為 **Public**
- **不要**勾任何初始化選項

### 2. 把這個資料夾的全部內容丟進 repo
```
yuimom-landing-test/
├── index.html
├── haiban/ zhongshan/ changzhuo/ baotai/
├── en/index.html
├── en/haiban/ en/zhongshan/ en/changzhuo/ en/baotai/
├── assets/css/main.css
├── assets/js/main.js
├── images/        ← 空的，要自己補
├── pdf/           ← 空的，可選
├── sitemap.xml
├── robots.txt
└── README.md
```

### 3. 補圖片
從你正式 repo（`yylin1110jp-creator/yuimom-landing`）的 `images/` 複製整個資料夾，內容必須包含：

- logo_hero.png, logo_nav.png
- favicon-192.png, apple-touch-icon.png
- haiban.jpg ~ haiban4.jpg
- zhongshan.jpg ~ zhongshan3.jpg
- changzhuo.jpg ~ changzhuo3.jpg
- baotai.jpg, baotai3.jpg, baotai4.jpg
- og-image.jpg

從正式 repo 把 `favicon.ico` 複製到 repo 根目錄。

### 4. 補 PDF（選用）
從正式 repo 的 `pdf/` 把 4 個 PDF 複製過來。

### 5. 開啟 GitHub Pages
- Settings → Pages
- Source: `Deploy from a branch` → `main` / `/ (root)`
- **不要**設 custom domain（保持 `username.github.io/repo-name/`）

幾分鐘後測試版會在：
`https://yylin1110jp-creator.github.io/yuimom-landing-test/`

## 測試重點

### 桌機
- 首頁、4 個建案頁、4 個英文建案頁 都可正常開
- 語言切換（EN / 中）按鈕對應頁面正確切換
- 右下角 LINE 浮動按鈕顯示

### 手機
- 底部固定 CTA Bar：左「立即洽詢」、右「LINE 諮詢」
- 右下角 LINE 浮動按鈕**消失**（避免重疊）
- 業種卡片各頁主推 3 張、保泰 2 張
- 地段周邊各頁 4 條

### SEO 結構
每個建案頁應該有：
- 頁籤 Title 含坪數和規格
- 適合業種 3 張卡片
- 地段周邊 4 條
- FAQ 6 題
- 下方 PDF 下載 bar

---

## 之後上正式版

確認測試版沒問題後，跟我說一聲，我給你正式版 zip（絕對路徑 + CNAME），就可以直接推到正式 repo `yuimom-landing` 取代舊的 SPA 版本。
