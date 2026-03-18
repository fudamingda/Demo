## Demo

這是一個用於測試 GitHub 流程的示範專案（Demo Repository）。

## 內容

- **目的**：練習/驗證 Git、GitHub、以及 `gh` CLI 的基本操作
- **狀態**：持續更新中

## 快速開始

### 1) 先安裝工具

- **Git**：確保 `git --version` 可正常執行
- **GitHub CLI (`gh`)**：確保 `gh --version` 可正常執行

### 2) 在本機初始化並提交

在 `Demo/` 目錄下執行（PowerShell）：

```bash
git init
git add .
git commit -m "docs: expand demo README"
```

### 3) 連到 GitHub 並推送

1. 先用 `gh` 登入（**請勿把 token 直接貼到指令或寫進檔案**）：

```bash
gh auth login
```

2. 建立遠端倉庫（或改用既有 repo URL）並推送：

```bash
gh repo create Demo --private --source . --remote origin --push
```

若你已有 GitHub repo，改成：

```bash
git remote add origin <你的repo.git>
git branch -M main
git push -u origin main
```

## 授權

本專案授權條款請見 `LICENSE`。
