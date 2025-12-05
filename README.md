# knowledge-base

個人文件知識庫 📚

## 簡介

這個 Repository 專門用來存放個人筆記，所有 HTML 或 Markdown 檔案依照類別放入其中，透過 GitHub Pages 提供線上查看使用。

🔗 **線上瀏覽**: [https://heimlichlin.github.io/knowledge-base/](https://heimlichlin.github.io/knowledge-base/)

## 目錄結構

```
knowledge-base/
├── index.md              # 首頁
├── _config.yml           # Jekyll 配置檔
├── notes/                # 筆記資料夾
│   ├── programming/      # 程式設計相關
│   ├── tools/            # 工具使用相關
│   └── misc/             # 其他筆記
└── README.md             # 本說明檔
```

## 如何新增筆記

1. 在對應的類別資料夾中創建新的 `.md` 或 `.html` 檔案
2. 如果是 Markdown 檔案，建議在檔案開頭加入 YAML Front Matter：
   ```yaml
   ---
   layout: default
   title: 你的筆記標題
   ---
   ```
3. 更新對應類別的 `index.md` 檔案，添加新筆記的連結

## 本地預覽

如果想在本地預覽，可以安裝 Jekyll 並執行：

```bash
gem install bundler jekyll
bundle install
bundle exec jekyll serve
```

然後在瀏覽器中開啟 `http://localhost:4000/knowledge-base/`

## 授權

本知識庫內容僅供個人學習使用
