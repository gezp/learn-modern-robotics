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

(a) 对于机械臂部分：$T^6$，对于底盘部分：$R^2\times S^1$，则整体为：$R^2\times T^7$

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

(a) $ (6-1-6)*6+(2*6)=0$, 不符合直觉，该机构的明显可活动的，即自由度大于0，因为关节之间的约束不是相互独立的。

(b) $(10-1-12)*6+(1*6+2*3+3*3)=3$

(c)$(5-1-6)*6+(2*3+3*3)=3$ 

> Tip: Cicular P 关节，还可以自旋，具有2个自由度。

(d)$(8-1-9)*6+(2*6+1*3)=3$ 

(e) $(8-1-8)*6+(1*2+2*4+1*2)=6$ 

(f) $(5-1-6)*6+(3*3+3*3)=6$ 

</details>

### Exercise 2.12 

使用Grubler公式计算空间机构自由度（2）

<details>
<summary>Solution (Click to expand)</summary>

(a) $ (8-1-9)*6+(2*6+1*3)=3$, （不确定）

(b) $ (9-1-9)*6+(1*9)=3$，不符合直觉，至少有4个自由度，最下面一个P关节，构成1个自由度，最上面两个P关节共同构成1个自由度，中间两个P关节独立分别构成1个自由度。

(c) $(14-1-18)*6+(1*6+2*6+3*6)=6$，符合直觉，上方平台具有6个自由度（3平移+3旋转）(不确定)。

(d) $(30-1-36)*6+(1*36)=6$，符合直觉，上方平台具有6个自由度（3平移+3旋转）(不确定)。

> Tip：一个关节应该对应两个连杆，如果3个连杆连接在同一个关节上（例如R关节），需要看作2个关节，4个连杆情况类似（看作3个关节）。

</details>

### Exercise 2.13

6×SS平台自由度

<details>
<summary>Solution (Click to expand)</summary>

Grubler公式：$(8-1-12)*6+(3*12)=6$

直觉上，上方平台应该具有4个自由度，可以在空间平移，以及自旋（绕z轴旋转）。

</details>

### Exercise 2.14

3×UPU平台自由度

<details>
<summary>Solution (Click to expand)</summary>

(a) Grubler公式： $(8-1-9)*6+(2*6+1*3)=3$

(b) 锁住3个P关节，上方平台不能再移动，该机构成为刚体，所以其自由度为3，符合Grubler公式的计算结果。

> Tip:  上方圆形平台是不能发生自旋的，由UPU中两个旋转关节轴平行约束确定。

</details>

### Exercise 2.15

使用Grubler公式计算不同排列的闭链空间机构自由度。

<details>
<summary>Solution (Click to expand)</summary>

(a) Grubler公式 $(6-1-6)*6+(1*6)=0$

(b) Grubler公式 $(6-1-6)*6+(1*6)=0$

结果显然不符合直觉。对于机构(a)，具有3个自由度（是一个类似平行四边形的机构），机构上方平台可以在一个平面内移动，并且能够调整倾角；对于机构（b），只有一个自由度，机构上方平台能有上下移动。

</details>

### Exercise 2.16

球面四连杆机构

<details>
<summary>Solution (Click to expand)</summary>

(a) 平面Grubler公式：$(4-1-4)*3+(1*4)=1$ （没太搞明白为什么用空间Grubler公式不行）

(b) C-Space拓扑结构为：$S^1$， 图示关节主动旋转，其它为被动关节。

(c) 不会

</details>

### Exercise 2.17

并联机器人（闭链）

<details>
<summary>Solution (Click to expand)</summary>

(a) Grubler公式：$(13-1-14)*6+(1*11+1*1+2*2)=4$

(b) 增加一个约束方程（点在直线上），故损失一个自由度，最终自由度为3.

(c) Grubler公式：$(11-1-12)*6+(1*12)=0$，自由度为0.

</details>

### Exercise 2.18

3×PUP 平台

<details>
<summary>Solution (Click to expand)</summary>

Grubler公式：$(8-1-9)*6+(1*6+2*3)=0$，自由度为0.

不符合直觉，显然可以上下移动，至少具有一个自由度。

</details>

### Exercise 2.19

Dual-Arm机器人

<details>
<summary>Solution (Click to expand)</summary>

Grubler公式：$(6-1-7)*6+(1*2+2*1+3*4)=4$，自由度为4.

</details>

### Exercise 2.20

蜻蜓机器人

<details>
<summary>Solution (Click to expand)</summary>

(a) Grubler公式：$(17-1-20)*6+(1*8+1*4+2*4+3*4)=8$，自由度为8.

(b) 因为一个刚体具有6个自由度，所以总和为$8+6=14$个自由度。

(c)  只有4个自由度，当机器人站立在地面时，每一条腿不能发生旋转，即固定住了，所以只有翅膀可以动，故自由度为4。

> Tip：不能使用Grubler公式？
>
> 每一个接触点可以看作一个S关节，地面看作一个link，即由Grubler可得：$(18-1-24)*6+(1*8+1*4+2*4+3*8)=-42+44=2$

</details>

### Exercise 2.21

TODO

<details>
<summary>Solution (Click to expand)</summary>

TODO

</details>

### Exercise 2.22

TODO

<details>
<summary>Solution (Click to expand)</summary>

TODO

</details>

### Exercise 2.23

TODO

<details>
<summary>Solution (Click to expand)</summary>

TODO

</details>

### Exercise 2.24

TODO

<details>
<summary>Solution (Click to expand)</summary>

TODO

</details>

### Exercise 2.25

TODO

<details>
<summary>Solution (Click to expand)</summary>

TODO

</details>

### Exercise 2.26

TODO

<details>
<summary>Solution (Click to expand)</summary>

TODO

</details>

### Exercise 2.27

TODO

<details>
<summary>Solution (Click to expand)</summary>

TODO

</details>

### Exercise 2.28

TODO

<details>
<summary>Solution (Click to expand)</summary>

TODO

</details>

### Exercise 2.29

TODO

<details>
<summary>Solution (Click to expand)</summary>

TODO

</details>

### Exercise 2.30

TODO

<details>
<summary>Solution (Click to expand)</summary>

TODO

</details>