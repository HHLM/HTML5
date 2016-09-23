# HTML5
html5学习小笔记
## 常用标签

### 1、标题标签一共有6个，h1、h2、h3、h4、h5、h6分别为一级标题、二级标题、三级标题、四级标题、五级标题、六级标题。并且依据重要性递减。`<h1>是最高的等级。`

### 2、 `<em>或<strong>标签。`

有了段落又有了标题，现在如果想在一段话中特别强调某几个文字，这时候就可以用到`<em>或<strong>`标签。
em 默认用斜体表示； stron 默认用粗体表示

<span style= "color:red"> `span`标签是没有语义的，它的作用就是为了设置单独的样式用的。</span>

### 3、`<q>标签`
引用一段文字用这个：比如 
<p>周瑜，不可否认，他是历史上一个了不起的英雄人物！确实也配的上那句 <q>聪明秀出为之英，胆略过人为之雄。</q></p>

###  4、`<blockquote>`

```html
假如应用别人的诗歌时候可以用这个，比如：
<blockquote>暗淡轻黄体性柔，情疏迹远只香留。何须浅碧深红色，自是花中第一流。</blockquote>
```
假如应用别人的诗歌时候可以用这个，比如：
<blockquote>暗淡轻黄体性柔，情疏迹远只香留。何须浅碧深红色，自是花中第一流。</blockquote>

### 5、`<br /> 换行标签`

<p>暗淡轻黄体性柔，<br/>情疏迹远只香留。<br/>何须浅碧深红色，<br/>自是花中第一流。</p>

### 6、`&nbsp; 空格`

来源：作文网&nbsp;&nbsp;作者：为梦想而飞 

### 7、`<address>标签，为网页加入地址信息`

地址：<address>广东省深圳市南山区软件产业基地</address>

### 8、`<code>标签 和<pre>标签`

插入一行代码时候用这个
插入多行代码时候用`<pre>`


<code> {background-image:linear-gradient(left, red 100px, yellow 200px);}</code>

<pre>
    cell.textLabel.highlightedTextColor = [UIColor redColor]; //点击时候 文字的颜色
    cell.textLabel.text = dataArray[indexPath.section][indexPath.row];
    cell.textLabel.highlightedTextColor = [UIColor redColor]; //点击时候 文字的颜色
 </pre>

### 9、`<ul> 、<li> 和 <ol>标签 `

<ol>
     <li>前端开发 </li>
     <li>学习html</li>
     <li>javascript学习</li>
</ol>

<ul>
     <li>前端开发 </li>
     <li>学习html</li>
     <li>javascript学习</li>
</ul>

### 10、`<table>标签`
创建表格的四个元素：
table、tbody、tr、th、td

<!--表格开始-->
<table style = "border:1px solid red">
<!--当表格内容非常多时，表格会下载一点显示一点，但如果加上<tbody>标签后，这个表格就要等表格内容全部下载完才会显示。-->
			<tbody>
				<!--有几行就写几对tr标签-->
				<caption>表格的标题随便起个名字吧</caption>
				<tr>
					<td>姓名</td><!--表示单元格 一行中有几对td就有几个单元格-->
					<td>性别</td>
					<td>年龄</td>
				</tr>
				<tr>
					<td>张三</td><!--表示单元格 一行中有几对td就有几个单元格-->
					<td>男</td>
					<td>18</td>
				</tr>
				<tr>
					<td>李四</td><!--表示单元格 一行中有几对td就有几个单元格-->
					<td>女</td>
					<td>16</td>
				</tr>
			</tbody>
</table>

### 11、`<a>标签`
<a href="http://www.imooc.com/code/315" title="前端开发学习">前端开发学习</a>
<!--图片-->
<img src="http://img.mukewang.com/52da54ed0001ecfa04120172.jpg" alt="下载失败时的替换文本" title = "提示文本">

```
1、src：标识图像的位置；
2、alt：指定图像的描述性文本，当图像不可见时（下载不成功时），可看到该属性指定的文本；
3、title：提供在图像可见时对图像的描述(鼠标滑过图片时显示的文本)；
4、图像可以是GIF，PNG，JPEG格式的图像文件。
```
### 12、`<form>标签`

<form method="post" action="save.php">
      <label for="username">用户名:</label>
      <input type="text"  name="username" id="username" value="" />
      <br />
      <label for="pass">密码:</label>
      <input type="password"  name="pass" id="pass" value="" />    
      <input type="submit" value="确定"  name="submit" />
      <input type="reset" value="重置" name="reset" />
</form>  
<br />
<form  method="post" action="save.php">
        <label>联系我们</label>
        <textarea cols="50" rows="10" >在这里输入内容...</textarea>
        <input type="submit" value="确定"  name="submit" />
    <input type="reset" value="重置"  name="reset" />
</form>

<br />
```
1.<form> ：所有表单控件（文本框、文本域、按钮、单选框、复选框等）都必须放在<form></form>标签之间（否则用户输入的信息可提交不到服务器上哦！）。
2.action ：浏览者输入的数据被传送到的地方,比如一个PHP页面(save.php)。
3.method ： 数据传送的方式（get/post）
```
```
1、<textarea>标签是成对出现的，以<textarea>开始，以</textarea>结束。
2、cols ：多行输入域的列数。
3、rows ：多行输入域的行数。
4、在<textarea></textarea>标签之间可以输入默认值。

```

