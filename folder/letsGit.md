# 開始 Git [^git]
[^git]:學習內容為『為你自己寫 Git』一書。本人已購買電子版，有興趣詳細學習的可以參考網站內容或支持購買。 https://gitbook.tw/
## 開始 git bash 來建立資料夾以及讓 Git 可以管理這個資料夾
![image](https://hackmd.io/_uploads/rJan109Bp.png)

### 基本指令說明
**`$ pwd`** 顯示目前位置。  
**`$ ls`** 列出 list 。  
**`$ mkdir GitHub`** 建立新資料夾「GitHub」。  
**`$ cd GitHub`** 移到「GitHub」這個資料夾。  
**`$ git init`** 請 Git 對這個資料夾初始化，使 Git 可以代管這個資料夾。  
    `Git 會在這個資料夾裡面產生一個隱藏的.git 目錄，主要是靠這個 .git 在控管整個資料夾。如果刪掉之後就回不去了。`
    
## 接著來建立一個檔案並且 push 至暫存區。
![image](https://hackmd.io/_uploads/ByjgP-oSp.png)  
`這裡可以看到目前文件還是在 untracked 的狀態。`

### 建立檔案指令說明
**`$ echo "hello.git" > welcome.html`** 增加一個內含 hello.git 的文件。  
or **`touch welcome.html`** 直接建立一個空白的文件。  
**`$ git st`** 用來看目前的狀態 (status)。

![image](https://hackmd.io/_uploads/ryvEwWiH6.png)  
`把這個文件交給 git ，現在文件狀態變成 new file，表示文件已經被放到暫存區了。`

### 暫存區指令說明
**`$ git add 文件名`** 將文件交給 git。  
**`$ git add *.html`** 將所有副檔名 .html 的文件都加入暫存區。  
或 **`$ git add --all`** or **`$ git add .`** 全部檔案加到暫存區。  

📌 但 git add. 僅會儲存當下資料夾的所有文件；而 --all 則是全部資料夾的全部文件。

## 最後 commit 至 repository.
![image](https://hackmd.io/_uploads/rkV35ZjHp.png)  
`一定要 commit 完才算完整存到檔案。`

### 流程結束指令說明
**`$ git commit -m"版更的內容"`** 共編時一定要完善的寫下版更的原因跟地方唷。
儘量不要留 bug fixed 這樣模糊的描述，別人完全不知道修了哪裡。
**`$ git commit -a -m "update content"`**  懶惰的話也可以一次 add + commit，但只限於版更， [Untracked](#基本指令說明) file 是無法使用的。


`:pushpin: commit 的時候只會存已經在暫存區 (add) 的文件，如果不在暫存區裡面的 commit 是不會存到的。`

---
# 檢視紀錄
## 先來建一個新的文件
![image](https://hackmd.io/_uploads/BJw-OGjBa.png)

### 複習一下指令
**`$ touch 文件名`** 新增一個文件。  
**`$ git add 文件名.html`** 加入暫存區。  
**`$ git commit -m "說明文字"`** commit 上去。

## 檢視記錄
![image](https://hackmd.io/_uploads/S1tR_fsB6.png)

### 檢視的指令說明
`$ git log` 
這裡可以看到 commit 的作者、時間以及說明。

# :outbox_tray: 上傳到 GitHub
