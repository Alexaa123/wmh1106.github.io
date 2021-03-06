# 基本视觉格式化

## 基本元素框

> CSS 假定每个元素都会生成一个或多个矩形框，这成为元素框。

各个元素中心有个内容区，内容区周围有`可选的`内边距、边框、外边距。

内容的背景会应用到内边距 padding，外边距通常是透明的，从中可以看到父元素的背景。

内边距不能为负值，外边距可以。

边框颜色如果不设置，取元素内容的前景色（也就是文本什么颜色，边框就是什么颜色）；边框样式有缝隙，则可以通过缝隙看到背景色；边框宽度不能为负。

![边框取内容前景色](https://ws2.sinaimg.cn/large/006tKfTcgy1fndopvhoc7j30tm0qm74u.jpg)

**`默认：边框、内容、内边距具有相同的背景`**


---

![框模型](https://ws3.sinaimg.cn/large/006tKfTcgy1fndtx76vqrj30v20juqbm.jpg)


一般情况，
元素的`width`就是左内边界到右内边界的距离；
元素的`height`就是上内边界到下内边界的距离。

---

对不同类型的**`元素格式化`**时存在差异：

1. 块级元素处理不同于行内元素。
2. 浮动元素、定位元素也有各自不同的表现。

---

布局原则：同级元素里面，尽量不要出现不同类型的元素。也就是说内联元素最好是和内联元素同级，块元素和块元素同级，这样能避免很多问题哦
