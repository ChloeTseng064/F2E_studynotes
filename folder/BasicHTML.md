
## head
```html=
  <!-- 網站作者 -->
        <meta name="author" content="Chloe">
        
  <!-- 字元編碼 -->
        <meta charset="utf-8"/>
        <meta name="description" content="網站描述，搜尋引擎title下面灰色的一大串字，75字元內">
        
  <!-- 網站關鍵字，建議最多五組，搜尋引擎容易找到網站用 -->
        <meta name="keywords" content="作品集,前端,Front-end,beginners">
        
  <!-- RWD -->
        <meta name="viewport" content="width=device-width,initial-scale=1">
        
  <!-- 網站發佈語言 -->
        <meta name="language" content="tw">
        
  <!-- css 選擇器 -->
        <link rel="stylesheet" type="text/css" href="css-selector.css">
        
  <!-- 版面的寬度是裝置的寬度，縮放比是1.0 -->
          <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
          
```
![image](https://hackmd.io/_uploads/BytrNFhB6.png)


> 💡 如果包含多個段落或章節，建議使用 < section >分段，
如果只有一段文章，建議使用 < article > ，
文章需要排版則使用 < div > 調整。


> 💡有時候網站只出現 header 或 nav 。依情況調整。

## block & inline
> 常見區塊元素 (block)：div、ul li、p、h1...
>
> 常見行內元素 (inline)：span、a、input、img...
* block 有面積，可以設定寬跟高。
* inline 不換行，設定寬高無效，可以設定 padding 的左右值，上下值無效，無法被撐開。
* inline-block 同時擁有兩種 display 的特性，可以設定寬高，但也可以與其他元素水平並排，可設定 寬高 / margin / padding。

`:bulb:inline-block 會產生空白字元，所以要清除空白字元`

```html=
     ul{   
            font-size: 0;  /* 清除空白字元 */
        }
        li{
            display: inline-block; /* ← 這裡 */
            font-size: 16px; /* 重新設定 size */
            width: 100px;
            height: 100px;
            background-color: #aaa;
            margin: 10px;
            font-size: 30px;
            text-align: center;
            line-height: 100px;
        }
```
