# Day 2 - 第一个HTML页面 Hello World!
今天，我的任务并不多，是编写第一个HTML页面  
一个展示Hello World!的页面  
首先需要了解HTML是一个标签语言，每一个标签使用<>包括起来。如`<h1>`就是一个标签  
在标准情况下，有头即有尾例如`<div></div>`
下面展示一个最简单的HTML代码  
```
<html>
    <body>
        <h1>Hello World!</h1>
    </body>
</html>
```
将这段代码，保存在本地仓库的/html/day2/index.html中,使用浏览器访问[http://localhost/day2/index.html](http://localhost/day2/index.html)

# Option 其他标签
HTML文档还会有很多很多标签，例如  
```
<a>超链接
<input />输入
<textarea />输入
<font>文字
<p>段落
<div>块
……等等
```
我们可以在[w3school](https://www.w3school.com.cn/html/html_elements.asp)中学习到更多

# Option 网页标题  
通常我们的网页打开后，窗口上方都会有个标签，显示我们网页的名字，而这个名字也是通过代码实现的  
```
<html>
    <head>
        <title>第一段代码</title>
    </head>
    <body>
        <h1>Hello World!</h1>
    </body>
</html>
```
在HTML的头部`<head></head>`中添加`<title></title>`来标明你的网站的标题  
在上一步结束之后使用浏览器打开，你会发现，你添加的中文字体，可能变成了乱码。  
这时候就要对网页文档的文字编码格式进行指定，我们使用如下标签进行指定  
`<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />`  
在Mac中编辑，默认的字符编码是`utf-8`，在Windows下编辑，可能会使用`gbk`或者`gb2312`  
我们可以通过对`charset`进行修改，进行多次尝试得到文档的编码  
本人使用VSCode进行编辑，右下角可以看到当前文档的字符编码，本仓库编辑的文档都是使用UTF8  

