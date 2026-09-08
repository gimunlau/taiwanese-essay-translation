# 台語散文翻譯歷程

中文散文 → 台灣台語的畢業製作網站。網站保存的不只是最後譯文，也呈現原文、V1、V2、V3、V4 與 FINAL 之間的修改歷程。

公開網站：https://gimunlau.github.io/taiwanese-essay-translation/

## 檔案結構

```
.
├── index.html
├── assets/
│   ├── style.css
│   └── app.js
├── data/
│   └── works.js
├── works/
│   └── sing-hun-e-kau-sing-hun-e-niau.html
└── .github/workflows/pages.yml
```

- `index.html`：首頁與八篇作品目錄。
- `assets/style.css`：全站共用排版與手機版樣式。
- `assets/app.js`：版本切換、案例展開、分類篩選及差異比較。
- `data/works.js`：第一篇的版本正文、案例、待確認問題與比較資料。
- `works/*.html`：每篇作品的獨立頁面骨架。
- `.github/workflows/pages.yml`：GitHub Pages 自動部署。

## 新增第二篇作品

1. 在 `works/` 複製第一篇 HTML，另存為第二篇的英文檔名，修改篇名與 WORK 編號。
2. 在 `data/` 新增第二篇資料檔，依 `works.js` 格式填入原文、各版正文、案例、待確認與版本差異。
3. 將第二篇 HTML 的資料檔路徑改成新資料檔。
4. 在 `index.html` 的作品列表加入 02 與連結。
5. 推送到 `main` 後，GitHub Pages 會自動更新。

## 內容原則

- 正文只採用各版本的實際正文。
- 忽略正文後附加的修正紀錄、修改紀錄或說明。
- 不自行改寫台語漢字、羅馬字、大小寫或特殊拼寫。
- 疑似錯字或語意問題放進「待確認」，不在正文暗中修正。
