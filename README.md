# YUIMOM 精選物業 — 測試包

這是給你在新 GitHub repo 測試用的版本。包含：

- 首頁（中文）`/`
- 海邊大面寬店面（中文，SEO 完整版）`/haiban/`
- 中山/長茁/保泰：占位頁（Coming Soon）

---

## 使用方式

### 1. 開新 GitHub repo
- 名稱建議：`yuimom-landing-test`
- 設為 **Public**
- **不要勾** Add README / .gitignore / license

### 2. 把這個資料夾的所有檔案丟進 repo
解壓後資料夾結構：
```
yuimom-landing-test/
├── index.html              ← 首頁
├── favicon.ico             ← 你既有的
├── haiban/index.html       ← 海邊頁（SEO 完整版）
├── zhongshan/index.html    ← 占位頁
├── changzhuo/index.html    ← 占位頁
├── baotai/index.html       ← 占位頁
├── assets/
│   ├── css/main.css
│   └── js/main.js
├── images/                 ← ⚠️ 空的，你要自己放圖
└── pdf/                    ← ⚠️ 空的，你要自己放 PDF
```

### 3. 補上圖片（必須）

把這些圖片放進 `images/` 資料夾（從你原本的 repo 複製即可）：

```
images/
├── logo_hero.png        ← Hero 區大 LOGO
├── logo_nav.png         ← 頂部 nav LOGO
├── favicon-192.png      ← favicon 192x192
├── apple-touch-icon.png ← iOS 桌面圖示
├── haiban.jpg           ← 海邊建案主圖
├── haiban2.jpg          ← 海邊圖 2
├── haiban3.jpg          ← 海邊圖 3
├── haiban4.jpg          ← 海邊圖 4
├── zhongshan.jpg        ← 中山主圖（首頁用）
├── changzhuo.jpg        ← 長茁主圖（首頁用）
├── baotai.jpg           ← 保泰主圖（首頁用）
└── og-image.jpg         ← OG 社群分享預覽圖 1200×630
```

> 占位頁不需要圖片，所以中山/長茁/保泰只要主圖一張即可（首頁卡片用）。
> 完整版完成後會用到更多圖。

### 4. 補上 PDF（選用）
```
pdf/
└── haiban.pdf
```
沒放也沒關係，點下載會 404 但不影響其他功能。

### 5. 啟用 GitHub Pages
- Settings → Pages
- Source: Deploy from a branch
- Branch: `main` / `(root)`
- **不要** 設 custom domain（保持 `username.github.io/repo-name/`）

幾分鐘後，網址就是：
`https://yylin1110jp-creator.github.io/yuimom-landing-test/`

---

## 路徑說明

**此測試包用的是相對路徑**（`./assets/`、`../images/`）。
所以可以放在 GitHub Pages 子目錄底下。

**之後如果要 deploy 到正式網域 `yuimom.site`**，需要改回絕對路徑（`/assets/`、`/images/`）。等你確認測試版 OK 後，我會給你正式版本。

---

## 測試重點

1. **首頁** — 視覺風格是否跟你原本的一致？
2. **海邊頁** — 滾下去看「適合業種」7 張卡片、地段周邊、FAQ。文案 OK 嗎？
3. **中山/長茁/保泰** — 應該都是 Coming Soon 占位頁。
4. **行動裝置** — 漢堡選單、響應式佈局是否正常？
5. **語言切換按鈕（EN）** — 點下去會 404（因為英文版還沒做）。

---

## 已知未完成項目

- 中山/長茁/保泰 中文完整 SEO 頁面
- 全站英文版（`/en/...`）
- `sitemap.xml` 更新
- 部分區塊文案微調

確認測試版 OK 後我會繼續完成這些。
