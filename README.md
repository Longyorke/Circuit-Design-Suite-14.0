# 2021暑假小学期

Circuit-Design-Suite-14.0

组合函数信号发生器及波形巡回切换电路的设计与实现



## 2 设计的基本过程与方案

### 2.1 方波-三角波产生电路

#### 2.1.1 实验原理

如将滞回比较器和积分器首尾相接形成反馈的闭环系统，则比较器输出方波经积分器积分后可得到三角波，三角波又经触发器自动翻转形成方波，这样即构成了方波-三角波发生器。图中运用了TL074组成的运放积分电路。
方波-三角波产生电路可由积分器和比较器同时产生三角波和方波。

#### 2.1.2 实验数据及计算

电路震荡频率：
$$
f=R_1/(4R_2 (R_3+R_5)C_1 )
$$
![image-20210622195454928](https://i.loli.net/2021/06/22/7Qk9xVCUbeqcM3z.png)

#### 2.1.3 实验原理图

![image-20210622195535362](https://i.loli.net/2021/06/22/ImYtUgEWJZLTfi8.png)

其中，R7控制方波的幅度，R5控制方波三角波的频率，R6控制三角波的幅度,实际可调。

#### 2.1.4 方波三角波的示波器显示

![image-20210622200013878](https://i.loli.net/2021/06/22/B57rULHCu3WgQAl.png)



#### 2.1.5 故障问题及解决办法



### 2.2 正弦波产生电路

#### 2.2.1 实验原理

将发生的三角波经过一个一阶低通滤波电路，如图 2-3所示，则三角波经低通滤波后可产生正弦波。图中运用了TL074及电容和电阻共同构成了低通滤波器。

#### 2.2.2 实验数据及计算

#### 2.2.3 实验原理图

![image-20210624093332039](https://i.loli.net/2021/06/24/YnICK7kU3OdAeh1.png)

其中,R32控制正弦波的幅度

#### 2.2.4 正弦波的示波器显示

![image-20210624093807888](https://i.loli.net/2021/06/24/DUQzwWeRngGjuCM.png)



#### 2.2.5 方波三角波正弦波的示波器显示

![image-20210624094336453](https://i.loli.net/2021/06/24/A8HjfpyCoer2uY4.png)



#### 2.2.6 故障问题及解决办法



### 2.3 锯齿波产生电路

#### 2.3.1 实验原理

锯齿波产生电路可在方波发生器和积分器之间加上两个二极管以及滑动变阻器来实现，滑动变阻器可用来调节占空比。
积分电路正向积分的时间常数远大于反向积分的时间常数，或者反向积分的时间常数远大于正向积分的时间常数，那么输出电压上升和下降的斜率相差很多，就可以获得锯齿波。利用二极管的单向导电性使积分电路两个方向的积分通路不同，就可以得到锯齿波发生电路。

#### 2.3.2实验数据及计算

根据三角波发生电路振荡周期的计算方法，可得出上升时间和下降时间，分别为









![image-20210624100351448](https://i.loli.net/2021/06/24/obfXVA3eGEsTwr1.png)

