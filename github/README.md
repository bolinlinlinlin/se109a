# Git/Github心得

## Git 是一種「分散式」版本的「版本控制」系統：
過去「集中式」版本控制系統中，需要一台專用的伺服器，所有的更新都需要跟這台伺服器溝通。也就是說，萬一這台伺服器壞了，或是沒有網路連線的環境，版本控制功能就沒辦法使用。

而 Git 使用「分散式」的優點是，即使在沒有伺服器或是沒有網路的環境，依舊可以使用 Git 來進行版控，待伺服器恢復正常運作或是在有網路的環境後再進行同步，不會受影響。而且，事實上在使用 Git 的過程中，大多的 Git 操作也都是在自己電腦本機就可以完成。
## 安裝 Git
```
Windows: 官網下載 Git 
Mac: $ brew install git  
Linux: $ apt-get install git
```
## 在目前工作區 (Workspace) 內建立一個 .git folder
```
$ git init
```
## 設定 Git config 環境
```
$ git config --global user.name "Max"
$ git config --global user.email "user@gmail.com”
```
## Github 下載資料庫 (Remote Repository) 至目前工作區 (Workspace)
```
$ git clone <repo URL>
```
## git add 建立索引
工作目錄 (Working Directory) 內所有檔案建立索引
```
$ git add .
```
## git commit 至本地資料庫
```
$ git commit -m "add helloword.txt"
```
## git push 至 GitHub
上傳指定分支至 Git 目錄
```
$ git push origin master
```
# 實作
## 找到一個喜歡的把它git clone下來

<img src=".\clone.jpg" width = "40%"><br>
<img src=".\clone1.jpg" width = "40%"><br>

就可以使用了

## 完成部分東西可以回推回去
