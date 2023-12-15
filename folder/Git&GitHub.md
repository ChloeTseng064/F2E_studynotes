科普 [^Git]
---

> - Git 幼幼班
> - Git 指令

### 為什麼我們要用 Git 以及 使用GitHub ?
GitHub 優點：協作與分享。
* 分享：GitHub 是世界上最大的代碼存放網站與開源社區, 對新手來說可以從別人的 code 中去學習 coding。
* Git 多人協作：Fork & Pull Request.[^pullrequest]
[^pullrequest]:多人協作筆記 -[Pull Request]()
* Git 版本管理 [^Git指令]：除了可以儲存每一次的版本，還可以精準的知道版本間的差別。
[^Git指令]: Git 指令筆記 - [Git 指令]()
## Git Repository
在 GitHub 上面，我們會建立我們的 Git 項目倉庫 (Git Repository)。


## 存檔(版本) 
可以想像倉庫中有一位叫 **MASTER** 👷🏻 的管理員在幫我們進行存/讀檔的工作。而每一次的變動都是一個新的版本。

:desktop_computer:**顯示 MASTER 頁面**

  `版本 1 的 code.`  
  `版本 2 的 code.`  
  `版本 3 的 code.`  
  `版本 4 的 code.`  

 **MASTER** 👷🏻 HI~
 版1--版2--版3--版4
 
 
## 分支 (BRANCH)

💡 一次只能招喚一個管理員 👷🏻 幫我們工作。但是可以一直切換不同的管理員做事。

:desktop_compute:**顯示 MASTER 頁面**  

  `版本 1 的 code.`  
  `版本 2 的 code.`  
  `版本 3 的 code.`  
  `修 bug 的 code.`  
  `版本 5 的 code.`    
  
原本的 MASTER 管理員。
💻**MASTER** 版1--版2--版3--修bug--版5

多請了一位叫 FIXBUG 的管理員，並且讀取了 MASTER 管理員的『存3』文件。

💻**FIXBUG** 版3--修bug

修個 bug 之後，再把檔案再存回去 MASTER 並且繼續後續的 coding。

MASTER 的『版3』文件不會消失，而 FIXBUG 的『版3』也是獨立的存在。

可以認為只是抓取了其中一個版本作為顯示，分支間的內容是完全獨立的。

## 合併
只是把其中分支上的存檔，合併到了 MASTER 上，並不會刪除或消失任何一段存檔。
![image](https://hackmd.io/_uploads/Bkb5m2FH6.png)[^Git]

## GitHub 界面
### 搜尋
![image](https://hackmd.io/_uploads/HJxY52Kra.png)
* 用戶(或組織名稱)/css(倉庫名稱)
* 倉庫簡介
* topic 標籤
* ○ 主要語言 ☆ 收藏 最後更新時間 `3 issues need help` (別人提待解決的問題)

### 主界面
![image](https://hackmd.io/_uploads/S1B12ntr6.png)
**README** 副檔名 md 表示這是一個用 Mark Down 寫成的文件。
倉庫下方都會默認顯示 README 檔案。

![image](https://hackmd.io/_uploads/HJq9n2tST.png)
這裡可以直接下載這個倉庫的全部資料夾及文件到自己的電腦。
也可以按上面 Watch ，隨時有更新的話會提醒你；或是按 Star 做收藏。
Fork 則是複製整個項目到自己的倉庫。

就算完全不懂 code 也可以將自己的文件上傳做備存或分享。
![image](https://hackmd.io/_uploads/rJDRJ6YHp.png)
檔案上傳完成後再按 commit changes 就可以完成上傳了。
![image](https://hackmd.io/_uploads/SJNjlpFrT.png)
也可以寫上一些改版的描述以及這裡就會問你需不需要存成 new branch 。

>**start a pull request**
通知原作者拉回這個請求 Pull Request (PR)[^aboutPR]

[^aboutPR]: 為你自己學Git - 關於PR https://gitbook.tw/chapters/github/pull-request

[^Git]: 这可能是你看过最通俗易懂的git介绍 https://www.youtube.com/watch?v=N6YQlPuAamw&t=119s

