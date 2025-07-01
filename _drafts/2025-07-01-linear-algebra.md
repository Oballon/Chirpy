线性代数

线性代数概念性极强，知识的融会贯通是备考关键

# 默认章节

## 考情分析

选择题：3道
填空题：1道
大题：1道

难度近几年呈上升趋势

## 考查轻重点分析

行列式：考查偏易
矩阵：考查难点
特征值、特征向量：难点

## 重要经验

**线性代数知识体系关联性极强**
若所给题设条件奇怪，考虑是在间接给性质
**各知识串用性很高，故熟悉重要结论很重要**

**具体型相关问题善用观察法**
**抽象型相关问题灵活寻找关系**

勿拘泥于矩阵变换中，考虑从实际意义把握（向量组、方程组、二次型等）

## 知识体系讨论

工具：行列式、**矩阵**
主题：向量组==方程组
应用：**特征值、特征向量**、相似，二次型

## 基础解系、通解、特征向量的书写规范

$$\begin{array}{rl}
基础解系：&\xi_1=(\quad,\quad,\cdots,\quad)^T,\xi_2=(\quad,\quad,\cdots,\quad)^T,\cdots,\xi_n=(\quad,\quad,\cdots,\quad)^T\\
\ \\
通解：&k_1\xi_1+k_2\xi_2+\cdots+k_n\xi_n\quad (k_1,k_2,\cdots,k_n为任意常数)\\
\ \\
单特征向量：&k\xi\quad (k\neq0)\\
\ \\
重特征向量：&k_1\xi_1+k_2\xi_2+\cdots+k_n\xi_n\quad (k_1,k_2,\cdots,k_n不同时为零)
\end{array}$$

# 行列式

## 行列式的性质

$$交换\ |\alpha_1,\alpha_2,\alpha_3|=-|\alpha_2,\alpha_1,\alpha_3|\\
 \ \\
倍加\ |\alpha_1,\alpha_2,\alpha_3|=|\alpha_1,k\alpha_1+\alpha_2,\alpha_3|\\
\ \\
倍乘或提取因子\ |k\alpha_1,\alpha_2,\alpha_3|=k|\alpha_1,\alpha_2,\alpha_3|\\
\ \\
拆分\ |\alpha_1,\alpha_2,\alpha_3+\beta|=|\alpha_1,\alpha_2,\alpha_3|+|\alpha_1,\alpha_2,\beta|\\
\ \\
成比例\ |\alpha_1,\alpha_2,k\alpha_2|=0$$
$$|kA|=k^n|A|\\
|A|=|A^T|\\
|AB|=|A||B|（A,B为同型方阵）
$$
$$|A|=\prod_{i=1}^n\lambda_i=\lambda_1\lambda_2\cdots \lambda_n（对相似对角化无要求）$$

## 逆序数计算

$$\tau(i_1,i_2,\cdots i_n):元素后面小于此元素的个数之和$$

## 副对角行列式

$$\bigg| \quad\quad\bigg|=(-1)^\frac{n(n-1)}{2}\prod_{i=1}^n\Delta$$

## 爪型行列式

$$第一列减j列的\frac{a_{i1}}{a_{ij}}即可化为上三角矩阵$$
![](pic-linear-algebra\Markji_1751359347607.png)

## 异爪型行列式

**递推法，按“尾部”行（列）展开**
![](pic-linear-algebra\Markji_1751359383717.png)
$$选取“两爪”(a_n,\quad x)较简单$$

## 三对角行列式

**递推法，按第一行或第一列展开，整理可得两两递推式**
![](pic-linear-algebra\Markji_1751359436900.png)
$$\quad\ D_{n}=2aD_{n-1}-a^2D_{n-2}\\
\Rightarrow D_n-aD_{n-1}=a(D_{n-1}-aD_{n-2})\\
\Rightarrow D_n-aD_{n-1}=a^n\\
\Rightarrow D_n=a^n+aD_{n-1}=a^n+a(a^{n-1}+aD_{n-2})=(n-1)a^n+a^{n-1}\cdot 2a$$

## 加边法

**针对除主对角元素外，各行（列）均有相同的元素**
![](pic-linear-algebra\Markji_1751359460950.png)
$$行元素相同加行，列元素相同加列$$

## 拆项法

![](pic-linear-algebra\Markji_1751359548244.png)
![](pic-linear-algebra\Markji_1751359563809.png)
![](pic-linear-algebra\Markji_1751359575364.png)
![](pic-linear-algebra\Markji_1751359593126.png)

## 二维“品”字型行列式

![](pic-linear-algebra\Markji_1751359922327.png)

## n维“品”字型行列式

![](pic-linear-algebra\Markji_1751359941213.png)![](pic-linear-algebra\Markji_1751359959730.png)

## 拉普拉斯展开定理

$$行列式可按任意k(1\leqslant k\leqslant n-1)行（列）展开，\\即在n阶行列式|A|中，可以任意选定k行（列），\\则含于此k行（列）中的所有k阶子式与其代数余子式乘积之和为|A|的值\\
（代数余子式下标为子式下标）$$
![](pic-linear-algebra\Markji_1751359996872.png)
$$拉普拉斯行、列展开：\\
|A|=\sum_{j=1}^{n}a_{1j}A_{1j}=a_{11}A_{11}+a_{12}A_{12}+\cdots+a_{1n}A_{1n}\\
A_{ij}=(-1)^{i+j}M_{ij}$$

## 分块矩阵的拉普拉斯展开式

**由拉普拉斯定理，可推广至n维分块阵**
$$\left|  
\begin{array}{cc}
A\\
\\
&B
\end{array}
\right|=
\left|  
\begin{array}{cc}
A&C\\
\\
&B
\end{array}
\right|=
\left|  
\begin{array}{cc}
A&\\
\\
C&B
\end{array}
\right|=|A||B|$$
$$\left|  
\begin{array}{cc}
&A\\
\\
B&
\end{array}
\right|=\left|  
\begin{array}{cc}
C&A\\
\\
B
\end{array}
\right|=\left|  
\begin{array}{cc}
&A\\
\\
B&C
\end{array}
\right|=(-1)^{mn}|A||B|（高维分块不是(-1)^{mnq\cdots}）\\
注：(-1)^{p+q}=(-1)^{m(m+n+1)}=(-1)^{mn}$$
$$\left|  
\begin{array}{cc}
A&B\\
\\
B&A
\end{array}
\right|=|(A+B)(A-B)|=|A^2-B^2|=|A^2-ABA^{-1}B|（前提：AB=BA，且A可逆）$$

## 范德蒙德行列式

$$D=\left|
\begin{array}{cccc}
1&1&\cdots&1\\
\\
a_1&a_2&\cdots& a_n\\
\\
\vdots&\vdots&&\vdots&\\
\\
a_1^{n-1}&a_2^{n-1}&\cdots& a_n^{n-1}
\end{array}
\right|
=\prod_{1\leqslant i\leqslant j\leqslant n}(a_j-a_i)\\
\ \\
(n-1)!项之积，“右减左，下减上”$$
$$注：若非两类标准型，逐行对换化标准型即可$$

## 重要结论

$$tr(A^*)=A_{11}+A_{22}+A_{33}=\lambda_1^*+\lambda_2^*+\lambda_3^*\xlongequal{|A|\neq0}\lambda_2\lambda_3+\lambda_1\lambda_3+\lambda_1\lambda_2\quad $$

## 行列式重要经验

递推时注意(-1)^k，多推一维，以防出错

## 行列式函数求某次项题型

$$f(x)=\left|
\begin{array}{cccc}
x&\underline{2x}&7&2\\
\\
1&x&5&1\\
\\
2&-1&3x&3\\
\\
3&2&1&4x
\end{array}
\right|\quad （考查逆序数）$$
$$x^4,x^3\rightarrow找同行同列x项\\
常数项\rightarrow f(0)$$

## 拉普拉斯展开考查题型

**“乘错行、列”展开式为0（反向还原行列式，某两行、列线性相关）**

$$\left\{
\begin{array}{l}
错行、列：直接为零\\
\\
反向还原计算：直接还原，或凑错行、列
\end{array}
\right.$$

## 具体型行列式计算
逆序数计算法、拉普拉斯展开、初等变换、特征值

**逆序数计算法：**
$$\bigg|\quad\quad\quad\bigg|=\sum(-1)^{\tau(j_1j_2\cdots j_n)}a_{1j_1}a_{2j_2}\cdots a_{nj_n}\qquad n!项之和，不同行、不同列$$

**拉普拉斯展开（余子式展开）：**
$$|A|=a_{i1}A_{i1}+a_{i2}A_{i2}+\cdots+a_{in}A_{in}$$

**初等变换：**倍乘会改变行列式，注意提取
**特征值求行列式：**特征值计算技巧
$$A=
\left(
\begin{array}{}
3&2&2\\
\\
2&3&2\\
\\
2&2&3
\end{array}
\right)=
E+
\left(
\begin{array}{}
2&2&2\\
\\
2&2&2\\
\\
2&2&2
\end{array}
\right)=E+B\\
\qquad\qquad\qquad\qquad\qquad\Rightarrow\lambda=1+tr(B)=1+6=7$$

## 抽象行列式重要技巧

**善用单位矩阵E构造行列式（可逆矩阵、正交矩阵、相似变换等）**
$$|A|=2,|B|=3,|A^{-1}+B|=2,求|A+B^{-1}|\\
|A+B^{-1}|=|EA+B^{-1}E|=|B^{-1}BA+B^{-1}A^{-1}A|=|B^{-1}(B+A^{-1})A|=|B^{-1}||B+A^{-1}||A|=\frac{4}{3}$$
**行列式运算的性质**
$$A=(\alpha,\alpha_1,\alpha_2,\alpha_3),B=(\beta,\alpha_1,\alpha_2,\alpha_3),|A|=1,|B|=-2,求|A+B|=|(\alpha+\beta,2\alpha_1,2\alpha_2,2\alpha_3)|\\
.....$$
**条件转化为矩阵关系，矩阵关系的计算（注意条件复用）**
$$A=(a_{ij})_{3\times 3}为非零矩阵,且a_{ij}+A_{ij}=0，求|A|\\
A=-(A^*)^T\Rightarrow |A|=-|A^*|\Rightarrow |A|=-|A|^2\\
|A|=a_{11}A_{11}+a_{12}A_{12}+a_{13}A_{13}=-(a_{11}^2+a_{12}^2+a_{13}^2)\neq0$$

# 矩阵

## 考情分析

矩阵知识点较繁杂，灵活性很高，考查重难点
矩阵相乘性质良好，矩阵相加性质很差，为考查难点

## 可逆矩阵的定义

$$设A,B是\textbf{n阶矩阵}，若有AB=BA=E，则称A,B互逆$$
$$注：A,B均为方阵时：AB=E\Leftrightarrow BA=E$$

## 等价矩阵

$$\quad\ A,B同型，且r(A)=r(B)\\
\Leftrightarrow 存在可逆方阵P,Q，使B=PAQ$$
$$注：任意两个等价矩阵均可通过初等变换转化$$

## 矩阵的等价标准型

$$\left[\begin{array}{}E_r&O\\O&O\end{array}\right],\quad \left[\begin{array}{}E_r&O\end{array}\right],\quad \left[\begin{array}{}E_r\\O\end{array}\right]$$
$$注：任意矩阵均可经初等变换转化为等价标准型$$

## 重要矩阵性质

$$AB=O\not\Leftrightarrow BA=O$$

## 几种重要矩阵

$$数量矩阵：kE\\
反对称矩阵：A^{T}=-A\quad(a_{ii}=0)$$

## 矩阵的秩

$$r(A)=k\\
\Leftrightarrow 存在k阶子式不为0，k+1阶子式全为0\\
\Leftrightarrow 最大线性无关组向量个数$$
$$注：
在行阶梯型下讨论非零行数（每台阶只能有一行）
$$

## 施密特正交化

$$\beta_1=\alpha_1$$
$$\beta_2=\alpha_2-\frac{(\alpha_2,\beta_1)}{(\beta_1,\beta_1)}\beta_1\qquad(\alpha_2-\frac{|\alpha_2||\beta_1|\cos\theta}{|\beta_1||\beta_1|}\beta_1=a_2-\underbrace{|\alpha_2|\cos\theta}_{\alpha_2投影长度}\cdot\underbrace{\frac{\beta_1}{|\beta_1|}}_{单位化\beta_1})$$
$$\beta_3=\alpha_3-\frac{(\alpha_3,\beta_1)}{(\beta_1,\beta_1)}\beta_1-\frac{(\alpha_3,\beta_2)}{(\beta_2,\beta_2)}\beta_2$$

## 矩阵的运算

$$分配律：A(B\pm C)=AB\pm AC;\\
 结合律：A(BC)=(AB)C$$
**四大运算可交换**
$$\begin{array}{}
({A^*})^{-1}=({A^{-1}})^{*} & ({A^*})^{T}=(A^{T})^{*} & ({A^{T}})^{-1}=({A^{-1}})^{T}\\
(A^k)^T=(A^T)^k & (A^k)^{-1}=(A^{-1})^k & (A^k)^*=(A^*)^k

\end{array}\quad（k为正整数）$$
**三大运算“乘法倒序”**
$$\begin{array}{}(AB)^{-1}=B^{-1}A^{-1}\quad(AB)^{T}=B^{T}A^{T}\quad(AB)^{*}=B^{*}A^{*}
\end{array}$$
$$(kA)^T=kA^T,\\
 (kA)^n=k^nA^n\\
AuBkC=ukABC（系数可任意改变位置）$$

## 逆矩阵与伴随矩阵

$$逆矩阵（A,B均为方阵）：AB=E\quad(A=B^{-1},B=A^{-1})$$
$$(kA)^{-1}=\frac{1}{k}A^{-1}\quad\quad
|A^{-1}|=|A|^{-1}\\

性质：\\
A可逆\Leftrightarrow A^{-1},A^*,A^T可逆

$$

$$伴随矩阵（方阵）：AA^{*}=A^{*}A=|A|E（拉普拉斯展开原理） $$
$$(kA)^*=k^{n-1}A^*\quad \quad |A^*|=|A|^{n-1}\quad \quad (A^*)^*=|A|^{n-2}A\quad$$
$$|A|\neq0时，A^*=|A|A^{-1}$$

## 逆矩阵与伴随矩阵的等价结论

$$r(A)=n\Leftrightarrow |A|\neq0\Leftrightarrow |A^*|=|A|^{n-1}\neq0\Leftrightarrow r(A^*)=n$$
$$\begin{array}{l l}
r(A)=n-1&\Leftrightarrow |A|=0且A中至少有一个n-1阶子式不为零\\
&\Leftrightarrow AA^*=|A|E=O且存在A_{ij}\neq0\\
&\Leftrightarrow r(A)+r(A^*)= n且A^*\neq O\\
&\Leftrightarrow r(A^*)=1

\end{array}$$
$$\begin{array}{ll}r(A)<n-1&\Leftrightarrow A的任意n-1阶子式全为零\\
&\Leftrightarrow A^*的所有元素A_{ij}=0\\
&\Leftrightarrow A^*=O\\
&\Leftrightarrow r(A^*)=0

\end{array}$$
$$r(A^*)=n\Leftrightarrow r(A)=n;\\
r(A^*)=1\Leftrightarrow r(A)=n-1;\\
r(A^*)=0\Leftrightarrow r(A)<n-1\\
（按定义理解）$$

## 三大初等变换
$$E_{ij},\quad E_{i}(k),\quad E_{ij}(k)$$

**左乘行变换，右乘列变换，下标由“近往远读”**
$$\begin{array}{lll}E_{ij}：互换\quad &[E_{ij}]^{-1}=E_{ij}\qquad &|E_{ij}|=-1\\

E_{i}(k):倍乘\quad &[E_{i}(k)]^{-1}=E_{i}(\frac{1}{k})\qquad &|E_i(k)|=k\\

 E_{ij}(k)：倍加\quad &[ E_{ij}(k)]^{-1}= E_{ij}(-k)\qquad &|E_{ij}(k)|=1
\end{array}$$
$$注：j行k倍加到i行，i列k倍加到j列$$

## 分块矩阵初等变换

**行变换左乘分块、列变换右乘分块**
**前提，行列对应**
$$\left(
\begin{array}{}
E_m&O\\
\\
G&E_n
\end{array}
\right)
\left(
\begin{array}{}
A&B\\
\\
C&D
\end{array}
\right)=
\left(
\begin{array}{}
A&B\\
\\
GA+C&GB+D
\end{array}
\right)$$
$$\left(
\begin{array}{}
P&O\\
\\
O&E
\end{array}
\right)\left(
\begin{array}{}
A&B\\
\\
C&D
\end{array}
\right)=
\left(
\begin{array}{}
PA&PB\\
\\
C&D
\end{array}
\right)（P不可逆也成立，但非初等变换）$$
$$\left(
\begin{array}{}
O&E_n\\
\\
E_m&O
\end{array}
\right)\left(
\begin{array}{}
A&B\\
\\
C&D
\end{array}
\right)=
\left(
\begin{array}{}
C&D\\
\\
A&B
\end{array}
\right)$$
$$舒尔公式（理解灵活使用）：\left(\begin{array}{}
E&O\\
-CA^{-1}&E
\end{array}\right)
\left(\begin{array}{}
A&B\\
C&D
\end{array}\right)=

\left(\begin{array}{}
A&B\\
O&D-CA^{-1}B
\end{array}\right)\\
$$
$$行列式与一般初等变换同理：
\left|
\begin{array}{}
E_m&O\\
\\
G&E_n
\end{array}
\right|,\left|
\begin{array}{}
P&O\\
\\
O&E
\end{array}
\right|,
\left|
\begin{array}{}
O&E_n\\
\\
E_m&O
\end{array}
\right|$$

## 分块矩阵的运算

$$\left(
\begin{array}{cc}
A&B\\
\\
C&D
\end{array}
\right)^T=
\left(
\begin{array}{cc}
A^T&C^T\\
\\
B^T&D^T
\end{array}
\right)$$
$$\left(
\begin{array}{ll}
B\\
\\
D&C
\end{array}
\right)^{-1}=
\left(
\begin{array}{cc}
B^{-1}\\
\\
-C^{-1}DB^{-1}&C^{-1}
\end{array}
\right)\quad\quad
\left(
\begin{array}{ll}
&B\\
\\
C&D
\end{array}
\right)^{-1}=
\left(
\begin{array}{cc}
-C^{-1}DB^{-1}&C^{-1}\\
\\
B^{-1}
\end{array}
\right)\\
（主、副对角仅位置不同，在相应位置上：负的，左乘行逆，右乘列逆）（其余分块同理）$$
$$\left(
\begin{array}{}
A_1\\
\\
&A_2\\
\\
&& \ddots\\
\\
&&&A_s
\end{array}
\right)^{-1}=
\left(
\begin{array}{}
A_1^{-1}\\
\\
&A_2^{-1}\\
\\
&& \ddots\\
\\
&&&A_s^{-1}
\end{array}
\right)\quad\quad
\left(
\begin{array}{}
&&&A_1\\
\\
&&A_2\\
\\
& \dots\\
\\
A_s
\end{array}
\right)^{-1}=
\left(
\begin{array}{}
&&&A_s^{-1}\\
\\
&&\dots\\
\\
& A_2^{-1}\\
\\
A_1^{-1}
\end{array}
\right)$$

## 分块矩阵的秩

$$r\left(\begin{array}{ll}A\\
\\
&B  \end{array}\right)=r(A)+r(B);\\
r\left(\begin{array}{ll}A\\
\\
C&B  \end{array}\right)= r(A)+r(B)（A列满秩或B行满秩时）\\
（按A,B极大线性无关组线性表出C把握）\\
r\left(\begin{array}{ll}A&D\\
\\
C&B  \end{array}\right)\xrightarrow{无关} r\left(\begin{array}{ll}A\\
\\
C&B  \end{array}\right)\geqslant r\left(\begin{array}{ll}A\\
\\
&B  \end{array}\right)=r(A)+r(B)\\（其余二维上下三角分块阵同理，无零分块则无以上结论）\\
$$

## 秩的性质1

$$\begin{array}{ll}A=0\Leftrightarrow r(A)=0;\quad A\neq0\Leftrightarrow r(A)\geqslant 1\\
r(A_{m\times n})\leqslant \min\{m,n\}
\end{array}$$
$$\begin{array}{ll}
|r(A)-r(B)|\leqslant r(\alpha A+ \beta B)\leqslant r([A, B])\leqslant r(A)+r(B)（线性表出理解）\\
\\
 r(A)+r(B)-n\leqslant r(A_{m\times n}B_{n\times s})\leqslant \min\{r(A),r(B)\}（矩阵的秩，越乘越小）;\\
 r(AB)= r(A),r(B)（左乘列满秩，或右乘行满秩，包括可逆矩阵）\\
\\
r([A,B])\geqslant \max\{r(A),r(B)\}（矩阵的秩，越拼越大）\\
\\
A_{m\times n}B_{n\times s}=O\Rightarrow \left\{
\begin{array}{l}
B的列向量都是方程组Ax=0的解\\
r(A)+r(B)\leqslant n
\end{array}
\right.
\end{array}\\
\ \\
n阶矩阵满足A^2-(k_1+k_2)A+k_1k_2E=O,\ k_1\neq k_2，则r(A-k_1E)+r(A-k_2E)=n$$

## 秩的性质2

$$存在一个k阶子式\neq0 \Rightarrow r(A)\geqslant k$$
$$A_{n\times n}可逆\Leftrightarrow |A|\neq0\Leftrightarrow r(A)=n\Leftrightarrow A为非奇异矩阵$$
$$A^k=O\Rightarrow |A|=0（初等矩阵不改变秩）\\
A,B均为n阶方阵，AB满秩\Leftrightarrow A,B满秩（可推广）$$

## 迹的性质

$$tr(A)=\sum_{i=1}^{n}a_{ii}=\sum_{i=1}^{n}\lambda_{i}=a_{11}+a_{22}+\cdots a_{nn}=\lambda_1+\lambda_2+\cdots \lambda_n（相似不变性，与能否相似对角化无关）$$
$$tr(ABC)=tr(BCA),\quad tr(ABC)\neq tr(ACB)（循环变序性）$$
$$tr(\alpha A+ \beta B)=\alpha\ tr(A)+ \beta\ tr(B)（线性叠加性）$$
$$tr(A^T)=tr(A)$$
$$若r(A)=1，即A=\alpha\ \beta^T（列乘行），则\\
\quad\quad tr(A)=\alpha^T\beta=\lambda（其余特征值为0）\\
\quad\quad A^n=\lambda^{n-1}A
$$

## 矩阵重要经验

$$1.\ A_{ij},\ A^*,\ A^{-1}密不可分,常以其间关系出题\\
2.\ 满足AB=BA的情形不止AB=E，如A,B为对角矩阵、零矩阵等等$$

## 讨论|A|=0常用方法

$$1.\ r(A)<n\\
2.\ Ax=0有非零解\\
3.\ |A|=\lambda_1\lambda_2\cdots \lambda_n$$

## 具体型矩阵含参数讨论秩问题

$$1.初等变换（主要方法）\\
注意灵活，初等行变换，转置后初等行变换均可，调整向量顺序\\
\\
非齐次方程组(A,b)中，可灵活调整A列向量顺序，方便变换\\
\ \\
2.借助行列式$$
$$注：\lambda+2任意用，\frac{1}{\lambda+2}仅在分类讨论后用$$

## 抽象逆矩阵求解

$$1.长除法因式分解求逆\\
\quad A^2+A=2E,求(A+3E)^{-1}\\
\quad\frac{A^2+A-2E}{A+3E}(整商)+aE(余数)=O
$$
$$2.矩阵关系推导\\
善用单位矩阵E拆解构造定义（可逆矩阵、正交矩阵、相似变换等）\\
A,B,A+B均可逆，证A^{-1}+B^{-1}可逆\quad
\rightarrow A^{-1}+B^{-1}=A^{-1}(B+A)B^{-1}\\
\ \\
观察矩阵形式，灵活乘相关矩阵进行消除\\
例：A,E-A均可逆，[E-(E-A)^{-1}]B=A，求B-A\\
[E-A](E-(E-A)^{-1})B=A-A^2\\
\ B-AB-B=A-A^2\rightarrow\ -AB=A-A^2\rightarrow\ B-A=-E$$

## 抽象矩阵证明可逆

**行列式、方程组仅有零解等：**
$$分块矩阵（初等变换化分块对角，行列式不为0）\\
题设出现行列式信息

$$
[Card#ID/22D7A#抽象逆矩阵求解]

## 逆矩阵计算

$$1.A^{-1}=\frac{A^*}{|A|}（适用低阶，二阶A^*：主对角互换，副对角添负号）$$
$$2.(A:E)\rightarrow(E:A^{-1})（E起记录作用）$$
$$3.初等矩阵拆解、分块矩阵求逆$$
$$特殊技巧：\\
(A^{-1}-E)^{-1}\rightarrow((E-A)A^{-1})^{-1}\rightarrow A(E-A)^{-1}$$

## 矩阵A的n次方计算

$$1. 数学归纳法情形：由低到高寻找规律$$
$$2.A=
\left(
\begin{array}{ccc}
\lambda&a&b\\
\\
&\lambda&c\\
\\
&&\lambda
\end{array}
\right)=
\underbrace{\left(
\begin{array}{ccc}
0&a&b\\
\\
&0&c\\
\\
&&0
\end{array}
\right)}_{B}+
\underbrace{\left(
\begin{array}{ccc}
\lambda&&\\
\\
&\lambda&\\
\\
&&\lambda
\end{array}
\right)}_{\lambda E}\\
\quad \quad B^3=O（n维同型矩阵n次方为O）$$
$$3.  r(A)=1\Rightarrow A=\alpha\ \beta^T（列乘行）\\
\quad\quad A^n=(trA)^{n-1}A$$
$$4.灵活运用相似变换、初等变换、矩阵运算等$$

## 矩阵方程问题

$$矩阵可逆：灵活使用矩阵关系提取X\\
AX=B,XA=B,AXB=C\\
\Rightarrow X=A^{-1}B,X=BA^{-1},X=A^{-1}CB^{-1}$$
$$A,B不可逆：AX=B（增广矩阵解非齐次方程组问题，X不唯一）$$

# 向量组与线性方程组

## 考情分析

难点：向量组的相关性证明

## 常用结论

$$初等行变换，不改变列相关性\\
初等列变换，不改变行相关性\\
（一般变换可能改变）$$
$$增加k行（列），秩最多增加k$$

## 相关性与线性表出重要结论

$$相关的向量组加向量仍相关\\
无关的向量组减向量仍无关$$
$$相关的向量组减分量仍相关\\
无关的向量组加分量仍无关$$
$$一个向量相关\Leftrightarrow零向量\\
两个向量相关\Leftrightarrow成比例$$
$$若n维向量组\alpha_1,\alpha_2,\cdots,\alpha_k线性无关，\alpha_{k+1}=\lambda_1\alpha_1+\lambda_2\alpha_2+\cdots+\lambda_k\alpha_k(\lambda_i\neq0,i=1,2,\cdots,k)\\
则\alpha_1,\alpha_2,\cdots,\alpha_k,\alpha_{k+1}中任意小于k个向量都线性无关$$

## 极大线性无关组求解

$$极大线性无关组选取规则：\\
列长逐小至大选取向量(1,2,3\cdots)，缺项需整理，满足逐小至大(1,2,3\cdots)\\
1.习惯上选取行阶梯型下的台角向量\\
2.逐小至大(1,2,3\cdots)，列长相同者地位等同，可自由替换

$$

## 线性相关与齐次解

$$\quad\ k_1\alpha_1+k_2\alpha_2+\cdots+k_s\alpha_s=0（探讨k是否全为零）\\
\Leftrightarrow \alpha_1,\alpha_2,\cdots,\alpha_m中存在向量是其余向量的线性组合$$
$$列向量组(\alpha_1,\alpha_2,\cdots,\alpha_s)线性无关\Leftrightarrow 齐次线性方程组(\alpha_1,\alpha_2,\cdots,\alpha_s)\left(\substack{x_1\\ x_2\\ \vdots\\ x_s}\right)=0只有零解\Leftrightarrow r(\alpha_1,\alpha_2,\cdots,\alpha_s)=s$$

## 线性表出与非齐次解

$$k_1\alpha_1+k_2\alpha_2+\cdots+k_s\alpha_s=\beta（探讨k是否存在）\\
（若\beta\neq0，则k一定不全为零）$$
$$\beta可由(\alpha_1,\alpha_2,\cdots,\alpha_s)表示\Leftrightarrow 非齐次线性方程组(\alpha_1,\alpha_2,\cdots,\alpha_s)\left(\substack{x_1\\ x_2\\ \vdots\\ x_s}\right)=\beta有解\Leftrightarrow r(\alpha_1,\alpha_2,\cdots,\alpha_s)=r(\alpha_1,\alpha_2,\cdots,\alpha_s,\beta)\\
表示法唯一（唯一解）\Leftrightarrow \alpha_1,\alpha_2,\cdots,\alpha_s线性无关$$

## 线性方程组解的性质

$$全部解的构成：齐次通解+非齐次特解\\
（非齐次通解中，除去含k项，即为“非齐次特解因子”）$$
$$基础解系不唯一，通解不唯一$$
**齐次解叠加性：**
$$y_1,y_2,y_3,\cdots,y_n为齐次解\\
k_1y_1+k_2y_2+\cdots+k_ny_n仍为齐次解$$
**非齐次解叠加性：**
$$y_1,y_2,y_3,\cdots,y_n为非齐次解\\
k_1y_1+k_2y_2+\cdots+k_ny_n\left\{
\begin{array}{ll}
\sum k_i=0,齐次解\\
\sum k_i=1,非齐次解
\end{array}
\right.$$
$$注：常系数线性微分方程与线性方程组性质相似，但不相同\\
常系数线性微分方程的非齐次解可以“模态”分解，线性方程组不可$$

## 线性方程组线性无关解个数

$$Ax=0齐次线性方程组的线性无关解个数为n-r(A)\\
\ \\
Ax=b非齐次线性方程组的线性无关解个数为n-r(A)+1$$
$$注：\\
1.非齐次特解必然无法被齐次通解的基础解系表示\\
（若可表示，代入方程组=0\quad\times ）\\
2.Ax=b组成增广矩阵(A,b)(b\neq0)，初等行变换后\overline{b}\neq0（故必有特解）$$

## 方程组解与秩的关系

$$\begin{array}{ll}
A_{m\times n}x=0（总有解）:&r(A)=n\quad只有零解\\
&r(A)<n\quad有无穷多解\\
\\
A_{m\times n}x=b:&r(A)\neq r(A,b)\quad无解\\
&r(A)= r(A,b)=n\quad有唯一解\\
&r(A)= r(A,b)<n\quad有无穷多解
\end{array}$$

## 相关性与线性表出的关系

$$同：\\
线性表出可转换为线性相关性问题$$
$$异：\\
AQ=B, 且Q可逆,则\\A与B有相同的行相关性，但A,B的列向量组等价，即可互相线性表出$$

## 方程组同解与公共解

**同解与公共解属不同概念**
$$同解：解互相满足（A的解是B的解（不含k_i代入成立），且r(A)=r(B)）\\
系数矩阵行向量等价，两方程组的基础解系向量组等价$$
$$公共解：解系空间有公共部分（寻求k_i的关系）\\
两方程组的基础解系向量组均可表示某向量空间的同一向量组$$

## 向量组等价与同解方程组性质

**向量组等价（列）== 同解方程组（行）**
$$\quad\ A,B的向量组可互相线性表出\\
\Leftrightarrow r(A)=r(B)，且A,B的向量组可单方向线性表出\\
\Leftrightarrow r(A)=r(B)=r(A,B)\\
$$
$$\quad\ Ax=0的解满足Bx=0，且Bx=0的解满足Ax=0\\
\Leftrightarrow r(A)=r(B)，且Ax=0的解满足Bx=0（或Bx=0的解满足Ax=0）\\
\Leftrightarrow r(A)=r(B)=r\left(\begin{array}{}A\\B\end{array}\right)\\
\Leftrightarrow 存在P,Q,使PA=B,QB=A\\
\Leftrightarrow存在可逆矩阵P，使PA_{m\times s}=\left(\begin{array}{}B_{n\times s}\\O\end{array}\right)(m\geqslant n) \\
\Leftrightarrow Q为列满秩矩阵且B=QA\quad（不同型,r(A)=r(B),且Ax=0的解满足QAx=0）\\
\qquad A_{m\times s}=P^{-1}\left(\begin{array}{}B_{n\times s}\\O\end{array}\right)=QB\quad(m\geqslant n) （Q相当于P^{-1}去掉后m-n列）$$
$$注：同型即初等行变换，不同型则左乘列满秩\\
\begin{array}{rcl}
初等变换&\Leftrightarrow& 同解且同型\\
左乘列满秩&\Leftrightarrow&同解但不一定同型\end{array}$$

## 齐次线性方程组同解、子解的性质

$$\underbrace{Ax=0}_{\textcircled{1}}与\underbrace{A^TAx=0}_{\textcircled{2}}同解\qquad r(A)=r(A^T)=r(AA^T)=r(A^T A)\\
\ \\
\textcircled{1}的解是\textcircled{2}的解\qquad 显然\\
\textcircled{2}的解是\textcircled{1}的解\qquad(Ax)^TAx=0\xRightarrow{平方和为零} Ax=0\\
\ \\
注：Ax=0与AA^Tx=0不一定同解$$
$$\quad\ Ax=0的解都是Bx=0的解\\
\Leftrightarrow Ax=0与\left\{\begin{array}{l}
Ax=0\\
Bx=0
\end{array}
\right.同解\\
\Leftrightarrow A的行向量组可线性表示B的行向量组\\
\Leftrightarrow r(A)=r\left(\begin{array}{l}A\\B\end{array}\right)\\
\Leftrightarrow 存在P，使得PA=B\\
\ \substack{\Rightarrow \\ \not\Leftarrow}\ r(A)\geqslant r(B)
\quad （向量空间不一定一致）$$

## 非齐次线性方程组同解、子解性质

**前提，非齐次线性方程组有解**
$$\quad\ Ax=\alpha的解满足Bx=\beta，且Bx=\beta的解满足Ax=\alpha\quad（齐次通解相同+非齐次特解相同）\\
\Leftrightarrow \left(\begin{array}{}A&\alpha\end{array}\right) \left(\begin{array}{}x\\-1\end{array}\right)=0与\left(\begin{array}{}B&\beta\end{array}\right)\left(\begin{array}{}x\\-1\end{array}\right)=0同解\\
\Leftrightarrow r(A)=r(B)=r(A,\alpha)=r(B,\beta)=r\left(\begin{array}{}A\\B\end{array}\right)=r\left(\begin{array}{}A&\alpha\\B&\beta\end{array}\right)\\
\Leftrightarrow存在可逆矩阵P，使P\left(A_{m\times s}\quad\alpha\right)=\left(\begin{array}{}B_{n\times s}&\beta\\O&O\end{array}\right)(m\geqslant n)，非齐次有解\\
\substack{\Rightarrow\\ \not\Leftarrow}\ Ax=0与Bx=0同解$$
$$\quad\ Ax=\alpha的解都是Bx=\beta的解\\
\Leftrightarrow Ax=\alpha与\left\{\begin{array}{l}
Ax=\alpha\\
Bx=\beta
\end{array}
\right.同解\\
\Leftrightarrow (A\quad\alpha)的行向量组可线性表示(B\quad\beta)的行向量组，且非齐次有解\\
\Leftrightarrow r(A\quad\alpha)=r\left(\begin{array}{}A&\alpha\\
B&\beta\end{array}\right)，且r(A)=r(A\quad\alpha)，r(B)=r(B,\beta)$$

## 向量空间

**标准正交基：**单位向量、正交向量组
**过渡矩阵： **熟练使用逆矩阵变换即可
$$(\beta_1,\beta_2,\cdots,\beta_n)=(\alpha_1,\alpha_2,\cdots,\alpha_n)P\\
P=(\alpha_1,\alpha_2,\cdots,\alpha_n)^{-1}(\beta_1,\beta_2,\cdots,\beta_n)$$
**向量坐标：**
$$\\(\beta_1,\beta_2,\cdots,\beta_n)y=(\alpha_1,\alpha_2,\cdots,\alpha_n)x \quad \Rightarrow \quad  x=Py（坐标变换均为此形式）$$
**善用向量空间理解把握相关性与线性表出相关性质**
$$注：向量个数小于向量维数，即向量空间不同时......\\
\left(\begin{array}{}
1&0\\
1&1\\
0&1
\end{array}
\right)\not\Leftrightarrow
\left(\begin{array}{}
0&0\\
1&0\\
0&1
\end{array}
\right)$$

## 向量组与方程组重要经验

$$1.相关、无关问题，先标明矩阵维数，再作讨论\\
2.初等变换讨论向量组线性表出、等价问题时，切记列为增广矩阵同时变换$$

## 求基础解系
初等变换法、n-r(A)个线性无关解

**初等变换法：......**
$$令自由变量\\\xi_1=\left(
\begin{array}{}
\vdots\\
x_3\\
x_4
\end{array}
\right)=
\left(
\begin{array}{}
\vdots\\
0\\
1
\end{array}
\right)（配平方程）\\
\xi_2=\left(
\begin{array}{}
\vdots\\
x_3\\
x_4
\end{array}
\right)=
\left(
\begin{array}{}
\vdots\\
1\\
0
\end{array}
\right)（配平方程）\\
齐次通解+非齐次特解\\
\ \\
注：可选不同的自由变量，故基础解系不唯一，其向量组等价$$
**n-r(A)个线性无关解: ......**

## 基础解系重要结论

$$定义：\\
1.\xi_1,\xi_2,\cdots,\xi_r均为齐次线性方程组的解\\
2.\xi_1,\xi_2,\cdots,\xi_r为Ax=0全部解的极大线性无关组$$
$$灵活从基础解系中反得列向量相关性\\
\xi=\left(
\begin{array}{}
1\\2\\-1\\0
\end{array}
\right)\Rightarrow \alpha_1+2\alpha_2-\alpha_3=0;\quad\xi=\left(
\begin{array}{}
1\\0\\1\\0
\end{array}
\right)\Rightarrow \alpha_1+\alpha_2=0（地位等同）$$
$$注：
\left.\begin{array}{l}
基础解系\rightarrow列向量的线性相关性\\
列向量的线性相关性\rightarrow基础解系
\end{array}\right\}不仅限于一维解系（灵活分析）$$

## 求公共解题型

**方程组均已知：**
$$联立求解即可$$
**一个方程组已知，另一个基础解系已知：**
$$\xi=(k_1\alpha_1+k_2\alpha_2)代入方程组，根据方程组存在非零解，确定k_i间的关系$$
**方程组未知，已知基础解系：**
$$（关键在于寻找k_1,k_2,l_1,l_2间的关系）\\
设公共解为：\\
\gamma=k_1\beta_1+k_2\beta_2=l_1\alpha_1+l_2\alpha_2\\
\Rightarrow k_1\beta_1+k_2\beta_2-l_1\alpha_1-l_2\alpha_2=0\\
解齐次方程组：\\
(\beta_1,\beta_2,-\alpha_1,-\alpha_2)\left(
\begin{array}{l}
k_1\\k_2\\l_1\\l_2
\end{array}
\right)=0\quad 用k_1,k_2或l_1,l_2表示公共解\gamma\\
(k_1,k_2,l_1,l_2)^T=c_1(4,-3,1,0)^T+c_2(-7,5,0,1)^T\\
\xi=(4c_1-7c_2)\alpha_1+(-3c_1+5c_2)\alpha_2=-c_1\beta_1-c_2\beta_2\quad{\color{blue}本质为四维向量张成二维向量空间}\\
\quad=c_1(4\alpha_1-3\alpha_2)+c_2(-7\alpha_1+5\alpha_2)$$

## ⭐️判定向量组线性无关题型

$$1.定义法（常规方法失效时考虑）：
k_1\alpha_1+k_2\alpha_2+\cdots+k_n\alpha_n=0（是否存在k_i全为0）
$$
$$相乘消k_i项（关键：找到相乘的矩阵、或向量）\\
例1：A\alpha_1=\alpha_1\neq0,A\alpha_2=\alpha_1+\alpha_2,A\alpha_3=\alpha_2+\alpha_3，证\alpha_1,\alpha_2,\alpha_3线性无关\\
\rightarrow (A-E)\alpha_1=0,(A-E)\alpha_2=\alpha_1,(A-E)\alpha_3=\alpha_2\\
循环相乘，或因子相乘(A+E,A-E,\cdots)\\
例2：A为n阶正定，\alpha_1,\alpha_2,\cdots, \alpha_r为n维非零向量，且\alpha_i^TA\alpha_j=0(i\neq j)，证\alpha_1,\alpha_2,\cdots,\alpha_r线性无关\\
\rightarrow\alpha_i^TA逐个相乘k_1\alpha_1+k_2\alpha_2+\cdots+k_n\alpha_n=0解k_i\\
\ \\
组合代入解k_i，线性变换表示，判定秩\\
例：\alpha_1,\alpha_2,\alpha_3线性无关，\beta_1=\alpha_1+\alpha_2,\beta_2=\alpha_1-\alpha_2,\beta_3=\alpha_3

$$
$$2.初等变换、行列式等（有秩、行列式等相关信息时考虑）:$$
$$已知\beta=\alpha_1+\alpha_2+\cdots+\alpha_m，\\
证\beta-\alpha_1,\beta-\alpha_2,\cdots,\beta-\alpha_m线性无关的充分必要条件是\alpha_1,\alpha_2,\cdots,\alpha_m线性无关\\
（构建初等变换关系）$$

## 几何意义题型

$$直线几何关系判定：\\
直线\frac{x-a_3}{a_1-a_2}=\frac{y-b_3}{b_1-b_2}=\frac{z-c_3}{c_1-c_2}与直线\frac{x-a_1}{a_2-a_3}=\frac{y-b_1}{b_2-b_3}=\frac{z-c_1}{c_2-c_3}的关系，\left(
\begin{array}{ccc}
a_1&b_1&c_1\\
\\
a_2&b_2&c_2\\
\\
a_3&b_3&c_3
\end{array}
\right)满秩\\
\ \\
判定矩阵
\left(
\begin{array}{ccc}
a_1-a_2&b_1-b_2&c_1-c_2\\
\\
a_2-a_3&b_2-b_3&c_2-c_3\\
\\
a_3-a_1&b_3-b_1&c_3-c_1
\end{array}
\right)的秩r(A)=
\left\{\begin{array}{l}
3，不共面\\
2，共面（相交或平行）\\
1，重合
\end{array}\right.
$$
$$三维方程组的几何关系判定（抽象为平面，以法向量把握）：\\
r(A)=1,r(\overline{A})=1，r(\overline{A})=2（两种情形）\\
r(A)=2,r(\overline{A})=2（两种情形）,r(\overline{A})=3（两种情形）\\
r(A)=3,r(\overline{A})=3
$$

## 具体向量组的线性表出与等价题型

**向量组的线性表出：**
$$列为增广矩阵，初等行变换，化最简形讨论（齐次解+非齐次解两部分）\\
注：非齐次解用台角表示出即可，不唯一$$
**向量组等价（较灵活）：**
$$分等价的完全性与不完全性两类情形\\1.方阵满秩，即可逆\\
2.非满秩，根据r(A)=r(B)=r(A,B)判断\\
3.无法判断秩（含参），列为增广矩阵，初等行变换讨论（通用性强）\\
等价完全性讨论：增广矩阵可单向表出，且r(A)=r(B)

$$

## 同一向量不同基下相同坐标问题

$$思路：设坐标(k_1,k_2,k_3)，整理为齐次线性方程组\\
e=k_1\alpha_1+k_2\alpha_2+k_3\alpha_3=k_1\beta_1+k_2\beta_2+k_3\beta_3\\
(\beta_1-\alpha_1)k_1+(\beta_2-\alpha_2)k_2+(\beta_3-\alpha_3)k_3=0有非零解问题$$

## 已知基础解系，求方程组题型

$$\xi_1,\xi_2为基础解系，\alpha_1=k_1\xi_1+k_2\xi_2,\quad \alpha_2=k_3\xi_1+k_4\xi_2\\
A(\alpha_1,\alpha_2)=O\\
\underbrace{\left(
\begin{array}{l}
\alpha_1^T\\ \\ \alpha_2^T
\end{array}
\right)A^T=O}_{\textcircled{1}}\quad与\quad
\underbrace{\left(
\begin{array}{l}
\xi_1^T\\ \\ \xi_2^T
\end{array}
\right)A^T=O}_{\textcircled{2}}\quad 同解\\
\ \\
解线性方程组\textcircled{2}基础解系\zeta_1,\zeta_2\\
A^T=(l_1\zeta_1+l_2\zeta_2,\quad l_3\zeta_1+l_4\zeta_2)\qquad
\left|\begin{array}{}
l_1&l_3\\
l_2&l_4
\end{array}\right|\neq0$$

## 抽象型方程组求解

**关键：根据通解得向量关系**
$$A=(\alpha_1,\alpha_2,\alpha_3),Ax=\beta的通解为(1,2,-1)^T+k(1,-2,3)^T,\\令B=(\alpha_1,\alpha_2,\alpha_3,\alpha_3+\beta),则求Bx=\alpha_1-\alpha_2的通解\\
\ \\
\left\{
\begin{array}{l}
\alpha_1+2\alpha_2-\alpha_3=\beta\\
\alpha_1-2\alpha_2+3\alpha_3=0
\end{array}
\right.\\
\ \\
线性表出问题：\\
\left\{\begin{array}{l}(\alpha_1,\alpha_2,\alpha_3,\alpha_3+\beta)x=0\\
(\alpha_1,\alpha_2,\alpha_3,\alpha_3+\beta)x=\alpha_1-\alpha_2
\end{array}
\right.$$

# 特征值、特征向量

## 考情分析

难点：抽象矩阵的相似

## 特征值与特征向量的定义

$$设A为n阶矩阵，若存在n维非零列向量\xi，使得\\
\qquad\qquad\qquad A\xi=\lambda\xi\ 或{\color{blue} (A-\lambda E)\xi=0}\\
则称\lambda为A 的特征值，\xi是对应与特征值\lambda的特征向量$$
$$注：\\
A\xi=\lambda\xi意义：伸缩变换\\
\xi由(A-\lambda E)x=0解得，为基础解系，非定量(k\xi_i,k\neq0)\\
特征方程|A-\lambda E|=0可能出现非实根情况，但不作为考察点$$

## 特征值、特征向量与齐次方程组的概念互通

$$A对应\lambda_i的特征向量\xi_i是(A-\lambda_iE)x=0的非零基础解系$$

## 特征值、特征向量的性质

$$1. A的不同特征值对应的特征向量线性无关\\
2. k重特征值最多有k个线性无关的特征向量（代数重数\geqslant几何重数\geqslant1）\\
3. 不同特征值对应的特征向量的非零线性组合不是A 的特征向量\\
4.同一特征值对应的特征向量为k_1\xi_1+k_2\xi_2+\cdots（k_i不全为零）$$
$$\lambda为A,B的特征值\not\Rightarrow \lambda是A+B,AB的特征值\\
 \xi是A,B的特征向量，则必是多项式f(A)+g(B),f(A)g(B)的特征向量\\
\\
\ [f(A)+g(B)]\xi=[f(\lambda_A)+f(\lambda_B)]\xi \\
f(A)g(B)\xi=f(A)g(\lambda_B)\xi=f(\lambda_A)g(\lambda_B)\xi

$$

## 矩阵相似的定义

$$A,B为\textbf{n阶方阵}，若存在n阶可逆矩阵P，使得P^{-1}AP=B，则称A\sim B$$

## 可相似对角化的本质

$$(A\xi_1,A\xi_2,\cdots,A\xi_n)=(\lambda_1\xi_1,\lambda_2\xi_2,\cdots,\lambda_n\xi_n)\rightarrow AP=P\Lambda\\
\ \\
若P可逆，即(\xi_1,\xi_2,\cdots,\xi_n)线性无关，则有P^{-1}AP=\Lambda，故A可相似对角化$$
$$注：\\
1.(\xi_1,\xi_2,\cdots,\xi_n)中各向量长度任意\\
2.(\xi_1,\xi_2,\cdots,\xi_n)的排列与\Lambda中\lambda_1,\lambda_2,\cdots,\lambda_n排列对应$$

## 矩阵可相似对角化的五大条件

$$充要条件：\\
\Leftrightarrow 存在可逆矩阵P，使P^{-1}AP=\Lambda\\
\Leftrightarrow n阶矩阵A有n个线性无关的特征向量\\
\Leftrightarrow n阶矩阵A对应于每个k_i重特征值都有k_i个线性无关的特征向量\\
\Leftrightarrow n阶矩阵A特征值的几何重数等于代数重数$$
$$充分条件：\\
\Leftarrow n阶矩阵A有n个不同的特征值\\
\Leftarrow n阶矩阵A为实对称矩阵$$

## 特征值与特征向量对应
$$A,\quad kA,\quad A^k,\quad f(A),\quad A^{-1},\quad A^*,\quad P^{-1}AP,\quad A^T$$

$$\begin{array}{cccccccc}

矩阵&A&kA&A^k&f(A)&A^{-1}&A^*&P^{-1}AP&A^T\\
\\
特征值&\lambda&k\lambda&\lambda^k&f(\lambda)&\frac{1}{\lambda}&{\frac{|A|}{\lambda}(|A|\neq0)}&\lambda&\lambda\\
\\
特征向量&\xi&\xi&\xi&\xi&\xi&\xi&P^{-1}\xi&-&特征向量非定值k\xi(k\neq0)

\end{array}$$
$$P^{-1}AP,A^*（A可逆时）,A^{-1},kA,A可反得A的特征值、特征向量\\
{\color{blue}（涉及k次方无法反得，其余均可）}$$

## 相似的性质

**注意相似性质的递归拓展**
$$充要条件：\\
A\sim B\Leftrightarrow A^{-1}\sim B^{-1}(|A|\neq0时),\quad A^T\sim B^T,\quad A^*\sim B^*(|A|\neq0时),\quad {\color{blue}A-kE\sim B-kE,\quad kA\sim kB}$$
$$性质-必要不充分条件（相似反求参数用此即可）：\\
\Rightarrow r(A)=r(B),\quad |A|=|B|,\quad|A-\lambda E|=|B-\lambda E|,\quad A,B有相同的特征值,\quad tr(A)=tr(B)\\
\Rightarrow f(A)\sim f(B),\quad f(A^T)\sim f(B^T),\quad f(A^{-1})\sim f(B^{-1}),\quad  f(A^{*})\sim f(B^{*})\\
\ \\
注：P^{-1}AP=B\Longrightarrow B+B^{-1}=P^{-1}AP+P^{-1}A^{-1}P= P^{-1}(A+A^{-1})P
{\color{blue}（f仅为关于A,A^{-1}的多项式）}$$
$$性质：
A\sim C,B\sim D\Rightarrow \left(\begin{array}{}A&O\\O&B\end{array}\right)\sim \left(\begin{array}{}C&O\\O&D\end{array}\right)$$

## 相似矩阵判定的方法

**先考虑用相似的必要条件排除，再考虑以下方法**
$$1. 定义法：P^{-1}AP=B\\
2. 传递性质：A\sim B,A\sim C\Rightarrow B\sim C\\
\star A,B有相同的特征值\\
\left\{
\begin{array}{l}
A,B可相似对角化\Rightarrow A\sim B\\
A,B不可相似对角化，且r(A-\lambda E)=r(B-\lambda E)\Rightarrow A\sim B\\
（较深，几何重数、代数重数、约旦标准型证得）\\
A可相似对角化，B不可相似对角化\Rightarrow A\not\sim B\\
（传递性反证）
\end{array}
\right.$$

## 正交矩阵及其性质

$$定义：A为n阶方阵，A^TA=AA^T=E,则称A是正交矩阵$$
$$正交矩阵的列（行）均是两两正交的单位向量\\
即，A\left\{
\begin{array}{}
既为，标准行正交向量组\\
又为，标准列正交向量组
\end{array}
\right.$$
$$性质：\\
1.\ A^T=A^{-1}\\
2.\ |A|=\pm1\\
3.\ 特征值为\pm1\\
4.\ A^{-1},A^*,A^T,-A为正交矩阵\\
5.\ A,B正交\Rightarrow AB,BA为正交矩阵\\
(ABB^TA^T=E\quad BAA^TB^T=E)$$

## 实对称矩阵的定义与性质

$$定义:A为n阶方阵，矩阵元素为实数，且A=A^T$$
$$性质：\\
1.实对称矩阵不同特征值的特征向量互相正交\\
2.实对称矩阵k重特征值必有k个线性无关的特征向量，则必可相似对角化\\
3.“重”特征向量正交化，仍为特征向量，故可正交相似对角化\\
\ \\
4.实对称矩阵必可正交相似对角化，故特征值正负个数对应正负惯性指数\\
\ \\
5.实对称矩阵必有n个n维的特征向量，{\color{blue}满向量空间}\\
若向量与所有“异特征值”的特征向量正交，则此向量为特征向量\\
\ \\
实对称矩阵各大运算均对称：\\A^{-1}=(A^{-1})^T\quad A^*=(A^*)^T\quad A^{k}=(A^{k})^T\quad kA=kA^T$$
$$注：
实对称矩阵A=A^T内含所有性质，备选使用$$

## 分块矩阵特征值

$$\left|\begin{array}{}
A-\lambda E\\
\\
C&B-\lambda E  \end{array}\right|=|(A-\lambda E)(B-\lambda E)|=0\\
\lambda_i=\lambda_A,\lambda_B$$
$$\left|\begin{array}{}
-\lambda E&A\\
\\
A&-\lambda E \end{array}\right|=|(-\lambda E-A)(-\lambda E+A)|=|\lambda^2 E-A^2|=0\\
\lambda_i=\lambda_A,-\lambda_A$$
$$|A+\lambda E|=0\rightarrow |A-\mu E|=0；\mu为特征值，且\mu_i=-\lambda_i$$

## 重要经验

$$特征值、特征向量与齐次方程组的关系密切$$
$$非零特征值个数无法判断矩阵的秩，除非可相似对角化$$

## 特征行列式处理技巧

$$勿直接计算行列式，先观察，进行行列式运算，提取因子\\
行和、列和相等（加到一边），对称矩阵等\\
\left|
\begin{array}{}
1-\lambda&a&1\\
\\
a&b-\lambda&a\\
\\
1&a&1-\lambda
\end{array}
\right|$$

## 特征值计算技巧

$$A=
\left(
\begin{array}{}
3&2&2\\
\\
2&3&2\\
\\
2&2&3
\end{array}
\right)=
E+
\left(
\begin{array}{}
2&2&2\\
\\
2&2&2\\
\\
2&2&2
\end{array}
\right)=E+B\\
\qquad\qquad\qquad\qquad\qquad\Rightarrow\lambda=1+tr(B)=1+6=7$$
$$此法可推广应用：由特征值计算行列式$$

## 正交相似对角化

$$正交化技巧：\\A-\lambda E有二重根，
（前提是配平方程）：\\
x_1=-2x_2+2x_3\\
\xi_1=\left(
\begin{array}{}
-2\\
\\
1\\
\\
0
\end{array}
\right)\qquad
\xi_2=\left(
\begin{array}{}
1\\
\\
2\\
\\
{\color{blue}\frac{5}{2}}
\end{array}
\right)前两元素配正交，后一元素配平$$
$$注：\\
特征向量正交化后依旧是矩阵的特征向量\\
\ \\
相似变换阵向量长度、重特征向量方向不唯一\\
正交变换阵仅重特征向量方向不唯一（单位向量）$$

## 矩阵多项式等式重要处理技巧

$$若有f(A)=O,则有f(\lambda)=0{\color{blue}（f仅为关于A,A^{-1},A^*在内的多项式）},可得A特征值的可能取值（不一定各值均可取到）\\
注：(A+A^*+A^{-1})\xi=(\lambda+\frac{|A|}{\lambda}+\frac{1}{\lambda})\xi=0\xRightarrow{\xi\neq0} (\lambda+\frac{|A|}{\lambda}+\frac{1}{\lambda})=0$$
$$若有f(A)\alpha=0(\alpha,A\alpha线性无关),可分解f(A)因式,由特征值与特征向量定义分析条件\\
例：A^2\alpha+A\alpha=0\\
\left\{
\begin{array}{l}
A(A\alpha+\alpha)=0\cdot (A\alpha+\alpha) \\
(A+E)A\alpha=0\cdot A\alpha\\
（保证A\alpha,A\alpha+\alpha非零）
\end{array}
\right.\Rightarrow
\left\{
\begin{array}{l}
|A|=0\\
|A+E|=0
\end{array}
\right.$$

## 相似对角化特例

$$n阶矩阵满足A^2-(k_1+k_2)A+k_1k_2A=O,\ k_1\neq k_2，则A可相似对角化$$
$$\Rightarrow \lambda_i可能的取值为k_1,k_2（k_1,k_2不一定均能取到）\\\\
(A-k_1E)(A-k_2E)=O\\
\Rightarrow n=r[(k_2-k_1)E]\leqslant r(A-k_1E)+r(A-k_2E)\leqslant n\\
即 r(A-k_1E)+r(A-k_2E)=n\\
\ \\
讨论\lambda=k_1情形:
n-r(A-k_1E)=r(A-k_2E)\\
讨论\lambda=k_2情形:
n-r(A-k_2E)=r(A-k_1E)\\
\Rightarrow
r(A-k_1E)+r(A-k_2E)=n，故有n个线性无关的特征向量$$

$$r(A)=1且tr(A)\neq0，则A可相似对角化，且\lambda=tr(A)$$
[Card#ID/28V5V#秩为1的矩阵求特征向量]

## 求相似矩阵

$$两种思路：\\
AP=PB（寻求表示关系）\\
B=P^{-1}AP（须求P^{-1}，可能较繁琐）$$

## 实对称矩阵求解特征向量

**关键：实对称矩阵不同特征值对应的特征向量正交**
$$已知“单”特征向量，求“重”特征向量:\\
\zeta_1,\zeta_2为单特征向量\left\{
\begin{array}{l}(x_1,x_2,x_3,x_4)\zeta_1=0\\
(x_1,x_2,x_3,x_4)\zeta_2=0
\end{array}
\right.解方程组，即可解得“重”特征向量\\
\ \\
已知“重”特征向量，求“单”特征向量:\\
\xi_1,\xi_2为重特征向量组\left\{
\begin{array}{l}(x_1,x_2,x_3)\xi_1=0\\
(x_1,x_2,x_3)\xi_2=0
\end{array}
\right.解方程组，即可解得“单”特征向量
$$

## 秩为1的矩阵求特征向量

![](pic-linear-algebra\Markji_1751360044319.png)
![](pic-linear-algebra\Markji_1751360051395.png)
![](pic-linear-algebra\Markji_1751360060112.png)
![](pic-linear-algebra\Markji_1751360067205.png)
![](pic-linear-algebra\Markji_1751360073729.png)

# 二次型

## 考情分析

矩阵合同主要考二次型的合同，即实对称矩阵的合同

## 二次型矩阵

$$规定二次型的矩阵必须是A=A^T，故二次型的矩阵唯一\\
实对称矩阵必可正交相似对角化$$

## 坐标变换的灵活运用

$$f=2(a_1x_1+a_2x_2+a_3x_3)^2+(b_1x_1+b_2x_2+b_3x_3)^2\\

\quad=2(x_1,x_2,x_3)
\left(\begin{array}{l}a_1\\a_2\\a_3
\end{array}\right)(a_1,a_2,a_3)
\left(\begin{array}{l}x_1\\x_2\\x_3
\end{array}\right)+(x_1,x_2,x_3)\left(\begin{array}{l}b_1\\b_2\\b_3\end{array}\right)(b_1,b_2,b_3)\left(\begin{array}{l}x_1\\x_2\\x_3\end{array}\right)\\
\quad=x^T(2\alpha\alpha^T+\beta\beta^T)x$$

$$正交变换下(P^TP=E,P=(e_1,e_2,e_3)):\\
f=x^TAx=y^TP^TA Py=y^T\Lambda y=y^T\left(\begin{array}{}2&&\\&1&\\&&-1\end{array}\right)y=2y_1^2+y_2^2-y_3^2\\
f在正交变换x=Qy=(e_1,-e_3,e_2)y下为\\
x=Qy=P\left(\begin{array}{}1&&\\&&1\\&-1&\end{array}\right)y=P\left(\begin{array}{}y_1\\y_3\\-y_2\end{array}\right)\\
故f=(y_1,y_3,-y_2)
\left(\begin{array}{}2&&\\&1&\\&&-1\end{array}\right)\left(\begin{array}{}y_1\\y_3\\-y_2\end{array}\right)$$

## 矩阵合同的定义

$$A,B为\textbf{n阶方阵}，若存在n阶\textbf{可逆矩阵C}，使得C^TAC=B，则称A与B合同，记为A\simeq B$$

## 正负惯性指数

$$合同变换化为标准型或规范型，正项个数为正惯性指数，负项个数为负惯性指数$$

## 二次型最值问题

$$\lambda_{\min}(y_1^2+y_2^2+\cdots+y_n^2)\leqslant x^TAx\leqslant \lambda_{\max}(y_1^2+y_2^2+\cdots+y_n^2)\\
故M\lambda_{\min}\leqslant x^TAx\leqslant M\lambda_{\max}$$
$$证：正交变换x=Qy,\\
x^Tx=(Qy)^T Qy=y^TQ^TQy=y^Ty=M\\
\ \\
x^TAx\xlongequal{坐标变换}y^T\Lambda y=\lambda_1y_1^2+\lambda_2y_2^2+\cdots+\lambda_ny_n^2$$

## 矩阵合同的性质

$$矩阵合同的性质（必要不充分条件）：\\
\begin{array}{ll}
A\simeq B&\Rightarrow r(A)=r(B)\\
A\simeq B,A=A^T& \Rightarrow B=B^T\\
A\simeq B,A\simeq C&\Rightarrow B\simeq C\\

A\simeq B&\Leftrightarrow A^{-1}\simeq B^{-1}（若可逆）,A^{T}\simeq B^{T}\\
&\Rightarrow A^{*}\simeq B^{*}
\end{array}\\
\ \\
若A可逆，则(A^{-1})^TAA^{-1}=A^{-1},故A与A^{-1}合同$$
$$证：
P^TAP=B  
\left\{\begin{array}{l}
\Leftrightarrow P^{-1}A^{-1}(P^{-1})^T=B^{-1}\\
\Leftrightarrow P^TA^TP=B^T\\
\Rightarrow P^*A^*(P^*)^T=B^*
\end{array}\right.$$

## 二次型矩阵合同的判定

**合同不要求实对称矩阵，但二次型矩阵只能是实对称矩阵**
$$充要条件：实对称矩阵
\left\{
\begin{array}{c}
正负惯性指数相同\\
或\\
特征值正负个数对应相同
\end{array}
\right.$$
$$实对称矩阵，矩阵相似A\sim B\ \substack{\Rightarrow\\ \not\Leftarrow}\ 矩阵合同A\simeq B$$
$$注：
可逆坐标变换（合同变换）不改变矩阵正、负惯性指数$$

## 标准型与规范型

$$对角线元素不一定为0，非对角线元素均为0
\left\{\begin{array}{l}
标准型对角线元素不一定为特征值\\
规范型对角线元素只能为-1,1,0

\end{array}\right.$$

## 二次型标准化或规范化

$$首选拉格朗日配方法（P自然可逆）：\\
配平后得y=\bigg(\qquad\bigg)x=Px，方程直接反解x=Cy（求逆矩阵繁琐）\\
注：拉格朗日配方法可任意配标准型或规范型系数\\
$$

$$备选正交相似对角化\\
注：正交变换无法任意配系数
\left\{
\begin{array}{rl}
x^TAx&=y^T(Q^T\Lambda_1 Q) y\\
&=y^T[Q^TE_2(\sqrt{3})\Lambda_2 E_2(\sqrt{3})Q] y\\
&Q^TE_2(\sqrt{3}) E_2(\sqrt{3})Q\neq E\\
&（非相似变换，即非正交变换）
\end{array}
\right.$$

## 正定二次型定义

$$前提：
A=A^T，且为实数$$
$$n元二次型f=x^TAx.若对任意x\neq0，均有x^TAx>0(当且仅当x=0时，f=0)，则\\称f为正定二次型，称A为正定矩阵$$

## ⭐️正定二次型的判定

$$前提：A=A^T，且为实数$$
$$充要条件：\\
\begin{array}{rl}
f=x^TAx正定
&\Leftrightarrow A的全部顺序主子式>0\\
&\Leftrightarrow A的特征值\lambda_i>0(i=1,2,\cdots,n)\\
&\Leftrightarrow f的正惯性指数p=n\\
&\Leftrightarrow A\simeq E\\
&\Leftrightarrow 存在可逆矩阵D，使得A=D^TD\\
&（灵活串用充要条件）\\
&\Leftrightarrow A^{-1},A^T,A^*(|A|\neq0),kA(k>0),P^TAP正定(P可逆)\\
&（特征值>0，具体意义证得）\\
\end{array}
$$
$$必要不充分条件：\\
\begin{array}{rl}
f=x^TAx正定&\Rightarrow a_{ii}>0 \\
&\Rightarrow |A|>0\\
&\Rightarrow A^k正定(P^TA^kP=P^TAP\cdots P^TAP=E)
\end{array}$$
$$ 顺序主子式：\\
D_1=a_{11},D_2=\left|
\begin{array}{}
a_{11}&a_{12}\\
\\
a_{21}&a_{22}
\end{array}
\right| ,
D_3=\left|
\begin{array}{}
a_{11}&a_{12}&a_{13}\\
\\
a_{21}&a_{22}&a_{23}\\
\\
a_{31}&a_{32}&a_{33}
\end{array}
\right| $$

## 正定矩阵的性质

$$A,B正定\Rightarrow A+B正定（实际意义易得）\\
A,B正定\Leftrightarrow\left(\begin{array}{cc}A&O\\O&B\end{array}\right)正定\\
若A正定且正交，故A特征值\lambda_i>0且\lambda_i=\pm1，则\lambda_i=1\\
若A可逆，则A^TA正定\quad证：(A^{-1})^TA^TAA^{-1}=E$$

## 重要经验

$$实对称矩阵正交变换较为特殊，可同时考查“相似”与“二次型”$$

## 重要结论

$$任何二次型均可通过“配方法”化为标准型或规范型\\
任何二次型均可通过“正交变换”化为标准型$$
$$正交变换不改变几何图形的形状\\
x^Tx=y^Ty\Rightarrow\Vert x\Vert=\Vert y\Vert\Rightarrow 形状不变$$

## 二次型无平方项情形

$$令\left\{
\begin{array}{l}
x_1=y_1-y_2\\
x_2=y_1+y_2\\
x_3=y_3
\end{array}
\right.$$

## 矩阵合同求坐标变换

**A,B均为对角矩阵：**
$$\left.\begin{array}{}f=2x_1^2+x_2^2-3x_3^2\\
f=-2y_1^2+y_2^2+3y_3^2
\end{array}\right\}对应变量代换即可$$
**A,B(B为对角矩阵)：**
$$配方法，配平后凑系数即可\\
\frac{1}{2}(\sqrt{2}x_1+\sqrt{2}x_2)^2+\frac{1}{9}(3x_1-3x_2)^2+x_3^2$$
**A,B(均非对角阵)：**
$$A,B分别配方法，凑成规范型，对应项相等，反解x=Cy\\
(3x_1-2x_2)^2+x_2^2\\
(y_1-4y_2)^2+y_2^2$$

## 二次型几何意义

$$\begin{array}{}
\lambda_1,\lambda_2,\lambda_3符号 & 曲面f=a(a>0)\\
3正 & 椭球面\\
2正1负 & 单叶双曲面\\
1正2负 & 双叶双曲面\\
2正1零 & 椭圆柱面\\
1正1负1零 & 双曲柱面

\end{array}$$

## 二次型几何应用处理方法

$$二次曲面x^2+3y^2+z^2+2xy+2xz+2yz=4经正交变换\\
化为\eta^2+4\xi^2=4\\
\Leftrightarrow \\
二次型f=x^2+3y^2+z^2+2xy+2xz+2yz经正交变换\\
化为\eta^2+4\xi^2$$

## 二次型“平方式”题型

**所给“平方式”不一定由可逆坐标变换得到**
$$f=(x_1-x_2+x_3)^2+(x_2+x_3)^2+(x_1+ax_3)^2\\
\left|\begin{array}{}1&-1&1\\0&1&1\\1&0&a\end{array}\right|=a-2\\
a\neq2,规范型即为“平方式”\\
a=2,代入表达式\rightarrow拆开\rightarrow拉格朗日配方$$

## 二次型正定相关题型

**灵活运用正定的定义及意义、其余充要条件熟用即可**
$$例：
A列满秩，或Ax=0只有零解\Rightarrow (x^TA^T)(Ax)\geqslant0，且仅在x=0处取到0，即(x^TA^T)(Ax)正定$$

## 正定二次型的解

$$f(x_1,x_2,x_3)=(a_{11}x_1+\cdots+a_{13}x_3)^2+(a_{21}x_1+\cdots+a_{23}x_3)^2+(a_{31}x_1+\cdots+a_{33}x_3)^2=0正定\\
\Leftrightarrow
\left(\begin{array}{l}
a_{11}&a_{12}&a_{13}\\
a_{21}&a_{22}&a_{23}\\
a_{31}&a_{32}&a_{33}
\end{array}\right)x=0仅有零解$$
$$
f(x_1,x_2,x_3)=x^TAx\xrightarrow{x=Cy化规范型（正交对角化、配方法）}f(x_1,x_2,x_3)=(x_1+x_2+x_3)^2=y^TC^T\ \Lambda \  Cy=0\\
{\color{blue}非负定}二次型f(x_1,x_2,x_3)=0的解，即x_1+x_2+x_3=0的解$$

# 横向知识点对比

## 各大运算的等价性质

$$\begin{array}{rl}
A可逆&\Leftrightarrow A^{-1},A^*,A^T可逆\\
A正定&\Leftrightarrow A^{-1},A^T,A^*(|A|\neq0),kA(k>0),P^TAP正定(P可逆)\\
A为正交矩阵&\Leftrightarrow A^{-1},A^*,A^T,-A为正交矩阵\\
\ \\
A\sim B & \Leftrightarrow A^{-1}\sim B^{-1}(|A|\neq0时),\quad A^T\sim B^T,\quad A^*\sim B^*(|A|\neq0时)\\
A\simeq B & \Leftrightarrow A^{-1}\simeq B^{-1}(|A|\neq0时),\quad A^T\simeq B^T\quad(\Rightarrow A^*\simeq B^*)

\end{array}$$

# 特殊情形

## 特殊矩阵1

$$A=\alpha\alpha^T+\beta\beta^T,\quad \alpha^T\beta=0,\alpha\alpha^T=2,\beta\beta^T=1\qquad
r(A)\leqslant 2\\
A\alpha=2\alpha,A\beta=\beta$$
$$A=\alpha\beta^T+\beta\alpha^T,\quad \alpha^T\beta=0,\alpha\alpha^T=2,\beta\beta^T=2\qquad
r(A)\leqslant 2\\
A\alpha=2\beta,A\beta=2\alpha\\
A(\alpha+\beta)=2(\alpha+\beta),A(\alpha-\beta)=-2(\alpha-\beta)$$
$$注：A均为实对称矩阵$$

## 特殊矩阵2

$$A=E-axx^T\rightarrow A^2=(E-axx^T)(E-axx^T)（寻找矩阵关系）$$

# 待整理问题

证明题：相似，正定等

# 结论证明

$$r(A)+r(B)-n\leqslant r(AB)$$

$$A_{m\times n}B_{n\times s}\quad
\left(
\begin{array}{}
AB&O\\
O&E_n
\end{array}
\right)\rightarrow
\left(
\begin{array}{}
AB&A\\
O&E_n
\end{array}
\right)\rightarrow
\left(
\begin{array}{}
O&A\\
-B&E_n
\end{array}
\right)\quad （分块矩阵初等变换）\\
r(AB)+n\geqslant r(A)+r(B)\\即
r(A)+r(B)-n\leqslant r(AB)$$

# 计算严谨性问题

经验表明，矩阵运算的出错率最高，弱智错误；勿急，一步错步步错
