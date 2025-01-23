
# 【使用GitHub CLI創建新的GitHub】



以下是更新後的Markdown指南，包含使用 `gh repo create my-new-repo --public` 指令來創建GitHub倉庫：

```markdown
# 在本地端建立新的 Git Repository 並推送到 GitHub

## 步驟 1：安裝 Git 和 GitHub CLI
首先，確保你已經安裝了 Git 和 GitHub CLI。如果你還沒有安裝，可以從以下網站下載並安裝：
- [Git 官方網站](https://git-scm.com/)
- [GitHub CLI 官方網站](https://cli.github.com/)

## 步驟 2：創建新的目錄
在本地端創建一個新的目錄，作為你的新專案的根目錄。

```sh
mkdir my-new-repo
cd my-new-repo
```

## 步驟 3：初始化 Git Repository
在目錄中初始化一個新的 Git repository。

```sh
git init
```

## 步驟 4：創建 README 文件
創建一個 README 文件，作為專案的簡介。

```sh
echo "# My New Repository" > README.md
```

## 步驟 5：添加文件到 Git
將 README 文件添加到 Git 的暫存區。

```sh
git add README.md
```

## 步驟 6：提交更改
提交添加的文件，並撰寫提交訊息。

```sh
git commit -m "Initial commit"
```

## 步驟 7：使用 GitHub CLI 創建新的 GitHub Repository
使用 GitHub CLI 創建一個新的公開 GitHub repository。

```sh
gh repo create my-new-repo --public
```

## 步驟 8：連接本地端 Repository 到 GitHub
執行完上一步後，GitHub CLI 會自動將本地端的 Git repository 連接到 GitHub 上的 repository。如果沒有自動連接，你可以手動連接：

```sh
git remote add origin https://github.com/your-username/my-new-repo.git
```

## 步驟 9：推送本地端 Repository 到 GitHub
將本地端的提交推送到 GitHub。

```sh
git push -u origin main
```

## 完整指令
以下是完整的指令流程：

```sh
mkdir my-new-repo
cd my-new-repo
git init
echo "# My New Repository" > README.md
git add README.md
git commit -m "Initial commit"

## 建置遠端Repo，並連上之
gh repo create my-new-repo --public
git push -u origin main
```

## 總結
這份指南教你如何在本地端建立新的 Git repository，並將其推送到 GitHub。


## 補充資料對照用

```sh
echo "# MyTemp" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main

## 掛入遠端Repo(事先用線上GitHub建好)
git remote add origin https://github.com/samofor/MyRepoNew.git
git add .
git commit -m "First commit" 
git branch -M main
git push -u origin main
```