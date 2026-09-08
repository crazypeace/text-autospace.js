text-autospace.js
=================

自动在中英文间添加空白符，优化中文排版。

使用方法及演示参考[demo](http://crazypeace.github.io/text-autospace.js/)

## 面对小白的使用说明

除了引入本js，你还需要引入jquery.js，所以你需要引入
```
<script src='https://cdn.bootcss.com/jquery/2.1.1/jquery.min.js'/>
<script src='https://crazypeace.github.io/text-autospace.js/text-autospace.min.js'/>
```

在你需要处理的HTML元素中添加`class="han-la"`
如`<html>`
```
<html class="han-la">
```

或
```
<div class='han-la'>
```

添加CSS
```
.han-la hanla:after {
	content: " ";
	display: inline;
	font-family: Arial;
	font-size: 0.89em;
}

.han-la code hanla,
.han-la pre hanla,
.han-la kbd hanla,
.han-la samp hanla {
	display: none;
}

.han-la ol > hanla,
.han-la ul > hanla,
.han-la tr > hanla {
	display: none;
}
```

如果你希望增加不应用此js的区域，比如blockquote，请添加
```
.han-la blockquote hanla {
	display: none;
}
```

## 用你的STAR告诉我这个Repo对你有用 Welcome STARs! :)
