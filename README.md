# 这篇文章用来整理前端的各种计算高度宽度方法的整理和说明。
* `clientheight`:可视内容区域高度（不包含border）。clientheight=height+padding-横向滚动轴高度。

![image](http://ww1.sinaimg.cn/large/639d3769gy1fpi48tidnrj20bf06v749.jpg)!

* `offsetheight`:开发者工具选择工具选中后看到的高度，可理解为div的可视高度， offsetheight=height+padding+border+横向滚动轴高度。

![image](http://ww1.sinaimg.cn/large/639d3769gy1fpi4fpifumj20bf06vaa1.jpg)

* `innerheight`:包括元素自身的高度+padding部分。 innerheight=height+padding

![image](http://ww1.sinaimg.cn/large/639d3769gy1fpi4qssm95j20f6072wei.jpg)


* `outerheight`:元素自身高度 + padding + border 。  outerheight=height+padding+border。如果参数为true时，高度为：元素自身高度 + padding + border +margin

![image](http://ww1.sinaimg.cn/large/639d3769gy1fpi4v0xqevj20f605x3yk.jpg)

* `height`:元素本身的高度，不包括padding、border、margin

![image](http://ww1.sinaimg.cn/large/639d3769gy1fpi4wbwig5j20f507rgln.jpg)

* `scrollheight`:容器可滚动高度。

![image](http://ww1.sinaimg.cn/large/639d3769gy1fpi4os28vqj20e70bhdfw.jpg)

* `style.height`:只有将高度定义在元素的style属性中这个变量才有效，才可以被读取。如果是抽取到了样式表中是无法取到的。





