# 形狀分類小遊戲 (Arms Shape Sort Game)

一款以拖放方式進行形狀分類的互動小遊戲，使用純 HTML + CSS + JavaScript 製作，無須安裝任何相依套件，直接用瀏覽器開啟即可遊玩。

## 執行方式

```
直接用瀏覽器開啟 shape_sort_game.html 即可。
```

---

## 多人版本協作指南

本專案使用 **Git** 進行版本控制，並透過 **GitHub** 進行遠端協作。以下說明如何讓同事加入協作。

### 前置需求

- 安裝 [Git](https://git-scm.com/downloads)
- 擁有 [GitHub](https://github.com) 帳號

---

### 步驟一：授予同事存取權限（Repository Owner 操作）

1. 前往 GitHub 上的專案頁面：`https://github.com/CKYcyan/arms-shape-sort-game`
2. 點選上方 **Settings** 分頁
3. 在左側選單選擇 **Collaborators**（或 **Collaborators and teams**）
4. 點選 **Add people**，輸入同事的 GitHub 帳號或信箱，送出邀請
5. 同事收到邀請 Email 後，接受邀請即可取得協作權限

---

### 步驟二：同事 Clone 專案到本機

同事接受邀請後，執行以下指令將專案複製到本機：

```bash
git clone https://github.com/CKYcyan/arms-shape-sort-game.git
cd arms-shape-sort-game
```

---

### 步驟三：建立功能分支（推薦的協作流程）

**避免直接在 `main` 分支上修改**，請每次新增功能或修正問題時建立獨立分支：

```bash
# 確保本機 main 是最新狀態
git checkout main
git pull origin main

# 建立並切換到新分支（分支名稱請使用英文、以 - 分隔）
git checkout -b feature/your-feature-name
```

分支命名範例：

| 類型 | 命名格式 | 範例 |
|------|----------|------|
| 新功能 | `feature/<功能描述>` | `feature/add-timer` |
| 修正 Bug | `fix/<問題描述>` | `fix/drag-drop-on-mobile` |
| 樣式調整 | `style/<調整描述>` | `style/update-button-color` |

---

### 步驟四：提交變更

```bash
# 查看目前修改的檔案
git status

# 將修改的檔案加入暫存區
git add shape_sort_game.html

# 提交，並寫上清楚的說明
git commit -m "feat: 新增計時功能"
```

**Commit 訊息建議格式：**

```
<類型>: <簡短說明>

類型可使用：
  feat     新功能
  fix      修正 Bug
  style    樣式或格式調整（不影響功能）
  refactor 重構（不新增功能也不修 Bug）
  docs     文件更新
```

---

### 步驟五：推送分支並發起 Pull Request

```bash
# 將分支推送到 GitHub
git push origin feature/your-feature-name
```

接著：

1. 前往 GitHub 專案頁面，會出現「Compare & pull request」的提示
2. 點選後填寫 PR 說明，描述你做了什麼改動
3. 指派給負責 Review 的人（Reviewer）
4. Review 通過後，由負責人將分支合併（Merge）到 `main`

---

### 步驟六：同步最新進度

當他人合併了新的變更，請定期同步 `main` 分支：

```bash
git checkout main
git pull origin main

# 若你正在開發中的分支需要包含最新 main 的變更
git checkout feature/your-feature-name
git merge main
```

---

## 專案結構

```
arms-shape-sort-game/
├── shape_sort_game.html   # 遊戲主檔案（HTML + CSS + JS 合併於單一檔案）
├── .gitignore             # Git 忽略設定
└── README.md              # 本說明文件
```

---

## 常用 Git 指令速查

| 指令 | 說明 |
|------|------|
| `git status` | 查看目前修改狀態 |
| `git pull origin main` | 拉取遠端最新變更 |
| `git checkout -b <branch>` | 建立並切換到新分支 |
| `git add <file>` | 將檔案加入暫存 |
| `git commit -m "<message>"` | 提交變更 |
| `git push origin <branch>` | 推送分支到遠端 |
| `git log --oneline` | 查看提交紀錄 |
| `git diff` | 查看尚未暫存的變更內容 |
