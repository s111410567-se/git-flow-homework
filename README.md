# Git Flow 與 GitHub Flow 作業

## 學生資料

- 姓名：禚鎮龍
- 學號：111410567
- 科系：資訊工程學系
- 作業主題：Git Flow 與 GitHub Flow

---

## 一、作業目的

本次作業練習使用 Git 與 GitHub 進行版本控制，完成建立分支、提交修改、合併、Fork 及 Pull Request 等操作。

完成的項目如下：

1. 建立公開的 GitHub 儲存庫
2. 建立新的 Branch
3. 在 Branch 中新增檔案並提交
4. 建立 Pull Request
5. 將 Branch 合併到 main
6. Fork 原始儲存庫
7. 在 Fork 儲存庫中新增檔案
8. 從 Fork 建立 Pull Request
9. 將 Fork 的修改合併回原始儲存庫

本次主要使用 GitHub 網頁介面操作，並列出相對應的 Git 指令。

---

## 二、建立儲存庫

在 GitHub 組織 `s111410567-se` 中建立公開儲存庫。

- 儲存庫名稱：`git-flow-homework`
- 可見度：Public
- 建立 README.md
- 加入 Java 的 .gitignore

原始儲存庫：

https://github.com/s111410567-se/git-flow-homework

---

## 三、建立 Branch

在原始儲存庫建立分支：

`developGitBranch`

接著在此分支中新增：

`gitBranch.md`

對應的 Git 指令：

- `git clone https://github.com/s111410567-se/git-flow-homework.git`
- `cd git-flow-homework`
- `git switch -c developGitBranch`
- `git add gitBranch.md`
- `git commit -m "建立 gitBranch.md"`
- `git push -u origin developGitBranch`

指令說明：

- `git clone`：下載遠端儲存庫。
- `git switch -c`：建立並切換到新分支。
- `git add`：將檔案加入暫存區。
- `git commit`：建立一次版本提交。
- `git push`：將修改推送到 GitHub。

---

## 四、建立 Pull Request 與 Merge

完成 `developGitBranch` 的修改後，建立 Pull Request：

`developGitBranch → main`

Pull Request 標題：

`合併 developGitBranch 分支`

確認內容後，使用 Merge Pull Request 將分支內容合併到 main。

對應的 Git 指令：

- `git switch main`
- `git merge developGitBranch`
- `git push origin main`

第一次 Pull Request：

https://github.com/s111410567-se/git-flow-homework/pull/1

---

## 五、Fork 儲存庫

將組織中的原始儲存庫 Fork 到個人帳號。

- 原始儲存庫：`s111410567-se/git-flow-homework`
- Fork 儲存庫：`s111410567-web/git-flow-homework`

Fork 是將其他帳號或組織中的儲存庫複製到自己的 GitHub 帳號，讓使用者可以在自己的副本中修改內容。

Fork 儲存庫：

https://github.com/s111410567-web/git-flow-homework

---

## 六、在 Fork 中新增內容

在個人帳號的 Fork 儲存庫中新增檔案：

`studentFork.md`

提交訊息：

`新增 Fork 操作紀錄`

對應的 Git 指令：

- `git clone https://github.com/s111410567-web/git-flow-homework.git`
- `cd git-flow-homework`
- `git add studentFork.md`
- `git commit -m "新增 Fork 操作紀錄"`
- `git push origin main`

---

## 七、從 Fork 建立 Pull Request

完成 Fork 儲存庫的修改後，建立第二次 Pull Request。

來源：

`s111410567-web/git-flow-homework:main`

目標：

`s111410567-se/git-flow-homework:main`

Pull Request 標題：

`新增 Fork 操作紀錄`

第二次 Pull Request：

https://github.com/s111410567-se/git-flow-homework/pull/2

---

## 八、作業成果連結

### 原始儲存庫 main 分支提交紀錄

https://github.com/s111410567-se/git-flow-homework/commits/main

### developGitBranch 分支提交紀錄

https://github.com/s111410567-se/git-flow-homework/commits/developGitBranch

### Fork 儲存庫 main 分支提交紀錄

https://github.com/s111410567-web/git-flow-homework/commits/main

### 第一次 Pull Request

https://github.com/s111410567-se/git-flow-homework/pull/1

### 第二次 Pull Request

https://github.com/s111410567-se/git-flow-homework/pull/2

---

## 九、完成結果

- [x] 建立公開儲存庫
- [x] 建立 Branch
- [x] 在 Branch 中新增檔案
- [x] 提交 Commit
- [x] 建立 Pull Request
- [x] Merge 分支
- [x] Fork 儲存庫
- [x] 在 Fork 中新增檔案
- [x] 從 Fork 建立 Pull Request
- [x] 將 Fork 修改合併回原始儲存庫
