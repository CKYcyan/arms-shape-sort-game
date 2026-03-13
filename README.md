# ARMS 展覽互動

展場用的小遊戲與圖鑑入口。

## 資料夾結構

```
GAME/
├── index.html              ← 首頁（從這裡連到各區）
├── shape_sort_game.html   ← 形狀分類小遊戲
├── gallery/               ← 圖鑑
│   ├── index.html          ← 圖鑑首頁
│   └── images/             ← 圖鑑用的圖片放這裡
└── README.md
```

## 連結怎麼寫

- **從首頁連到遊戲**：`shape_sort_game.html` 或 `./shape_sort_game.html`
- **從首頁連到圖鑑**：`gallery/index.html` 或 `gallery/`
- **從圖鑑回首頁**：`../index.html`
- **圖鑑裡放圖片**：放在 `gallery/images/`，HTML 裡用 `images/檔名.jpg`

## GitHub Pages 網址

啟用後會是：`https://CKYcyan.github.io/arms-shape-sort-game/`

- 首頁：`https://CKYcyan.github.io/arms-shape-sort-game/`
- 遊戲：`https://CKYcyan.github.io/arms-shape-sort-game/shape_sort_game.html`
- 圖鑑：`https://CKYcyan.github.io/arms-shape-sort-game/gallery/`
