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



#### 二、表单属性
> autocomplete、autofocus、multiple、placeholder、required

#### 三、链接属性
> <link>的sizes属性、<base>的target属性、超链接<a>

#### 四、其他属性
> script、ol、html、style
