## D3.js 入门系列--选择元素和绑定元素
---

### 选择元素

在D3 中用于选择元素的函数有两个:

>  - d3.select(): 是选择所有指定元素的第一个
>  - d3.selectAll() : 是选择指定元素的全部

这两个函数返回的结果称为选择集,常见用法如下:

```js
var body = d3.select("body");       //选择文档中的body元素
var p1 = body.select("p");      //选择body中的第一个p元素
var p = body.selectAll("p");        //选择body中的所有的p元素
var svg = body.select("svg");       //选择body中的svg元素
var rects = body.selectAll("rect");     //选择svg中所有的svg元素
```

##### 选择集和绑定数据通常是一起使用的.

### 绑定元素

在D3中是通过以下两个函数来绑定数据的:

> - datum: 绑定一个数据到选择集上
> - data(): 绑定一个数组到选择集上,数组的各项值分别与选择集的各元素绑定

相对而言,data() 比较常用.






