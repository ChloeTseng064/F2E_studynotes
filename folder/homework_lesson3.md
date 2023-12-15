# [Assignment] 靜態新聞網頁

`✍🏼 從風傳媒中挑一篇文章，試著排版文章及加入導覽列、旁邊的熱門文章等等區塊。`

## :question: Purpose
`熟悉基礎 HTML 及 CSS 語法。`


## :feet: Step
1. 分析整體頁面框架構成，利用 flex 去組成盒子。
    ![image](https://hackmd.io/_uploads/ByWtztBSa.png)
    
    <font color=#989898><small>最崩潰的就是大盒套小盒再套小小盒，一但自己亂掉尺寸就會開始亂跑。</small></font>

2. 學著套用 Google Fonts。
    ```html=
        <head>
            <link rel="preconnect" href="https://fonts.googleapis.com">
            <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
            <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;500;700&display=swap" rel="stylesheet">
        </head>
    ```
3. 元素命名要有意義，未來共編別人才能看得懂。
4. 上排導覽列插入圖片後的 css 設定。
	```css=
        #nav-container{
                display: flex;
                padding:8px 0px;
                border-bottom: 1px solid #CDCDCC; }
            .nav-left{
                display:flex;
                flex:none;
                justify-content: space-around;
                align-items: center;
                width: 90%; /* 使 .nav-left 佔據整個 .container 的寬度 */ }   
            .item{
                display: flex;
                justify-content: center;
                align-items:center;
                flex:none;
                padding:8px 4px;
                max-width: 100%;      
                    }
            .item-image img{
                width:100px;
                height: 25px;
                max-width: 100%;
                max-height: 100%;
                object-fit: contain;
                    }
    ```
    <font color="989898"><small>這邊最崩潰，第一次使用 flex 的用法，其實還不太了解每一段的意義所以變成在盲用。後來一條一條的詢問 ChatGPT 所代表的意義，試著有意識的去使用每一段 code。</small></font>
5. 按鍵及連結的 hover
    ```css=
    .sub-link{
        font-size:14px;
        padding:0 8px;
        display:flex;
        align-items: center;
        text-align: center;

        & a {
            color:black;
            font-weight:bold;
            text-decoration: none;
            display:block;
            }
        & a:hover{
            text-decoration: underline;
            color:black;
            }
        & a:visited{
            color:black;
            }

    ```
    <font color="989898"><small>這段是 ChatGPT 教我的，其實還不太理解 & 的意思，而且按鍵也還不會做。</small></font>
    
    ![image](https://hackmd.io/_uploads/rk9h2KHHT.png)
    <font color="989898"><small>之後要練習做成元件的方式，可惡用 Figma 做元件很容易呀。</small></font>
6. 本來以為最簡單的文字排版，其實要排的漂亮整齊也不容易，易讀的間距與行高很重要。
7. 右方熱門文章其實做很快 (相較上面的導覽)，但屬於較簡單的卡片，之後也要試著練習複雜的卡片。


### 👉🏼 [程式碼及頁面展示](https://codepen.io/ChloeTseng1026/pen/ExrBNry) 
