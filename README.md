


## 论文假设
BG is static 

对于移动的BG 需要通过运动估计来补偿BG的运动，才能使用该方法进行空洞填充


## 输入内容参数
采用DERS获取的深度图
利用VSRS 2.0 获取合成视图

## step 1 深度图像的空洞填补
取 位置 i 的周围一个平方区域，利用k-means(k=2) 获取两分类分别代表FG 和BG ，然后对于空洞部分的像素，如果其大于
