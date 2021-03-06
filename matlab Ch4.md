## 第四章 matlab 可视化(画图功能)

### 4.1基本画图命令

| 方法             | 描述                                   |
| ---------------- | -------------------------------------- |
| plot(x,y)        | 各个点连线形成的图                     |
| subplot(m,n)     | m行n列的图                             |
| stem(x,y,'fill') | 火柴杆图(fill表示火柴点是空心还是实心) |
| bar(x,y,k)       | 条形图，k从0到1取值，表示宽度          |
| scatter(x,y)     | 散点图                                 |
| semilogx(x,y)    | 画出（log(x),y）的图                   |
| semilogy(x,y)    | 画出（x,log(y)）的图                   |
| polar(theta,r)   | 极坐标画图(给出极角和极径)             |

| 方法      | 描述   |
| --------- | ------ |
| pie(A,b)  | 饼图   |
| hist(a,x) | 直方图 |

#### 三种方法在同一个图画多个曲线

##### 1. plot(x,y1,'g',x,y2,'r') %只有plot能用这种方法

##### 2. 采用矩阵方式储存

```matlab
A=[];
A(:1)=y1;
A(:2)=y2;
plot(x,A)
```

##### 3.hold on 命令

### 4.3 三维绘图

| 方法                      | 描述                                       |
| ------------------------- | ------------------------------------------ |
| [U,V]=meshgrid(x,y)       | 利用x和y生成网格矩阵U,V,以便mesh和surf绘图 |
| mesh(X,Y,Z)               | 画空心图                                   |
| surf(X,Y,Z)               | 画实心图                                   |
| meshc(X,Y,Z)/surfc(X,Y,Z) | 画图并且投影等高线                         |
| plot3(x,y,z)              | 画空间曲线图                               |
| bar3(y,z)                 | 三维条形图                                 |
| bar3h(x,y)                | 竖着画三维条形图                           |
| scatter3(x,y,z)           | 散点图                                     |
| contour3(x,y,z)           | 等值线图                                   |

### 4.4 其他常用命令

| 方法                | 描述                 |
| ------------------- | -------------------- |
| imagesc()           | 将元素数值转换为颜色 |
| imwrite()           | 将矩阵变为图片       |
| imread('图片路径')  | 将图片转换为矩阵储存 |
| plotyy(x1,y1,x2,y2) | 双纵轴绘图           |
| stairs(x,y)         | 阶梯图               |
| area(x,y)           | 面积图               |
| compass(x,y)        | 矢量图               |
| text()              | 插入文本             |
| [x,y,z]=sphere()    | 绘制球面             |
| shading interp      | 连续曲面             |



