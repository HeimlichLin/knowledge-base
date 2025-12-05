---
layout: default
title: Git 基本指令
---

# Git 基本指令

這是一個範例筆記，展示如何在此知識庫中添加筆記。

## 常用指令

### 初始化與設定

```bash
# 初始化新的 Git 倉庫
git init

# 設定使用者名稱
git config --global user.name "Your Name"

# 設定使用者信箱
git config --global user.email "your.email@example.com"
```

### 基本操作

```bash
# 查看狀態
git status

# 添加檔案到暫存區
git add <file>
git add .

# 提交變更
git commit -m "提交訊息"

# 查看歷史紀錄
git log
git log --oneline
```

### 分支操作

```bash
# 查看分支
git branch

# 創建新分支
git branch <branch-name>

# 切換分支
git checkout <branch-name>

# 創建並切換到新分支
git checkout -b <branch-name>

# 合併分支
git merge <branch-name>
```

### 遠端操作

```bash
# 添加遠端倉庫
git remote add origin <url>

# 推送到遠端
git push -u origin main

# 從遠端拉取
git pull origin main

# 克隆倉庫
git clone <url>
```

---

[← 返回工具筆記](index.md) | [← 返回首頁](../../)
