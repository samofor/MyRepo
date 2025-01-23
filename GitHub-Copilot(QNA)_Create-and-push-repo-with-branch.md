
# 【建置新的Git repository並推送到GitHub】

- 以下是用Markdown語法寫成的詳細操作步驟，教你如何在本地端環境下建置新的Git repository並推送到GitHub，然後創建一個新的branch：


- 在本地端建立新的 Git Repository 並推送到 GitHub，然後創建新分支

## 步驟 1：安裝 Git 和 GitHub CLI
首先，確保你已經安裝了 Git 和 GitHub CLI。如果你還沒有安裝，可以從以下網站下載並安裝：
- [Git 官方網站](https://git-scm.com/)
- [GitHub CLI 官方網站](https://cli.github.com/)

## 步驟 2：創建新的目錄
在本地端創建一個新的目錄，作為你的新專案的根目錄。

```sh
mkdir MyRepo
cd MyRepo
```

## 步驟 3：初始化 Git Repository
在目錄中初始化一個新的 Git repository。

```sh
git init
```

## 步驟 4：創建 README 文件
創建一個 README 文件，作為專案的簡介。

```sh
echo "# MyRepo" > README.md
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
gh repo create MyRepo --public
```

## 步驟 8：推送本地端 Repository 到 GitHub
將本地端的提交推送到 GitHub。

```sh
git push -u origin main
```

## 步驟 9：在 GitHub 上創建新分支
創建名稱為 `MyBranch` 的新分支。

```sh
git checkout -b MyBranch
git push -u origin MyBranch
```

## 完整指令
以下是完整的指令流程：

```sh
mkdir MyRepo
cd MyRepo
git init
echo "# MyRepo" > README.md
git add README.md
git commit -m "Initial commit"
gh repo create MyRepo --public
git push -u origin main
git checkout -b MyBranch
git push -u origin MyBranch
```

## 總結
這份指南教你如何在本地端建立新的 Git repository，並將其推送到 GitHub，然後創建一個新的分支。希望這對你的學習有幫助！如果有任何問題，隨時告訴我！

```sh
你可以將以上內容複製到一個Markdown文件（例如：`create-and-push-repo-with-branch.md`）中，然後下載或使用Markdown查看器來閱讀。希望這對你的學習有幫助！
```