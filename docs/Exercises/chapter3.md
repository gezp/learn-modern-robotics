# Chapter3

## Exercise 3.1

坐标系{s}，{a}，{b}之间的变换关系

**Soulution:**

(a) 画图，略

(b) 
$$
R_{sa}=
\begin{bmatrix}
0&-1&0\\
0&0&-1\\
1&0&0
\end{bmatrix},
R_{sb}=
\begin{bmatrix}
1&0&0\\
0&0&1\\
0&-1&0
\end{bmatrix}
$$
(c)
$$
R_{sb}^{-1}=R_{sb}^T=\begin{bmatrix}
1&0&0\\
0&0&-1\\
0&1&0
\end{bmatrix}
$$

(d) $R=R_{ab}=R_{sa}^TR_{sb}$

(e) $R=R_{sb}=Rot(\hat x,-90)$表示绕x轴旋转-90度，$R_1=R_{sa}R$表示将$R_{sa}$绕局部坐标系$\hat x_{a}$旋转-90度，$R_2=RR_{sa}$表示将$R_{sa}$绕世界坐标系$\hat x_{s}$旋转-90度。

(f) $p_s = R_{sb} p_b$

(g)$p'$表示移动点的位置， $p''$表示改变坐标系。

(h)$w_s = R_{sb} w_b$

(i) $[\hat w]\theta = log(R_{sa})$

(j) $R = exp([\hat w]\theta)$

## Exercise 3.2

坐标变换

**Soulution:**

根据题意：$p'=Rot(\hat z,-120)Rot(\hat y,135)Rot(\hat x,30)p=Rp$

(a) 先计算$R=Rot(\hat z,-120)Rot(\hat y,135)Rot(\hat x,30)= \\
\begin{bmatrix}
cos(-120)&-sin(-120)&0\\
sin(-120)&cos(-120)&0\\
0&0&1
\end{bmatrix}
\begin{bmatrix}
cos(135)&0&sin(135)\\
0&1&0\\
-sin(135)&0&cos(135)
\end{bmatrix}
\begin{bmatrix}
1&0&0\\
0&cos(30)&-sin(30)\\
0&sin(30)&cos(30)
\end{bmatrix}
$

然后计算$p'=Rp$

(b) R在(a)中已经计算。


## Exercise 3.3

坐标变换

**Soulution:**

(1) 通过观察，坐标元素只是顺序变了，说明是通过旋转坐标轴得到，不难得到

$R_1=\begin{bmatrix}
0&0&1\\
1&0&0\\
0&1&0
\end{bmatrix}$

(2)因为$||p_1||\ne||p'_1||$, 而旋转不会改变向量的长度，因此不存在这样的R 

(3) $w_3=p3\times p3'=(-4\sqrt2,0,4\sqrt2) \rightarrow \hat w_3 = (-\sqrt2/2,0,\sqrt2/2)$

$cos\theta_3=\frac{p\cdot p'}{||p||\cdot||p'||}=1/2 \rightarrow \theta_3 = 60°$ , 则$R_3=Rot(\hat w_3,\theta_3)$ 。

## Exercise 3.4

证明 $R_{ab}R_{bc}=R_{ac}$

**Soulution:**

不难得到

$[\hat x_b,\hat y_b,\hat z_b]=R^T\cdot  [\hat x_a,\hat y_a,\hat z_a] = R_{ab}^T [\hat x_a,\hat y_a,\hat z_a] $,

$[\hat x_c,\hat y_c,\hat z_c]=S^T\cdot  [\hat x_b,\hat y_b,\hat z_b] = R_{bc}^T [\hat x_b,\hat y_b,\hat z_b] $

综合上述可得 $[\hat x_c,\hat y_c,\hat z_c] = R_{bc}^TR_{ab}^T [\hat x_a,\hat y_a,\hat z_a] $

由于：$[\hat x_c,\hat y_c,\hat z_c] = R_{ac}^T [\hat x_a,\hat y_a,\hat z_a] $ 

则$R_{bc}^TR_{ab}^T= R_{ac}^T $ , 即 $R_{ab}R_{bc}=R_{ac}$


## Exercise 3.5

指数坐标

**Soulution:**

tr(R)=0

则$\theta=cos^{-1}(\frac{trR-1}{2})=2\pi/3$, $[\hat w]=\frac{1}{2sin\theta}(R-R^T)=(\sqrt3/3,-\sqrt3/3,\sqrt3/3)$.

## Exercise 3.6

指数坐标

**Soulution:**

由题得

$R= Rot(\hat x,\pi/2)Rot(\hat z,\pi)=
\begin{bmatrix}
1&0&0\\
0&0&-1\\
0&1&0
\end{bmatrix}
\begin{bmatrix}
-1&0&0\\
0&-1&0\\
0&0&1
\end{bmatrix}
=
\begin{bmatrix}
-1&0&0\\
0&0&-1\\
0&-1&0
\end{bmatrix}
$

由于tr(R)=-1，

则$\theta=\pi$, $[\hat w]=\frac{1}{\sqrt{2(1+r_{33})}}(r_{13},r_{23},1+r_{33})=(0,-\sqrt2/2,\sqrt2/2)$.

## Exercise 3.7

指数坐标

**Soulution:**

(a) 由于tr(R)=-1，

则$\theta=\pi$, $[\hat w]=\frac{1}{\sqrt{2(1+r_{33})}}(r_{13},r_{23},1+r_{33})=(\sqrt2/2,0,\sqrt2/2)$.

易知，$\theta_2=-\pi$, $[\hat w_2]=(-\sqrt2/2,0,-\sqrt2/2)$也是一组解

(b) 由于$v_1 \times v_2 = (-1,-1,1)$ 与$\hat w=(2/3,2/3,1/3)$不平行，所以无解。
