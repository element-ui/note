# HTML 标签

vsc编辑器，用!可以快速生成html骨架

JS-CSS-HTML Formatter
每次保存，都会自动格式化js css和html代码

Auto Rename Tag
自动重命名配对的HTML/XML标签

CSS Peek
追踪至样式



# 1. HTML 表格

```html
<!--border的值表示表格边框的大小-->
<!-- cellpadding 表示单元格的边距 -->
<!-- cellspacing 表示单元格的间距，就是单元格之间的间距 -->
<!-- bgcolor="red" 设置表格或单元格背景颜色 -->
<!-- background="" 设置表格或单元格背景图片  -->
<!-- align="left/right" 设置文本的排列 -->
<table border="9" cellpadding="20" cellspacing="5" bgcolor="#606080" width="400px" height="400px">
    <!-- caption 表示标题 -->
    <caption>我的标题</caption>
    <tr>
        <!-- th表示表头 -->
        <th>序号</th>
        <!-- colspan 表示合并列 -->
        <th colspan="2">名称</th>
    </tr>
    <tr>
        <!--tr表示行-->
        <!--td指(table data)表示列-->
        <td>1</td>
        <td colspan="2">spring</td>
    </tr>
    <tr>
        <!-- rowspan 表示合并行 -->
        <td rowspan="2">2</td>
        <td>spring</td>
        <td>html</td>
    </tr>
    <tr>
        <td>spring</td>
        <td>html</td>
    </tr>
</table>
```

<img src="html%E6%A0%87%E7%AD%BE.assets/image-20220317021259386.png" alt="image-20220317021259386" style="zoom:50%;" />



# 2. HTML 列表

```html
<!-- 无序列表 -->
<!-- type 可以设置无序列表前面的符号 -->
<ul type="disc">
    <li>苹果</li>
    <li>香蕉</li>
    <li>柠檬</li>
    <li>桔子</li>
</ul>  

<ul type="circle">
    <li>苹果</li>
    <li>香蕉</li>
    <li>柠檬</li>
    <li>桔子</li>
</ul>  

<!-- 有序列表 -->
<!-- type 可以设置有序列表前面的符号 -->
<ol type="A">
    <li>苹果</li>
    <li>香蕉</li>
    <li>柠檬</li>
    <li>桔子</li>
</ol> 

<!-- 自定义列表 -->
<dl>
    <dt>水果</dt>
    <dd>苹果</dd>
    <dd>香蕉</dd>
</dl> 
```

<img src="html%E6%A0%87%E7%AD%BE.assets/image-20220317022334577.png" alt="image-20220317022334577" style="zoom:67%;" />



# 3. HTML 块

<img src="html%E6%A0%87%E7%AD%BE.assets/image-20220317102027601.png" alt="image-20220317102027601" style="zoom: 67%;" />



# 4. HTML 内联框架（iframe）

```html
<!-- 可以设置宽度和高度 -->
<!-- name 可以通过target绑定的值，通过iframe标签中的name属性来接收 -->
<iframe src="/example/html/demo_iframe.html" name="iframe_a" width="300px" height="200px"></iframe>
<p><a href="http://www.w3school.com.cn" target="iframe_a">W3School.com.cn</a></p>
<p><b>注释：</b>由于链接的目标匹配 iframe 的名称，所以链接会在 iframe 中打开。</p>
```

<img src="html%E6%A0%87%E7%AD%BE.assets/image-20220317103247965.png" alt="image-20220317103247965" style="zoom:67%;" />



# 5. HTML script

HTML <noscript> 标签定义了替代内容，这些内容将显示给在浏览器中禁用了脚本或浏览器不支持脚本的用户：

实例

```html
<script>
document.getElementById("demo").innerHTML = "Hello JavaScript!";
</script>
<!-- 浏览器不支持script脚本的话，会显示noscript标签中的内容 -->
<noscript>抱歉，您的浏览器不支持 JavaScript！</noscript>
```



# 6. HTML a

```html
<!-- 将在新窗口中加载，因为 target 属性被设置为 "_blank"。 -->
<a href="http://www.w3school.com.cn" target="_blank">这个连接</a> 
<!-- 也将在新窗口中加载，即使没有 target 属性。 -->
<a href="http://www.w3school.com.cn">这个连接</a> 
```



# 7. HTML 头

### 7.1 base标签

base 标签为页面上的所有链接规定默认地址或默认目标（target）：

```html
<head>
<base href="http://www.w3school.com.cn/images/" />
<base target="_blank" />
</head>

<!-- href 不写则默认base标签中的默认地址，和跳转方式 -->
<!-- 点击跳转会跳转到 http://www.w3school.com.cn/images/中-->
<a href="">跳转</a>
```



### 7.2 meta标签

meta 元数据（metadata）是关于数据的信息

meta 标签提供关于 HTML 文档的元数据。元数据不会显示在页面上，但是对于机器是可读的

典型的情况是，meta 元素被用于规定页面的描述、关键词、文档的作者、最后修改时间以及其他元数据

```html
<!-- 下面的 meta 元素定义页面的关键词： -->
<meta name="keywords" content="HTML, CSS, XML" />
```



# 8. HTML 布局

```html
<details>
    <summary>小陈</summary>
    <p>陈小胖</p>
</details>
```

![image-20220320220514743](html%E6%A0%87%E7%AD%BE.assets/image-20220320220514743.png)



# 9. HTML 语义

HTML5 <figure> 和 <figcaption> 元素

在书籍和报纸中，与图片搭配的标题很常见

标题（caption）的作用是为图片添加可见的解释

通过 HTML5，图片和标题能够被组合在 *<figure>* 元素中：

实例

```html
<figure>
   <img src="pic_mountain.jpg" alt="The Pulpit Rock" width="304" height="228">
   <figcaption>Fig1. - The Pulpit Pock, Norway.</figcaption>
</figure> 
```

![image-20220317110912203](html%E6%A0%87%E7%AD%BE.assets/image-20220317110912203.png)



# 10. HTML 字符实体

<img src="html%E6%A0%87%E7%AD%BE.assets/image-20220317183244087.png" alt="image-20220317183244087" style="zoom:50%;" />



# 11. HTML URL

```html
scheme://host.domain:port/path/filename
```

解释：

- scheme - 定义因特网服务的类型。最常见的类型是 http
- host - 定义域主机（http 的默认主机是 www）
- domain - 定义因特网域名，比如 w3school.com.cn
- :port - 定义主机上的端口号（http 的默认端口号是 80）
- path - 定义服务器上的路径（如果省略，则文档必须位于网站的根目录中）
- filename - 定义文档/资源的名称

**编者注：**URL 的英文全称是 Uniform Resource Locator，中文也译为“**统一资源定位符**”

以下是其中一些最流行的 scheme：

| Scheme | 访问               | 用于...                             |
| :----- | :----------------- | :---------------------------------- |
| http   | 超文本传输协议     | 以 http:// 开头的普通网页。不加密。 |
| https  | 安全超文本传输协议 | 安全网页。加密所有信息交换。        |
| ftp    | 文件传输协议       | 用于将文件下载或上传至网站。        |
| file   |                    | 您计算机上的文件。                  |



# 12. HTML 框架

框架：就是将几个html页面整合在一起显示出来

```html
<!-- 假如一个框架有可见边框，用户可以拖动边框来改变它的大小。为了避免这种情况发生，可以在 <frame> 标签中加入：noresize="noresize"。 -->
<frameset rows="50%,50%">
    <frame src="/example/html/frame_a.html" noresize="noresize">
    <frameset cols="25%,75%">
        <frame src="/example/html/frame_b.html">
        <frame src="/example/html/frame_c.html">
    </frameset>
</frameset>

<noframes>
    <body>您的浏览器无法处理框架！</body>
</noframes>
```

<img src="html%E6%A0%87%E7%AD%BE.assets/image-20220318142510883.png" alt="image-20220318142510883" style="zoom:50%;" />



# 13. HTML XHTML

### 13.1 什么是 XHTML？

```
- XHTML 指的是可扩展超文本标记语言
- XHTML 与 HTML 4.01 几乎是相同的
- XHTML 是更严格更纯净的 HTML 版本
- XHTML 是以 XML 应用的方式定义的 HTML
- XHTML 是 [2001 年 1 月](https://www.w3school.com.cn/w3c/w3c_xhtml.asp)发布的 W3C 推荐标准
- XHTML 得到所有主流浏览器的支持
```

### 13.2 如何从 HTML 转换到 XHTML

```
1. 向每张页面的第一行添加 XHTML <!DOCTYPE>
2. 向每张页面的 html 元素添加 xmlns 属性
3. 把所有元素名改为小写
4. 关闭所有空元素
5. 把所有属性名改为小写
6. 为所有属性值加引号
```

### 13.3 XHTML 元素 - 语法规则

```html
<!-- XHTML 元素必须正确嵌套 --> 
错误：<b><i>This text is bold and italic</b></i>
正确：<b><i>This text is bold and italic</i></b>

<!-- XHTML 元素必须始终关闭 -->
错误：<p>This is a paragraph		<br>	<hr>
正确：<p>This is a paragraph</p>	<br/>	<hr/>

<!-- XHTML 元素必须小写 -->
错误：
    <BODY>
    <p>This is a paragraph</p>
    </BODY>
正确：
    <body>
    <p>This is a paragraph</p>
    </body>

<!-- XHTML 文档必须有一个根元素 -->
<html></html>
```

### 13.4 XHTML 属性 - 语法规则

```html
<!-- XHTML 属性必须使用小写 -->
错误：<table WIDTH="100%">
正确：<table width=100%>
    
<!-- XHTML 属性值必须用引号包围 -->
错误：<table width=100%>
正确：<table width="100%">

<!-- XHTML 属性最小化也是禁止的 -->
错误：
    <input checked>
    <input readonly>
    <input disabled>
    <option selected>
正确：
    <input checked="checked" />
    <input readonly="readonly" />
    <input disabled="disabled" />
    <option selected="selected" />
```



# 14. HTML 表单

### 14.1 input元素

*<input>* 元素是最重要的*表单元素*

<input> 元素有很多形态，根据不同的 *type* 属性

这是本章中使用的类型：

| 类型     | 描述                                 |
| :------- | :----------------------------------- |
| text     | 定义常规文本输入                     |
| radio    | 定义单选按钮输入（选择多个选择之一） |
| submit   | 定义提交按钮（提交表单）             |
| password | 定义密码                             |
| checkbox | 定义复选框                           |
| button   | 定义按钮                             |
| range    | 定义进度条                           |



##### 14.1.1 select 元素（下拉列表）

*<select>* 元素定义*下拉列表*：

您能够通过添加 selected 属性来定义预定义选项。

实例：

```html
<select name="cars">
  <optgroup label="Swedish Cars">
    <option>Volvo</option>
    <option value="saab">Saab</option>
  </optgroup>
  <optgroup label="German Cars">
    <option value="mercedes">Mercedes</option>
    <option value="audi">Audi</option>
  </optgroup>
</select>
```

![image-20220320220643724](html%E6%A0%87%E7%AD%BE.assets/image-20220320220643724.png)



##### 14.1.2 textarea 元素

*<textarea>* 元素定义多行输入字段（*文本域*）：

实例:

```html
<textarea name="message" rows="10" cols="30">
    The cat was playing in the garden.
</textarea>
```



##### 14.1.3 button 元素

*<button>* 元素定义可点击的*按钮*：

实例：

```html
<button type="button" onclick="alert('Hello World!')">Click Me!</button>
```



##### 14.1..4 HTML5 datalist 元素

*<datalist>* 元素为 <input> 元素规定预定义选项列表。

用户会在他们输入数据时看到预定义选项的下拉列表。

<input> 元素的 *list* 属性必须引用 <datalist> 元素的 *id* 属性。

实例:

通过 <datalist> 设置预定义值的 <input> 元素：

```html
<form action="action_page.php">
    <input list="browsers">
    <datalist id="browsers">
        <option value="Internet Explorer">
        <option value="Firefox">
        <option value="Chrome">
        <option value="Opera">
        <option value="Safari">
    </datalist> 
</form>
```

<img src="html%E6%A0%87%E7%AD%BE.assets/image-20220318152547883.png" alt="image-20220318152547883" style="zoom:50%;" />



##### 14.1.5 输入限制

这里列出了一些常用的输入限制（其中一些是 HTML5 中新增的）：

| 属性      | 描述                               |
| :-------- | :--------------------------------- |
| disabled  | 规定输入字段应该被禁用。           |
| max       | 规定输入字段的最大值。             |
| maxlength | 规定输入字段的最大字符数。         |
| min       | 规定输入字段的最小值。             |
| pattern   | 规定通过其检查输入值的正则表达式。 |
| readonly  | 规定输入字段为只读（无法修改）。   |
| required  | 规定输入字段是必需的（必需填写）。 |
| size      | 规定输入字段的宽度（以字符计）。   |
| step      | 规定输入字段的合法数字间隔。       |
| value     | 规定输入字段的默认值。             |

**输入类型：date**

*<input type="date">* 用于应该包含日期的输入字段。

根据浏览器支持，日期选择器会出现输入字段中。

实例：

```html
<form>
  Birthday:
  <input type="date" name="bday">
</form>
```

<img src="html%E6%A0%87%E7%AD%BE.assets/image-20220318153658824.png" alt="image-20220318153658824" style="zoom:50%;" />



**readonly 属性**

*readonly* 属性规定输入字段为只读（不能修改）

readonly 属性不需要值。它等同于 readonly="readonly"



##### 14.1.6 autofocus 属性

autofocus 属性是布尔属性。

如果设置，则规定当页面加载时 <input> 元素应该自动获得焦点。



##### 14.1.7 formaction 属性

formaction 属性规定当提交表单时处理该输入控件的文件的 URL。

formaction 属性覆盖 <form> 元素的 action 属性。

formaction 属性适用于 type="submit" 以及 type="image"。

实例：

拥有两个两个提交按钮并对于不同动作的 HTML 表单：

```html
<form action="action_page.php">
    First name: <input type="text" name="fname"><br>
    Last name: <input type="text" name="lname"><br>
    <input type="submit" value="Submit"><br>
    <input type="submit" formaction="demo_admin.asp" value="Submit as admin">
</form> 
```

| 属性            | 描述                                                         |
| --------------- | ------------------------------------------------------------ |
| height 和 width | height 和 width 属性规定 <input> 元素的高度和宽度。height 和 width 属性仅用于 <input type="image">。 |
| placeholder     | 该提示会在用户输入值之前显示在输入字段中                     |
| formmethod      | 向 action URL 发送表单数据（form-data）的 HTTP 方法          |
| formnovalidate  | 规定在提交表单时不对 <input> 元素进行验证                    |
| formtarget      | 规定的名称或关键词指示提交表单后在何处显示接收到的响应，formtarget="_blank" |



##### 14.1.8 multiple 属性

multiple 属性是布尔属性。

如果设置，则规定允许用户在 <input> 元素中输入一个以上的值。

multiple 属性适用于以下输入类型：email 和 file。

实例：

接受多个值的文件上传字段：

```html
Select images: <input type="file" name="img" multiple>
```

<img src="html%E6%A0%87%E7%AD%BE.assets/image-20220318160042738.png" alt="image-20220318160042738" style="zoom:67%;" />



##### 14.1.9 Name 属性

如果要正确地被提交，每个输入字段**必须**设置一个 name 属性

本例只会提交 "Last name" 输入字段：

实例:

```html
<form action="action_page.php">
    First name:<br>
    <input type="text" value="Mickey">
    <br>
    Last name:<br>
    <input type="text" name="lastname" value="Mouse">
    <br><br>
    <input type="submit" value="Submit">
</form> 
```



##### 14.1.10 用 fieldset 组合表单数据

*<fieldset>* 元素组合表单中的相关数据

*<legend>* 元素为 <fieldset> 元素定义标题

```html
<form action="/demo/demo_form.asp">
    <fieldset>
        <legend>Personal information:</legend>
        First name:<br>
        <input type="text" name="firstname" value="Mickey">
        <br>
        Last name:<br>
        <input type="text" name="lastname" value="Mouse">
        <br><br>
        <input type="submit" value="Submit">
    </fieldset>
</form>
```

<img src="html%E6%A0%87%E7%AD%BE.assets/image-20220318150208020.png" alt="image-20220318150208020" style="zoom:50%;" />



##### 14.1.11 output

```html
<form oninput="x.value=parseInt(a.value)+parseInt(b.value)">0
<input type="range" id="a" value="50">100
+<input type="number" id="b" value="50">
=<output name="x" for="a b"></output>
</form>
```

<img src="html%E6%A0%87%E7%AD%BE.assets/image-20220320222004357.png" alt="image-20220320222004357" style="zoom:50%;" />



### 14.2 Form 属性

HTML <form> 元素，已设置所有可能的属性，是这样的：

实例：

```html
<form action="action_page.php" method="GET" target="_blank" accept-charset="UTF-8"
ectype="application/x-www-form-urlencoded" autocomplete="off" novalidate></form> 
```

下面是 <form> 属性的列表：

| 属性           | 描述                                                     |
| :------------- | :------------------------------------------------------- |
| accept-charset | 规定在被提交表单中使用的字符集（默认：页面字符集）       |
| action         | 规定向何处提交表单的地址（URL）（提交页面）              |
| autocomplete   | 规定浏览器应该自动完成表单（默认：开启）                 |
| enctype        | 规定被提交数据的编码（默认：url-encoded）                |
| method         | 规定在提交表单时所用的 HTTP 方法（默认：GET）            |
| name           | 规定识别表单的名称（对于 DOM 使用：document.forms.name） |
| novalidate     | 规定浏览器不验证表单                                     |
| target         | 规定 action 属性中地址的目标（默认：_self）              |



##### 14.2.1 Target 属性

`target` 属性规定提交表单后在何处显示响应

`target` 属性可设置以下值之一：

| 值        | 描述                         |
| :-------- | :--------------------------- |
| _blank    | 响应显示在新窗口或选项卡中   |
| _self     | 响应显示在当前窗口中         |
| _parent   | 响应显示在父框架中           |
| _top      | 响应显示在窗口的整个 body 中 |
| framename | 响应显示在命名的 iframe 中   |

注意：默认值为 `_self`，这意味着响应将在当前窗口中打开



##### 14.2.2 Novalidate 属性

`novalidate` 属性是一个布尔属性。

如果已设置，它规定提交时不应验证表单数据。

实例：

未设置 novalidate 属性的表单：

```html
<form action="/action_page.php" novalidate>
```



##### 14.2.3 Autocomplete 属性

`autocomplete` 属性规定表单是否应打开自动完成功能。

启用自动完成功能后，浏览器会根据用户之前输入的值自动填写值。

实例:

启用自动填写的表单：

```html
<form action="/action_page.php" autocomplete="on">
```



##### 14.2.4 form 属性

规定 input 元素所属的一个或多个表单。

**提示：**如需引用一个以上的表单，请使用空格分隔的表单 id 列表。

实例:

输入字段位于 HTML 表单之外（但仍属表单）：

```html
<form action="action_page.php" id="form1">
   First name: <input type="text" name="fname"><br>
   <input type="submit" value="Submit">
</form>

 Last name: <input type="text" name="lname" form="form1">
```



##### 14.2.5 Action 属性

*action 属性*定义在提交表单时执行的动作

向服务器提交表单的通常做法是使用提交按钮

通常，表单会被提交到 web 服务器上的网页

在上面的例子中，指定了某个服务器脚本来处理被提交表单：

```html
<form action="action_page.php">
```

如果省略 action 属性，则 action 会被设置为当前页面



##### 14.2.6 Method 属性

*method 属性*规定在提交表单时所用的 HTTP 方法（*GET* 或 *POST*）：

```html
<form action="action_page.php" method="GET">
```

或：

```html
<form action="action_page.php" method="POST">
```



# 15. 获取坐标

```html
<script type="text/javascript">
    function move(e){
        x = e.clientX
        y = e.clientY
        let c = document.getElementById("clear")
        c.innerHTML = "坐标：("+x+","+y+")"
    }
    function leave(){
        let c = document.getElementById("clear")
        c.innerHTML = ""
    }
</script>
<p>将鼠标移入盒子内可以显示坐标的位置</p>
<div class="box" onmousemove="move(event)"></div>
<div id="clear" onmouseleave="leave()"></div>
```



# 16. HTML 媒体

### 16.1 HTML 对象

##### 16.1.1 object元素

object标签将插件或者是网页或者是图片等等嵌入到网页中

```html
<!-- 有结束标签 -->
<object width="100%" height="500px" data="snippet.html"></object>
<object data="audi.jpeg"></object>
```

##### 16.1.2embed元素

embed标签将插件或者是网页或者是图片等等嵌入到网页中

```html
<!-- 没有结束标签 -->
<embed width="100%" height="500px" src="snippet.html">
<embed src="audi.jpeg">
```



### 16.2 HTML 音频

##### 16.2.1 使用 HTML5 audio元素

audio元素是一个 HTML5 元素，在 HTML 4 中是非法的，但在所有浏览器中都有效。实例

```html
<!-- controls 属性一定要写上，不写就显示不出音频来 
	 autoplay 属性是自动播放
-->
<audio controls="controls" autoplay>
    <!-- 这是MP3格式 -->
  <source src="song.mp3" type="audio/mp3" />
    <!-- 这是ogg格式 为了使这段音频在 Firefox 和 Opera 中同样有效，添加了一个 ogg 类型的文件。如果失败，会显示错误消息。-->
  <source src="song.ogg" type="audio/ogg" />
</audio>
```

<img src="html%E6%A0%87%E7%AD%BE.assets/image-20220318184912141.png" alt="image-20220318184912141" style="zoom:50%;" />



##### 16.2.2 向网站添加音频的最简单方法

向网页添加音频的最简单的方法是什么？

雅虎的媒体播放器绝对算其中之一。

使用雅虎媒体播放器是一个不同的途径。您只需简单地让雅虎来完成歌曲播放的工作就好了。

它能播放 mp3 以及一系列其他格式。通过一行简单的代码，您就可以把它添加到网页中，轻松地将 HTML 页面转变为专业的播放列表。

使用雅虎播放器是免费的。如需使用它，您需要把这段 JavaScript 插入网页底部：

```html
<script type="text/javascript" src="http://mediaplayer.yahoo.com/js"></script>
```

然后只需简单地把 MP3 文件链接到您的 HTML 中，JavaScript 会自动地为每首歌创建播放按钮：

```html
<a href="song1.mp3">Play Song 1</a>
<a href="song2.mp3">Play Song 2</a>
```



### 16.3 HTML 视频

##### 16.3.1 使用video标签

video是 HTML 5 中的新标签。

video标签的作用是在 HTML 页面中嵌入视频元素。

以下 HTML 片段会显示一段嵌入网页的 ogg、mp4 或 webm 格式的视频：

```html
<video width="320" height="240" controls="controls">
    <source src="movie.mp4" type="video/mp4" />
    <source src="movie.ogg" type="video/ogg" />
    <source src="movie.webm" type="video/webm" />
</video>
```



##### 16.3.2 最好的 HTML 解决方法

HTML 5 + <object> + <embed>

```html
<!-- 当浏览器无法播放video设定的格式，，会退回到embed标签中设定的格式，如果再无法播放就会返回报错 -->
<!-- autoplay="1" 可以设置自动播放 muted="1" 可以设置静音播放 -->
<!-- loop 可以设置无限播放视频 -->
<video width="320" height="240" controls="controls" loop="1" muted="1">
    <source src="movie.mp4" type="video/mp4" />
    <source src="movie.ogg" type="video/ogg" />
    <source src="movie.webm" type="video/webm" />
    <object data="movie.mp4" width="320" height="240">
        <embed src="movie.swf" width="320" height="240" />
    </object>
</video>
```



##### 16.3.3 loop属性

添加 `loop=1` 会让您的视频永远循环。

值 0（默认）：视频将播放一次。

值 1：视频将循环（永远）。



##### 16.3.4muted属性

muted="1"可以设置静音播放视频



##### 16.3.5 controls属性

可以显示出播放/音量等组件

<img src="html%E6%A0%87%E7%AD%BE.assets/image-20220319003704509.png" alt="image-20220319003704509" style="zoom:50%;" />



# 17. HTML 5

### 17.1 什么是HTML5？

HTML5 是最新的 HTML 标准。

HTML5 是专门为承载丰富的 web 内容而设计的，并且无需额外插件。

HTML5 拥有新的语义、图形以及多媒体元素。

HTML5 提供的新元素和新的 API 简化了 web 应用程序的搭建。

HTML5 是跨平台的，被设计为在不同类型的硬件（PC、平板、手机、电视机等等）之上运行。

**注释：**在下面的章节中，您将学到如何“帮助”老版本的浏览器处理 HTML5。



##### 17.1.1 HTML5 - 新的属性语法

HTML5 标准允许 4 中不同的属性语法。

本例演示在 <input> 标签中使用的不同语法：

| 类型          | 示例                                          |
| :------------ | :-------------------------------------------- |
| Empty         | <input type="text" value="John Doe" disabled> |
| Unquoted      | <input type="text" value=John Doe>            |
| Double-quoted | <input type="text" value="John Doe">          |
| Single-quoted | <input type="text" value='John Doe'>          |

在 HTML5 标准中，根据对属性的需求，可能会用到所有 4 种语法。



##### 17.1.2 HTML5 - 新特性

HTML5 的一些最有趣的新特性：

- 新的语义元素，比如 <header>（头部）, <footer>（底部）, <article>（段落部分）, and <section>（内容部分）。
- 新的表单控件，比如数字、日期、时间、日历和滑块。
- 强大的图像支持（借由 <canvas> 和 <svg>）
- 强大的多媒体支持（借由 <video> 和 <audio>）
- 强大的新 API，比如用本地存储取代 cookie。



##### 17.1.3 HTML5 - 被删元素

以下 HTML 4.01 元素已从 HTML5 中删除：

```html
- <acronym>
- <applet>
- <basefont>
- <big>
- <center>
- <dir>
- <font>
- <frame>
- <frameset>
- <noframes>
- <strike>
- <tt>
```



### 17.2 HTML5 支持

创建新标签

```html
<!-- 创建新标签用到的script标签必须放到head标签中  -->
<script>document.createElement("myHero")</script>
<myHero>My First Hero</myHero>
```



### 17.3 HTML5 元素

##### 17.3.1 新的语义/结构元素

HTML5 提供的新元素可以构建更好的文档结构：

| 标签         | 描述                                                 |
| :----------- | :--------------------------------------------------- |
| <article>    | 定义文档内的文章。                                   |
| <aside>      | 定义页面内容之外的内容。                             |
| <bdi>        | 定义与其他文本不同的文本方向。                       |
| <details>    | 定义用户可查看或隐藏的额外细节。                     |
| <dialog>     | 定义对话框或窗口。                                   |
| <figcaption> | 定义 <figure> 元素的标题。                           |
| <figure>     | 定义自包含内容，比如图示、图表、照片、代码清单等等。 |
| <footer>     | 定义文档或节的页脚。                                 |
| <header>     | 定义文档或节的页眉。                                 |
| <main>       | 定义文档的主内容。                                   |
| <mark>       | 定义重要或强调的内容。                               |
| <menuitem>   | 定义用户能够从弹出菜单调用的命令/菜单项目。          |
| <meter>      | 定义已知范围（尺度）内的标量测量。                   |
| <nav>        | 定义文档内的导航链接。                               |
| <progress>   | 定义任务进度。                                       |
| <rp>         | 定义在不支持 ruby 注释的浏览器中显示什么。           |
| <rt>         | 定义关于字符的解释/发音（用于东亚字体）。            |
| <ruby>       | 定义 ruby 注释（用于东亚字体）。                     |
| <section>    | 定义文档中的节。                                     |
| <summary>    | 定义 <details> 元素的可见标题。                      |
| <time>       | 定义日期/时间。                                      |
| <wbr>        | 定义可能的折行（line-break）。                       |

##### 17.3.2 新的表单元素

| 标签       | 描述                             |
| :--------- | :------------------------------- |
| <datalist> | 定义输入控件的预定义选项。       |
| <keygen>   | 定义键对生成器字段（用于表单）。 |
| <output>   | 定义计算结果。                   |

##### 17.3.3 新的输入类型

| 新的输入类型                                                 | 新的输入属性                                                 |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| color/datedatetime/datetime-local/email/month/number/range/search/tel/time/url/week | autocomplete/autofocus/form/formaction/formenctype/formmethod/formnovalidate/formtargetheight/ 和 widthlistmin 和 max/multiple/pattern (regexp)placeholder/required/step |

##### 17.3.4 HTML5 - 新的属性语法

HTML5 允许四种不同的属性语法。

该例演示 <input> 标签中使用的不同语法：

| 标签          | 描述                                          |
| :------------ | :-------------------------------------------- |
| Empty         | <input type="text" value="John Doe" disabled> |
| Unquoted      | <input type="text" value=John>                |
| Double-quoted | <input type="text" value="John Doe">          |
| Single-quoted | <input type="text" value='John Doe'>          |

##### 17.3.5 HTML5 图像

| 标签     | 描述                             |
| :------- | :------------------------------- |
| <canvas> | 定义使用 JavaScript 的图像绘制。 |
| <svg>    | 定义使用 SVG 的图像绘制。        |

##### 17.3.6 新的媒介元素

| 标签     | 描述                                 |
| :------- | :----------------------------------- |
| <audio>  | 定义声音或音乐内容。                 |
| <embed>  | 定义外部应用程序的容器（比如插件）。 |
| <source> | 定义 <video> 和 <audio> 的来源。     |
| <track>  | 定义 <video> 和 <audio> 的轨道。     |
| <video>  | 定义视频或影片内容。                 |



### 17.4 HTML 迁移

##### 17.7.1从 HTML4 迁移至 HTML5

本章讲解如何从一张典型的 HTML4 页面迁移至典型的 HTML5。

本章演示如何把一张已有的 HTML4 页面转换为 HTML5 页面，在不破坏如何原始内容和结构的情况下。

**注释：**您可以使用相同的技巧从 HTML4 以及 XHTML 迁移至 HTML5。

|    典型的 HTML4    | 典型的 HTML5 |
| :----------------: | :----------: |
| <div id="header">  |   <header>   |
|  <div id="menu">   |    <nav>     |
| <div id="content"> |  <section>   |
|  <div id="post">   |  <article>   |
| <div id="footer">  |   <footer>   |



##### 17.7.2 去除head标签

HTML5：在html页面中不写head标签也不影响页面的效果



# 18. HTML5 API

### 18.1 地理位置

##### 18.1.1 getCurrentPosition() 

请使用 getCurrentPosition() 方法来获得用户的位置。

```html
<script>
    var x=document.getElementById("demo");
    function getLocation(){
        if (navigator.geolocation){
            navigator.geolocation.getCurrentPosition(showPosition);
        }
        else{x.innerHTML="Geolocation is not supported by this browser.";}
    }
    function showPosition(position){
        x.innerHTML="Latitude: " + position.coords.latitude +
            "<br />Longitude: " + position.coords.longitude;
    }
</script>
```



##### 18.1.2 处理错误和拒绝

getCurrentPosition() 方法的第二个参数用于处理错误。它规定当获取用户位置失败时运行的函数：

```js
function showError(error){
    switch(error.code){
        case error.PERMISSION_DENIED:
            x.innerHTML="User denied the request for Geolocation."
            break;
        case error.POSITION_UNAVAILABLE:
            x.innerHTML="Location information is unavailable."
            break;
        case error.TIMEOUT:
            x.innerHTML="The request to get user location timed out."
            break;
        case error.UNKNOWN_ERROR:
            x.innerHTML="An unknown error occurred."
            break;
    }
}
```



##### 18.1.3 getCurrentPosition() - 返回数据

若成功，则 getCurrentPosition() 方法返回对象。始终会返回 latitude、longitude 以及 accuracy 属性。如果可用，则会返回其他下面的属性。

| 属性                    | 描述                   |
| :---------------------- | :--------------------- |
| coords.latitude         | 十进制数的纬度         |
| coords.longitude        | 十进制数的经度         |
| coords.accuracy         | 位置精度               |
| coords.altitude         | 海拔，海平面以上以米计 |
| coords.altitudeAccuracy | 位置的海拔精度         |
| coords.heading          | 方向，从正北开始以度计 |
| coords.speed            | 速度，以米/每秒计      |
| timestamp               | 响应的日期/时间        |



##### 18.1.4 watchPosition()

返回用户的当前位置，并继续返回用户移动时的更新位置（就像汽车上的 GPS）。

clearWatch() - 停止 watchPosition() 方法

下面的例子展示 watchPosition() 方法。您需要一台精确的 GPS 设备来测试该例（比如 iPhone）：

实例：

```html
<script>
    var x=document.getElementById("demo");
    function getLocation(){
        if (navigator.geolocation){
            navigator.geolocation.watchPosition(showPosition);
        }
        else{x.innerHTML="Geolocation is not supported by this browser.";
        }
    }
    function showPosition(position){
        x.innerHTML="Latitude: " + position.coords.latitude +
            "<br />Longitude: " + position.coords.longitude;
    }
</script>
```



### 18.2 HTML5 拖放

```html
<!DOCTYPE HTML>
<html>
    <head>
        <style type="text/css">
            #div1 {
                width:198px; 
                height:66px;
                padding:10px;
                border:1px solid #aaaaaa;
            }
        </style>
        <script type="text/javascript">
            function drag(ev){
                //设置数据类型和确定物体的id
                //ev.dataTransfer.setData(数据类型，被拖动物体对应的id)
                ev.dataTransfer.setData("Text",ev.target.id);
            }
            
            function allowDrop(ev){
                //默认数据和元素是不被拖物放置的，通过preventDefault()可阻止默认机制
                ev.preventDefault();
            }

            function drop(ev){
                ev.preventDefault();
                var data=ev.dataTransfer.getData("Text");	
                //将被拖物放置指定的位置
                ev.target.appendChild(document.getElementById(data));
            }
        </script>
    </head>
    <body>
        <p>请把 W3School 的图片拖放到矩形中：</p>
        <!-- ondragover="allowDrop(event)" 有拖物放入时触发 -->
        <div id="div1" ondrop="drop(event)" ondragover="allowDrop(event)"></div>
        <br />
        <!-- draggable="true" 设置可拖动 -->
        <!-- ondragstart="drag(event) 设置被拖动是触发事件,规定拖动什么数据-->
        <img id="drag1" src="D:\picture\2.png" draggable="true" ondragstart="drag(event)" style="width:190px; height:60px;"/>
    </body>
</html>
```

<img src="html%E6%A0%87%E7%AD%BE.assets/image-20220320005120900.png" alt="image-20220320005120900" style="zoom: 80%;" />	<img src="html%E6%A0%87%E7%AD%BE.assets/image-20220320005145985.png" alt="image-20220320005145985" style="zoom: 80%;" />



##### 18.2.1 把元素设置为可拖放

首先：为了把一个元素设置为可拖放，请把 draggable 属性设置为 true：

```html
<img draggable="true">
```



##### 18.2.2 拖放的内容 - ondragstart 和 setData()

然后，规定当元素被拖动时发生的事情。

在上面的例子中，ondragstart 属性调用了一个 drag(event) 函数，规定拖动什么数据。

dataTransfer.setData() 方法设置被拖动数据的数据类型和值：

```js
function drag(ev) {
    ev.dataTransfer.setData("text", ev.target.id);
}
```

在本例中，数据类型是 "text"，而值是这个可拖动元素的 id ("drag1")。



##### 18.2.3 拖到何处 - ondragover

ondragover 事件规定被拖动的数据能够被放置到何处。

默认地，数据/元素无法被放置到其他元素中。为了实现拖放，我们必须阻止元素的这种默认的处理方式。

这个任务由 ondragover 事件的 event.preventDefault() 方法完成：

```js
function allowDrop(ev){
    //默认数据和元素是不被拖物放置的，通过preventDefault()可阻止默认机制
    ev.preventDefault();
}
```



##### 18.2.4 进行放置 - ondrop

当放开被拖数据时，会发生 drop 事件。

在上面的例子中，ondrop 属性调用了一个函数，drop(event)：

```js
function drop(ev) {
    ev.preventDefault();
    var data = ev.dataTransfer.getData("text");
    ev.target.appendChild(document.getElementById(data));
}
```



### 18.3 HTML 本地存储

##### 18.3.1 HTML 本地存储对象

HTML 本地存储提供了两个在客户端存储数据的对象：

- window.localStorage - 存储没有截止日期的数据
- window.sessionStorage - 针对一个 session 来存储数据（当关闭浏览器标签页时数据会丢失）

在使用本地存储时，请检测 localStorage 和 sessionStorage 的浏览器支持：

```js
if (typeof(Storage) !== "undefined") {
    // 针对 localStorage/sessionStorage 的代码
} else {
    // 抱歉！不支持 Web Storage ..
}
```



##### 18.3.2 localStorage 对象

localStorage 对象存储的是没有截止日期的数据。当浏览器被关闭时数据不会被删除，在下一天、周或年中，都是可用的。

```js
// 存储
localStorage.setItem("lastname", "Gates");
// 取回
document.getElementById("result").innerHTML = localStorage.getItem("lastname");
localStorage.removeItem()// 移除某个值
localStorage.clear()// q
```

**实例解释：**

- 创建 localStorage 名称/值对，其中：name="lastname"，value="Gates"
- 取回 "lastname" 的值，并把它插到 id="result" 的元素中

上例也可这样写：

```js
// 存储
localStorage.lastname = "Gates";
// 取回
document.getElementById("result").innerHTML = localStorage.lastname;
```

删除 "lastname" localStorage 项目的语法如下：

```js
localStorage.removeItem("lastname");
```

**注释：名称/值对始终存储为字符串。如果需要请记得把它们转换为其他格式！**



下面的例子对用户点击按钮的次数进行计数。在代码中，值字符串被转换为数值，依次对计数进行递增：

```js
//判断localStorage中的clickcount的值是否为空，为空则执行else，赋值给clickcount=1,再一次执行则localStorage.clickcount=1，再执行localStorage.clickcount = Number(localStorage.clickcount) + 1;
if (localStorage.clickcount) {
    localStorage.clickcount = Number(localStorage.clickcount) + 1;
} else {
    localStorage.clickcount = 1;
}
document.getElementById("result").innerHTML = "您已经点击这个按钮 " +
localStorage.clickcount + " 次。";
```



##### 18.3.3 sessionStorage 对象

sessionStorage 对象等同 localStorage 对象，不同之处在于只对一个 session 存储数据。如果用户关闭具体的浏览器标签页，数据也会被删除。

下例在当前 session 中对用户点击按钮进行计数：

**实例:**

```js
if (sessionStorage.clickcount) {
    sessionStorage.clickcount = Number(sessionStorage.clickcount) + 1;
} else {
    sessionStorage.clickcount = 1;
}
document.getElementById("result").innerHTML = "在本 session 中，您已经点击这个按钮 " +
sessionStorage.clickcount + " 次。";
```



# 19. 标签

### 19.1 progress 

```html
<progress value="22" max="100">
```

![image-20220320222404517](html%E6%A0%87%E7%AD%BE.assets/image-20220320222404517.png)

| 属性  | 值       | 描述                       |
| :---- | :------- | :------------------------- |
| max   | *number* | 规定任务一共需要多少工作。 |
| value | *number* | 规定已经完成多少任务。     |



### 19.2 ruby

```html
<ruby>
陈<rt> chen </rt>
</ruby>
```

![image-20220320222819705](html%E6%A0%87%E7%AD%BE.assets/image-20220320222819705.png)



### 

















