# Chapter2

### Exercise 2.1

描述n维空间，一个刚体的C-Space拓扑结构。

<details>
<summary>Solution (Click to expand)</summary>

平移自由度$a=n$，旋转自由度$b=n(n-1)/2$.

C-space的拓扑空间为:

* n=2：$R^2\times S^1$

* n=3：$R^3\times S^2 \times S^1$

* n>3：$R^n\times S^{n-1} \times \dots \times S^1$

</details>


### Exercise 2.2

分别计算（a）,(b)情况下的手臂自由度。

<details>
<summary>Solution (Click to expand)</summary>

shoulder, elbow, wrist joints考虑为spherical joint(ball-and-socket).

(a) (4-1-3)*6+(3+3+3)=9

(b)固定手掌的情况： (3-1-3)*6+(3+3+3)=3

</details>

### Exercise 2.3

手臂自由度（Exercise 2.2）扩展。

<details>
<summary>Solution (Click to expand)</summary>

- 略

</details>

### Exercise 2.4

驾驶汽车自由度。

<details>
<summary>Solution (Click to expand)</summary>

相比手臂系统，增加一个R关节（方向盘），连杆数量N没有改变，根据Grubler公式，即其自由度为n+1。

</details>

### Exercise 2.5

人机系统自由度

<details>
<summary>Solution (Click to expand)</summary>

Grubler公式：$(7-1-7)*6+(1*5+3*2)=5$

</details>

### Exercise 2.6

计算移动6R机械臂自由度

<details>
<summary>Solution (Click to expand)</summary>

(a) 对于机械臂部分：$T^6$，对于底盘部分：$R^2\times T^2$，则整体为：$R^2\times T^8$

> Tip：对于底盘，类比于滚动硬币，需要考虑轮子的旋转角度，但是其自由度为3，轮子的旋转角度与底盘二维位置具有约束关系。

(b) Grubler公式：$(7-1-7)*6+(1*7)=1$  ，自由度为1。（6R机械臂，看作7个连杆，6个R关节）

(c) Grubler公式：$(12-1-13)*6+(1*13)=1$  ，自由度为1。

</details>

### Exercise 2.7

计算SRS机械臂自由度

<details>
<summary>Solution (Click to expand)</summary>

(a) $(8-1-9)*6+(1*3+3*6)=9$

(b) $((2n+2)-1-3n)*6+(1*n+3*2n)=n+6$

(c)  $((2n+2)-1-3n)*6+(1*n+3*n+2*n)=6$

</details>

### Exercise 2.8

移动盘

<details>
<summary>Solution (Click to expand)</summary>

1条腿Grubler公式：$(m-1-J)*6+F=d$

n条腿Grubler公式：$(((m-2)*n+2)-1-J*n)*6+(F*n)=6$

则有d=6

</details>

### Exercise 2.9

使用Grubler公式计算平面机构自由度(1)

<details>
<summary>Solution (Click to expand)</summary>

> Tip : $dof=m(N-1-J)+\sum_{i=1}^J f_i$ （条件：关节之间的约束相互独立)，对于平面机构m=3。

(a): $(10-1-12)*3+(1*9+1*3)=3$

(b): $(14-1-18)*3+(1*16+1*2)=3$

(c): $(8-1-9)*3+(1*6+1*2+2*2)=4$

(d): $(6-1-7)*3+(1*6+1*1)=1$

(e): $(14-1-18)*3+(1*14+1*4)=3$

(f): $(7-1-9)*3+(1*8+1*1)=0$

</details>

### Exercise 2.10

使用Grubler公式计算平面机构自由度(2)

<details>
<summary>Solution (Click to expand)</summary>

(a): $(6-1-7)*3+(1*7)=1$

(b): $(6-1-6)*3+(1*4+1*2)=3$

(c): $(14-1-18)*3+(1*16+1*2)=3$

(d): $(21-1-27)*3+(1*18+1*9)=6$

</details>

### Exercise 2.11

使用Grubler公式计算空间机构自由度（1）

<details>
<summary>Solution (Click to expand)</summary>

>  Tip : $dof=m(N-1-J)+\sum_{i=1}^J f_i$ （条件：关节之间的约束相互独立），对于空间机构m=3。

(a) $ (6-1-6)*6+(2*6)=6$

符合直觉。

(b) $(11-1-12)*6+(1*6+1*3+3*3)=6$

> Tip：注意RP关节之间的link，也就是滑块link，不能漏掉。另一种做法就是把RP关节看作一个关节，其自由度为2，此时在Grubler中，link数量发生了变化（不考虑滑块link）。

(c)$(10-1-11)*6+(1*5+1*3+3*3)=5$ 

> Tip: Cicular P 关节那里的滑块link，有两个关节，即R+P关节。

(d)$(8-1-9)*6+(2*6+1*3)=3$ 

(e) $(8-1-8)*6+(1*2+2*4+1*2)=6$ 

(f) $(5-1-6)*6+(3*3+3*3)=6$ 

</details>

### Exercise 2.12 

使用Grubler公式计算空间机构自由度（2）

<details>
<summary>Solution (Click to expand)</summary>

(a) $ (8-1-9)*6+(2*6+1*3)=3$ 

(b) $ (9-1-9)*6+(1*9)=3$

不符合直觉，至少有4个自由度，最下面一个P关节，构成1个自由度，最上面两个P关节共同构成1个自由度，中间两个P关节独立分别构成1个自由度。

(c) $(14-1-18)*6+(1*6+2*6+3*6)=6$

符合直觉，上方平台具有6个自由度（3平移+3旋转）(不确定)。

(d) $(30-1-36)*6+(1*36)=6$

符合直觉，上方平台具有6个自由度（3平移+3旋转）(不确定)。

> Tip：一个关节应该对应两个连杆，如果3个连杆连接在同一个关节上（例如R关节），需要看作2个关节，4个连杆情况类似（看作3个关节）。

</details>

### Exercise 2.13

6×SS平台自由度

<details>
<summary>Solution (Click to expand)</summary>

Grubler公式：$(8-1-12)*6+(3*12)=6$

上方平台可以在空间中平移运动，以及自旋（绕z轴旋转）。

> Tip，直觉上，具有3个自由度，对于空间刚体具有6个自由度，该平台显然被约束保持水平，说明具有两个约束（roll,pitch角约束），同时该机构可以平移，当考虑进行上下平移时，是通过自旋实现的（yaw角），所以，这里也有个约束方程，最终自由度为6-3=3。

</details>

### Exercise 2.14

3×UPU平台自由度

<details>
<summary>Solution (Click to expand)</summary>

(a) Grubler公式： $(8-1-9)*6+(2*6+1*3)=3$

(b) 锁住3个P关节，上方平台不能再移动，该机构成为刚体。该机构具有3个主动关节，所以其自由度为3，符合Grubler公式的计算结果。

> Tip:  上方圆形平台是不能发生自旋的，由UPU中两个旋转关节轴平行约束确定。

</details>

### Exercise 2.15

使用Grubler公式计算不同排列的闭链空间机构自由度。

<details>
<summary>Solution (Click to expand)</summary>

(a) 对于该机构的所有link在同一个平面运动，故采用平面Grubler公式，

即 $(6-1-6)*3+(1*6)=3$ ，自由度为3。

结果符合直觉，机构上方平台可以在一个平面内移动，并且能够调整倾角。

(b) Grubler公式 $(6-1-6)*6+(1*6)=0$，，自由度为0.

结果不符合直觉，对于该机构，具有一个自由度，机构上方平台能有上下移动。

</details>

### Exercise 2.16

球面四连杆机构

<details>
<summary>Solution (Click to expand)</summary>

(a) 该机构所有link可以看作在球面上移动，采用平面Grubler公式。

即：$(4-1-4)*3+(1*4)=1$ 

(b) C-Space拓扑结构为：$S^1 \times S^1 \times S^1 \times S^1=T^4$

> Tip，该机构的C-space为4维，自由度为1，说明该闭链结构具有3个约束方程（参考平面四连杆机构）。

(c) 略（TODO）

</details>

### Exercise 2.17

并联机器人（闭链）

<details>
<summary>Solution (Click to expand)</summary>

(a) Grubler公式：$(13-1-14)*6+(1*11+1*1+2*2)=4$

(b) 增加一个约束方程（点在直线上），故损失2个自由度，最终自由度为2.

> Tip：空间直线方程，可以看作两个平面的交集，即两个方程。

(c) 所有的R关节轴经过点A，则该机构所有link可以看作在球面上移动，采用平面Grubler公式。

即：$(11-1-12)*3+(1*12)=3$，自由度为6.

</details>

### Exercise 2.18

3×PUP 平台

<details>
<summary>Solution (Click to expand)</summary>

Grubler公式：$(8-1-9)*6+(1*6+2*3)=0$，自由度为0.

不符合直觉，显然可以上下移动，至少具有一个自由度。

> TIP：上方PU关节之间的link（滑块link）很容易漏掉。

</details>

### Exercise 2.19

Dual-Arm机器人的自由度

<details>
<summary>Solution (Click to expand)</summary>
物体可以在桌面滑动，将物体与桌面的约束看作一个关节，其自由度为2。

则由Grubler公式：$(7-1-8)*6+(1*2+2*1+3*4+2*1)=6$，自由度为6。

</details>

### Exercise 2.20

蜻蜓机器人的自由度

<details>
<summary>Solution (Click to expand)</summary>

(a) Grubler公式：$(17-1-20)*6+(1*8+1*4+2*4+3*4)=8$，自由度为8.

(b) 因为一个刚体具有6个自由度，所以总和为$8+6=14$个自由度。

(c)  每一个接触点可以看作一个S关节，地面看作一个link，即由Grubler可得：$(18-1-24)*6+(1*8+1*4+2*4+3*8)=-42+44=2$

</details>

### Exercise 2.21

毛虫机器人的自由度

<details>
<summary>Solution (Click to expand)</summary>

(a) Grubler公式：$(8-1-7)*6+(3*5+1*2)=17$，自由度为17. （RPR关节具有3个自由度）

(b) link保持接触叶子表面，受到了曲面约束（只能在二维曲面面上移动），损失一个自由度，故6个link接触叶子时自由度为17-6=11

(c) 由(b)同理，故2个link接触叶子时自由度为17-2=15

</details>

### Exercise 2.22

四指机械手（URR×4）的自由度

<details>
<summary>Solution (Click to expand)</summary>

(a) 对于四指机械手，由Grubler公式：$(13-1-12)*6+(1*8+2*4)=16$

刚体接触表面的约束为曲面约束，即只能在二维曲面上运行，损失1个自由度，则最终自由度为16-4=12.

对于n指情况， $((3*n+1)-1-3*n)*6+(1*2n+2*n)-n=3n$

(b) 对于四指机械手，由Grubler公式：$(13-1-12)*6+(1*8+3*4)=20$

刚体接触表面的约束为曲面约束，即只能在二维曲面上运行，损失1个自由度，则最终自由度为20-4=16.

对于n指情况，$((3*n+1)-1-3*n)*6+(1*2n+3*n)-n=4n$

(c) 由于手掌，椭球物体被固定住，则每一根手指相互独立，对于一根手指，可以将手掌，椭球物体以及指尖看作一个link，不难看出，手指被固定住，不能移动，故该系统的自由度为0。

(d)  由Grubler公式：$(13-1-16)*6+(1*8+2*4+3*4)=4$

> Tip：可以将手掌，椭球物体看作一个link，椭球与指尖由一个S关节连接。

</details>

### Exercise 2.23

曲柄滑块机构

<details>
<summary>Solution (Click to expand)</summary>

设曲柄关节角度为$\theta$，滑块的位移为$x$。

$x=\begin{cases} 2Lcos\theta & -\frac{\pi}{2}<\theta <\frac{\pi}{2} \\ 0 & otehrs \end{cases} $

> 没看懂题目意思（TODO）

</details>

### Exercise 2.24

平面四连杆机构

<details>
<summary>Solution (Click to expand)</summary>

(a) Grubler公式：$(4-1-4)*3+(1*4)=1$，自由度为1

(b) 略（TODO）

</details>

### Exercise 2.25

平面四连杆机构（扩展）

<details>
<summary>Solution (Click to expand)</summary>

略（TODO）

</details>

### Exercise 2.26

平面2R开链机器人的工作空间

<details>
<summary>Solution (Click to expand)</summary>

(a) C-space为 $S^1\times S^1=T^2$，即$(\theta_1,\theta_2)$。

(b) 工作空间为一个圆环，内环半径为1，外环半径为3，即$\{(x,y)|1\le x^2+y^2 \le 9\}$

(c) 略（TODO）

</details>

### Exercise 2.27

平面3R开链机器人的工作空间

<details>
<summary>Solution (Click to expand)</summary>

(a) 工作空间为一个圆环，内环半径为2，外环半径为8.

(b) 工作空间为一个圆，半径为8，显然情况(b)的机器人具有更大的位形空间。

(c) 对于平面开链机器人，增加最后一个link长度，可以增加工作空间半径（为所有link之和）。

</details>

### Exercise 2.28

任务空间

<details>
<summary>Solution (Click to expand)</summary>

(a) 黑板上书写，任务空间为$R^2 \times S^2$ ，$R^2$表示粉笔在二维黑板上的位置，$S^2$表示粉笔的朝向。

(b) 挥动指挥棒，任务空间为$R^3 \times S^2$，$R^3$表示指挥棒在空间中的位置，$S^2$表示指挥棒的朝向。

</details>

### Exercise 2.29

C-space拓扑结构

<details>
<summary>Solution (Click to expand)</summary>

(a) $R^2\times S^1$

(b) $S^2\times S^1$

(c) $R^2 \times S^1 \times S^1 \times S^1 \times[a,b]\times S^1= R^2 \times T^4 \times [a,b]$

(d) $R^3\times S^2 \times S^1 \times T^6 = R^3 \times S^2 \times T^7$

> Tip：对于平面刚体的位形空间为$R^2\times S^1$，对于空间刚体的位形空间为$R^3\times S^2 \times S^1$

</details>

### Exercise 2.30

滚硬币算法

<details>
<summary>Solution (Click to expand)</summary>

（1）首先输入$\dot \theta,\dot \phi$，硬币做圆周运动（运动半径为$R=\frac{\dot \theta r}{\dot \phi }$），运动到目标位形的硬币切线上（硬币x方向所在的直线）。

（2）然后，只输入$\dot \theta$，使得$\dot \phi=0$，硬币做直线运动，运动到目标位形。

</details>

### Exercise 2.31 

差分移动底盘的运动约束

<details>
<summary>Solution (Click to expand)</summary>

(a) 不难得到，机器人前进的速度为$v_{forward}=\frac{r}{2}(w_1+w_2)$，自旋的速度为 $\dot \theta = \frac{r}{2d}(w_2-w_1)$

$\dot x= v_{forward}\cos\theta= \frac{r\cos\theta}{2}(w_1+w_2)$，

$\dot y= v_{forward}\sin\theta= \frac{r\sin\theta}{2}(w_1+w_2)$，

则：$ \begin{cases} g_1(q)=[\frac{1}{2}r\cos\theta,\frac{1}{2}r\sin\theta,-\frac{r}{2d},1,0]  \\ g_2(q)=[\frac{1}{2}r\cos\theta,\frac{1}{2}r\sin\theta,\frac{r}{2d},0,1]\end{cases}$

当$w_1=w_2$时，机器人只发生x方向的平移；当$w_1=-w_2$时，机器人只发生自旋；其它情况为平移与自旋的叠加运动。

(b) 由(a)中三个等式不难得到3个Pfaffian约束
$$
A(q)\dot q =

\begin{bmatrix}
1 & 0 & 0 & -\frac{r\cos\theta}{2} & -\frac{r\cos\theta}{2}\\
0 & 1 & 0 & -\frac{r\sin\theta}{2} & -\frac{r\sin\theta}{2} \\
0 & 0 & 1 & \frac{r}{2d} & -\frac{r}{2d}
\end{bmatrix}

\begin{bmatrix}
\dot x \\
\dot y \\
\dot \theta \\
\dot \phi_1 \\
\dot \phi_2 \\
\end{bmatrix}

=0
$$

> 在(a)中，一共有4个等式，其中只有3个有效等式（关于$\dot x, \dot y，\dot \theta$的等式），$v_{forward}$为中间产物。

(c) 显然，这三个约束都是非完整约束(nonholonomic constraints)。

</details>

### Exercise 2.32 

完整约束 (holonomic constraints)与非完整约束 (nonholonomic constraints)

<details>
<summary>Solution (Click to expand)</summary>

(a) 是不完整约束。

(b) 第一个是不完整约束，第二个是完整约束。

对于第二个约束，有$g(q)=q_3\sin q_1+q_4 \cos q_1 =0 \longrightarrow \frac{\partial g}{\partial q} q=0$，

</details>