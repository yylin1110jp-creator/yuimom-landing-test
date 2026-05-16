# YUIMOM 精選物業 — 測試包 v2

## 這版的改動

✓ 業種卡片從 7 張 → **3 張**（銀行、餐廳、共享辦公）
✓ 地段周邊從 10 個 → **4 個**（輕軌、流行音樂中心、展覽館＋港埠、漢神）
✓ 新增手機版底部固定 CTA Bar（左：立即洽詢｜右：LINE 諮詢）
✓ 桌機版維持右下角 LINE 浮動按鈕；手機版自動隱藏避免重疊
✓ 海邊頁中文 1747 字（精簡後仍含完整 SEO 結構）

---

## 使用方式

### 1. 開新 GitHub repo
- 名稱建議：`yuimom-landing-test`
- 設為 **Public**
- **不要勾** Add README / .gitignore / license

### 2. 把這個資料夾的所有檔案丟進 repo
```
yuimom-landing-test/
├── index.html              ← 首頁
├── haiban/index.html       ← 海邊頁（SEO 完整版）
├── zhongshan/index.html    ← 占位頁
├── changzhuo/index.html    ← 占位頁
├── baotai/index.html       ← 占位頁
├── assets/
│   ├── css/main.css
│   └── js/main.js
├── images/                 ← ⚠️ 空的，要從原 repo 複製進來
└── pdf/                    ← ⚠️ 空的（選用）
```

### 3. 補上圖片
從你 `yuimom-landing` 的 `images/` 複製這幾個必要的：

```
images/
├── logo_hero.png        ← Hero 區大 LOGO
├── logo_nav.png         ← 頂部 nav LOGO
├── favicon-192.png
├── apple-touch-icon.png
├── haiban.jpg ~ haiban4.jpg
├── zhongshan.jpg        ← 首頁卡片用
├── changzhuo.jpg        ← 首頁卡片用
├── baotai.jpg           ← 首頁卡片用
└── og-image.jpg
```

`favicon.ico` 放根目錄。

### 4. 啟用 GitHub Pages
- Settings → Pages
- Source: Deploy from a branch → `main` / `(root)`
- **不要**設 custom domain

網址：`https://yylin1110jp-creator.github.io/yuimom-landing-test/`

---

## 測試重點

### 手機 (760px 以下)
- ✅ 底部固定 CTA Bar 一直在
- ✅ 右下角 LINE 浮動按鈕應該消失
- ✅ 業種卡 3 張，每張很短可滑完
- ✅ 地段 4 條，一眼看完

### 桌機
- ✅ 右下角 LINE 浮動按鈕在
- ✅ 底部 CTA Bar 不顯示
- ✅ 視覺風格跟原本一致

---

## 已知未完成

- 中山/長茁/保泰 中文完整 SEO 頁面（目前是占位頁）
- 全站英文版（`/en/...`）
- `sitemap.xml` 更新

確認測試版視覺/體驗 OK 後，會繼續完成。
