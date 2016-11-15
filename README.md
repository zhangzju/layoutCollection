# layout Collection
收集常用的页面布局的各种实现



## 圣杯布局

![grail layout](./grail/grail.PNG)

* 使用传统的浮动来实现，其中，main，left和right先后在container容器中
* main占据全部的width，left和right的width是固定的，给容器增加padding来使main的内容不被left和right遮盖
* left因为浮动原因会换行，这是，只要使用**margin-left:-100%**就可以使left回缩到main这一行的开始，而right则使用margin-left的负值，大小为自己的width，即可退缩到main这一行的右边。
* 对于容器container，需要清除浮动，可以使用伪类after的**clear:both**来清除浮动。



## 双飞翼布局

