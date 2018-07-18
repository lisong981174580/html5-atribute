## html5属性变化
> 标签=元素名+属性
#### 一、input
> 增加了email、url、number、range、Date picker、search、color、tel
* email
> 手机上直接调出键盘 输入@的时候可以调出相关邮箱
```
 <input type="email" name="email">
```
* url
> 手机上直接调出键盘 输入.的时候可以调出.com \ .cn
```
 <input type="url" name="url">
```

* tel
> 手机上直接调出数字键盘
```
 <input type="tel" name="tel">
```

* number
> 手机上直接调出数字键盘  只能输入数字 pc端还可以输入e
```
 <input type="number" name="number">
```
* Date picker
> 手机上直接调出指定日历 pc也是的
```
1、选择年月日 date
<input type="date" name="date">
2、选择年月 month
<input type="month" name="month">
3、选择年周 week
<input type="week" name="week">
4、选择时间 time
<input type="time" name="time">

5、datetime  不再兼容
<input type="datetime" name="datetime">

6、datetime-local 本地时间
<input type="datetime-local" name="datetime-local">
```

* Range input
```
<!--
 min:最小值
 max:最大值
 如果没有以上两者默认是0-100
-->
<input type="range" name="range" max="10" min="1">

```
* Search input
```
<!--自动匹配-->
<input type="search" name="search">
```
* Color input
```
<!--选择颜色-->
<input type="color" name="color">

```

#### 二、表单属性
> autocomplete、autofocus、multiple、placeholder、required
* autocomplete
```
<!--自动补全
autocomplete ：自动补全  默认是on      可以填on\off
-->
<form action=""  autocomplete="off">
    <input type="text" name="text">
    <input type="email" name="email">
    <input type="submit" name="submit">
</form>
```
* autofocus
```
<!--自动补全   适用于所有input
autofocus ：自动获取焦点
-->
 <input type="text" name="text" autofocus="autofocus">
</form>
```
* multiple
```
<!--
multiple ：上传多个文件
如果是email  带上这个属性后，后端将接收到一个数组
-->
    <input type="file" name="file" multiple="multiple">
    <input type="email" name="email" multiple="multiple">
```
* placeholder
> 表单的提示语  用于input

* required
> 定义是否必填
```
<!--
required:用于表单验证
-->
<form action=""  autocomplete="on">
    <input type="text" name="text" autofocus="autofocus">
    <input type="email" name="email"  required="required">
    <input type="submit" name="submit">
</form>
```
#### 三、链接属性
> <link>的sizes属性、<base>的target属性、超链接<a>
```
<head>
    <meta charset="UTF-8">
    <title>link</title>
    <!--
     sizes: 宽*高 对网站图标进行大小控制
     target:打开方式    _blank:弹出一个新窗口    _self:当前页打开  默认
    -->
    <link rel="ico" href="icon.gif" type="image/gif" sizes="16*16"  >
    <base  target="_blank"><!--标签为页面上的所有链接规定默认地址或默认目标。-->
</head>
<body>
<!--
media:对设备进行优化
hreflang:设置语言
rel:设置超链接的引用
-->
  <a href="" media="" hreflang="zh" rel="" ></a>
</body>
```
#### 四、其他属性
> script、ol、html、style
* script
```
<head>
    <meta charset="UTF-8">
    <title>script</title>
    <!--
    defer:加载完脚本后不执行，而是等整个页面加载之后再执行  只能在ie里面生效
    async:加载完成后立即执行，而不需要等到整个页面加载完成后执行  异步双线程加载  网页端多线程操作
    -->
    <script src=""  defer="defer"></script>
    <script src="" async="async" ></script>
    <script src=""></script>
</head>

```
* ol
```
<!--
start:起点
reversed：倒着数
-->
<ol start="10" reversed>
    <li></li>
    <li></li>
    <li></li>
    <li></li>
</ol>

```
* html、style
```
<!--
 manifest="cache.manifest"  定义页面离线应用文件
-->
<html lang="en" manifest="cache.manifest">
```
```
<body>
<!--
scoped：这个属性可以把style放在任意地方
-->
    <style scoped></style>
</body>

```
