# HTML - 前端小小班首頁

### HTML 規則

![](https://i.imgur.com/pZVuOsA.png =400x120)

![](https://i.imgur.com/rMSAXg7.png =600x70)

-   名詞
    -   標籤 Tag
        -   起始標籤 Opening tag，`<>` 裡面包著標籤名稱
        -   結束標籤 Closing tag，和開始標籤長一樣，只是前面有 `/`
    -   內容 Content
    -   元素 Element
        -   由起始標籤、結束標籤、內容所組成
    -   屬性 Attribute
        -   屬性名稱與值，用 `=`
        -   每一個屬性用`空白`隔開

### 基本的 HTML 文件的架構

```html
<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8" />
		<title>My test page</title>
		<link rel="shortcut icon" href="./favicon.ico" />
	</head>
	<body>
		<img src="./images/firefox.png" alt="My test image" />
	</body>
</html>
```

-   `<!DOCTYPE>`
    -   聲明表示檔案類型，並幫助瀏覽器能夠正確顯示網頁
    -   它只能出現一次，在頁面的頂部
    -   HTML5 `<!DOCTYPE html>`
-   `<html>`
    -   HTML 頁面的根元素
-   `<head>`

    -   裡面放的是你想涵括的重要資訊，但不會顯示於網頁瀏覽者眼前的
    -   例如顯示於搜尋結果的關鍵字、頁面說明、CSS 等等
        -   `<meta name="keywords" content="網頁關鍵字">`
        -   `<meta name="description" content="網頁簡短描述">`
        -   [分享文章到 Facebook 的 Meta 設定﹍縮圖+標題+摘要+作者資訊](https://www.wfublog.com/2015/04/facebook-meta-og-setting-thumbnail-title-description-author.html)
        -   `favicon.ico`
            -   書籤列的圖示
            -   瀏覽器會對每一個網站都請求 favicon
            -   ![](https://i.imgur.com/YQLFCCa.png)

-   `<body>`
    -   包含了所有會顯示於網頁瀏覽者眼前的內容
-   `<meta charset="utf-8">`
    -   指定了你的檔案使用 utf-8 這種字元編碼
-   `<title>`
    -   網頁標題
    -   ![](https://i.imgur.com/1e90PID.png)

### 標題

```html
<h1>My main title</h1>
<h2>My top level heading</h2>
<h3>My subheading</h3>
<h4>My sub-subheading</h4>
<h5>很少用到</h5>
<h6>這個也是</h6>
```

### 圖片

```html
<img src="./images/firefox-icon.png" alt="My test image" />
```

-   `src` 屬性
    -   檔案來源，可以放相對路徑或是絕對路徑
-   `alt` 屬性
    -   無法正確看到圖片時，代替說明文字
    -   通常發生：
        -   許多視能障礙的網頁瀏覽者，會使用「Screen Readers」這樣的工具，利用說明文字（alt text）來了解網頁要呈現的圖片內容。
        -   就是有些東西出錯了。例如，你誤植了圖片來源的路徑，你可能就會看到類似以下的文字：
            -   ![](https://i.imgur.com/dycwDh6.png)

### 超連結

```html
<a href="http://google.com/">這裡是谷歌</a>
```

-   `href` 屬性
    -   連結
    -   可以是相對路徑、絕對路徑
-   `target="_blank"`

### 表格

-   `<table>`
    -   把內容包起來
-   `<tr>`
    -   table row
-   `<th>`
    -   table header 標題
-   `<td>`
    -   table data
-   `rowspan` 屬性
    -   合併 row
-   `colspan` 屬性
    -   合併 column

```html
<table border="1">
	<tr>
		<th>Firstname</th>
		<th>Lastname</th>
		<th>Age</th>
	</tr>
	<tr>
		<td>奕迅</td>
		<td>陳</td>
		<td>30</td>
	</tr>
	<tr>
		<td>杰倫</td>
		<td>周</td>
		<td>20</td>
	</tr>
	<tr>
		<td>榮浩</td>
		<td>李</td>
		<td>10</td>
	</tr>
</table>
```

![](https://i.imgur.com/1vc6r2i.png)
