# 各种height方法整理。
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


* `offsetTop`: 这个属性与offsetParent有关：返回该对象元素边界的左上角顶点相对于offsetParent的左上角顶点的水平偏移量。可以理解为容器相对于document的top的绝对偏移。等于top+marginTop
offsetTop = pardent.marginTop +pardent.borderWidth+ pardent.paddingWidth =20+20+40;
![image](http://ww1.sinaimg.cn/large/639d3769gy1fpi5zu4setj20g40bqdfw.jpg)

* `clientTop`: 容器内部相对于容器本身的top偏移，实际就是 上borderWidth 
* `style.height`:只有将高度定义在元素的style属性中这个变量才有效，才可以被读取。如果是抽取到了样式表中是无法取到的。

* window.innerWidth = width + padding + border + 纵向滚动条宽度
* window.innerHeight = height + padding + border + 横向滚动条高度
* window.outerWidth = width + padding + border + 纵向滚动条宽度
* window.outerHeight = height + padding + border + 横向滚动条高度 + 工具条高度
* document.body.clientWidth与document.body.clientHeight：document.body.clientWidth获得的也是可视区域的宽度，但是document.body.clientHeight获得的是body内容的高度，如果内容只有200px，那么这个高度也是200px,如果想通过它得到屏幕可视区域的宽高，需要样式设置，如下：

* `jquery.innerheight()`:高度范围是所匹配元素的高度height+padding
* `jquery.outerheight()`:高度范围是所匹配元素的高度height+padding+border；
* `outerheight(true)`:高度范围是所匹配元素的高度height+padding+border+margin；
* `$(window).width()` = width + padding  等同于 document.documentElement.clientWidth
* `$(window).height()` = height + padding 等同于 document.documentElement.clientHeight


