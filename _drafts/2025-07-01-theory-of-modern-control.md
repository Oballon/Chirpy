现代控制理论

现代控制理论中诸多方法难以查得证明，且用即可；801控制原理的考察范围不完全明晰，视为风险的一部分

# 默认章节

## 考情分析

两大难点：能控能观结构分解，观测器状态反馈

# 状态空间表达式

## 考情分析

线性系统离散化不考

## 连续、离散系统的表达式

$$连续：\begin{array}{l}
\dot{x} =Ax + Bu \\
y=Cx+Du
\end{array}（系统矩阵A为方阵）$$
$$离散：\begin{array}{l}
x(k+1) =Gx(k) +Hu(k)\\
y(k)=Cx(k)+Du(k)
\end{array}\\
$$

## 连续系统与离散系统对比

**总括衍生，离散系统考查较弱**
$$离散系统与连续系统诸多性质极其相似：
$$
$$\left.\begin{array}{}系统实现相通\\
非奇异变换相通
\end{array}\right\}
“积分元”\frac{1}{s}对应“延迟元”z^{-1}(T) \quad \#\quad \frac{\frac{1}{s}}{1+\frac{\lambda}{s}}对应\frac{\frac{1}{z}}{1+\frac{\lambda}{z}} $$
$$\mathscr{L}变换对应Z变换$$
$$传递函数阵计算公式（零初始条件）：\\
\left\{\begin{array}{l}
sX(s) =AX(s)+ BU(s) \\
Y(s)=CX(s)
\end{array}\right.\Rightarrow Y(s)=C(sI-A)^{-1}BU(z)\\
\ \\
\left\{\begin{array}{l}
zX(z)=GX(z)+HU(z)\\
Y(z)=CX(z)
\end{array}\right.\Rightarrow Y(z)=C(zI-G)^{-1}HU(z)\\
 注：根据状态空间表达式，计算离散、连续传递函数仅字母有异$$

## 非奇异变换及其性质

$$状态空间表达式非唯一，线性变换系统等价\\
连续：\left\{
\begin{array}{l}
\dot{x}=Ax+Bu\\
y=Cx+Du
\end{array}
\right.\xrightarrow{x=Tz,\quad z=T^{-1}x}
\left\{
\begin{array}{l}
\dot{z}=T^{-1}ATz+T^{-1}Bu\\
y=CTz+Du
\end{array}
\right.
$$
$$性质：\\
不改变系统传递函数阵\\
不改变特征方程、特征值\\
不改变能控、能观性
$$

## SISO能控标准Ⅰ型实现

**离散系统实现同理**
$${\color{blue}分母为首“1”型}\\
W(s)=\frac{b_ns^n+b_{n-1}s^{n-1}+\cdots+b_1s+b_0}{s^n+a_{n-1}s^{n-1}+\cdots+a_1s+a_0}=b_n+\frac{(b_{n-1}-a_{n-1}b_n)s^{n-1}+\cdots+(b_1-a_1b_n)s+(b_0-a_0b_n)}{s^n+a_{n-1}s^{n-1}
+\cdots+a_1s+a_0}\\
友矩阵：
A=
\begin{pmatrix}
  0&1&0&\cdots&0 \\
  0&0&1&\cdots&0 \\
\vdots&\vdots&\vdots&\ddots&\vdots \\
 0&0&0&\cdots&1 \\
  -a_0&-a_1&-a_2&\cdots &-a_{n-1}
\end{pmatrix}\qquad
b=\begin{pmatrix}
0\\
0\\
\vdots \\
0 \\
1
\end{pmatrix}\\
\ \\
c=((b_0-a_0b_n),(b_1-a_1b_n),\cdots,(b_{n-1}-a_{n-1}b_n))\qquad d=b_n$$
$$注：连续、离散系统传递函数实现一致\\
若分子阶次低于分母，则c仅由b_0,b_1,\cdots,b_{n-1}顺序构成
$$

## SISO能观标准Ⅰ型实现

**离散系统实现同理**
$$W(s)=\frac{b_ns^n+b_{n-1}s^{n-1}+\cdots+b_1s+b_0}{s^n+a_{n-1}s^{n-1}+\cdots+a_1s+a_0}\\
友矩阵：
A=
\begin{pmatrix}
  0&1&0&\cdots&0 \\
  0&0&1&\cdots&0 \\
\vdots&\vdots&\vdots&\ddots&\vdots \\
 0&0&0&\cdots&1 \\
  -a_0&-a_1&-a_2&\cdots &-a_{n-1}
\end{pmatrix}\qquad
b=\begin{pmatrix}
\beta_{n-1}\\
\beta_{n-2}\\
\vdots \\
\beta_1\\
\beta_0
\end{pmatrix}\\
\ \\
c=(1,0,\cdots,0,0)\qquad d=\beta_n\\
\ \\
\begin{pmatrix}
  1 \\
  a_{n-1}&1&&\text{{\huge 0}} \\
  a_{n-2}&a_{n-1}&1\\
  \vdots&\vdots&\ddots&\ddots \\
  a_0&a_1&\cdots &a_{n-1}&1
\end{pmatrix}
\begin{pmatrix}
\beta_n\\
\beta_{n-1}\\
\beta_{n-2}\\
\vdots \\
\beta_0
\end{pmatrix}=
\begin{pmatrix}{}
b_n\\
b_{n-1}\\
b_{n-2}\\
\vdots\\
b_0
\end{pmatrix}\qquad （按行计算，一般不超三阶）$$
$$注：连续、离散系统传递函数实现一致\\
能观标准Ⅰ型实现的计算矩阵为n+1维；能观标准Ⅰ型的变换矩阵为n维
$$

## MIMO系统能控、能观标准型实现

$$W(s)=\boldsymbol\beta_n+\frac{\boldsymbol\beta_{n-1}s^{n-1}+\boldsymbol\beta_{n-2}s^{n-2}+\cdots+\boldsymbol\beta_1s+\boldsymbol\beta_0}{s^n+a_{n-1}s^{n-1}+\cdots+a_1s+a_0}\quad （\beta_n提取与\text{SISO}方式一致）\\
\boldsymbol\beta_{n-1},\boldsymbol\beta_{n-2},\cdots,\boldsymbol\beta_1,\boldsymbol\beta_0为m\times r为矩阵，m为输出矢量的维数，r为输入矢量的维数$$
$$能控标准Ⅰ型：\\
A=
\begin{pmatrix}
\mathbf{0}_r&\textbf{I}_r&\mathbf{0}_r&\cdots&\mathbf{0}_r \\
\mathbf{0}_r&\mathbf{0}_r&\textbf{I}_r&\cdots&\mathbf{0}_r \\
\vdots&\vdots&\vdots&\ddots&\vdots \\
\mathbf{0}_r&\mathbf{0}_r&\mathbf{0}_r&\cdots&\textbf{I}_r \\
  -a_0\textbf{I}_r&-a_1\textbf{I}_r&-a_2\textbf{I}_r&\cdots &-a_{n-1}\textbf{I}_r
\end{pmatrix}\qquad
B=\begin{pmatrix}
\mathbf{0}_r\\
\mathbf{0}_r\\
\vdots \\
\mathbf{0}_r \\
\textbf{I}_r
\end{pmatrix}\\
\ \\
C=(\boldsymbol\beta_0,\boldsymbol\beta_1,\cdots,\boldsymbol\beta_{n-1})\quad D=\boldsymbol\beta_n$$
$$能观标准Ⅱ型：\\
A=
\begin{pmatrix}
\mathbf{0}_m&\mathbf{0}_m&\cdots&\mathbf{0}_m&  -a_0\textbf{I}_m\\
\textbf{I}_m&\mathbf{0}_m&\cdots&\mathbf{0}_m&-a_1\textbf{I}_m \\
\mathbf{0}_m&\textbf{I}_m&\cdots&\mathbf{0}_m &-a_2\textbf{I}_m\\
\vdots&\vdots&\ddots&\vdots &\vdots\\
\mathbf{0}_m&\mathbf{0}_m&\cdots&\textbf{I}_m &-a_{n-1}\textbf{I}_m\\
\end{pmatrix}\qquad
B=\begin{pmatrix}
\boldsymbol\beta_0\\
\boldsymbol\beta_1\\
\boldsymbol\beta_2\\
\vdots\\
\boldsymbol\beta_{n-1}
\end{pmatrix}\\
\ \\
C=(\mathbf{0}_m,
\mathbf{0}_m,
\cdots ,
\mathbf{0}_m,
\textbf{I}_m)\quad D=\boldsymbol\beta_n$$
$$注：能控标准Ⅰ型与能观标准Ⅱ型不是简单转置关系$$

## 约旦标准型实现

**离散系统实现同理**
$$思路：传递函数因式分解$$
$$单根：G(s)=\frac{a}{s-\lambda_1}+\frac{b}{s-\lambda_2}+\frac{c}{s-\lambda_3}+\cdots\\
A=
\left(\begin{array}{l}
\lambda_1\\
&\lambda_2\\
&&\lambda_3
\end{array}\right)\quad

b=
\left(\begin{array}{l}
1\\
1\\
1
\end{array}\right)\\
\ c=
\left(\begin{array}{l}
a & b & c
\end{array}\right)\\
或A=
\left(\begin{array}{l}
\lambda_1\\
&\lambda_2\\
&&\lambda_3
\end{array}\right)\quad b=
\left(\begin{array}{l}
a\\
b\\
c
\end{array}\right)\\
\ c=
\left(\begin{array}{l}
1 & 1 & 1
\end{array}\right)$$
$$重根：G(s)=\frac{a}{(s-\lambda_1)^3}+\frac{b}{(s-\lambda_1)^2}+\frac{c}{(s-\lambda_1)}\\
A=
\left(\begin{array}{l}
\lambda_1&1\\
&\lambda_1&1\\
&&\lambda_1
\end{array}\right)\quad

b=
\left(\begin{array}{l}
0\\
0\\
1
\end{array}\right)\\
\ c=
\left(\begin{array}{l}
a&b&c
\end{array}\right)$$
$$注：同时含有单根、复根，矩阵拼接即可\\
{\color{blue}只考查输入一维系统}$$

## 约旦标准型

$$定义：除了主对角线和主对角线上方元素之外，其余都是零\\主对角线上方的对角线的系数若不为0只能为1，且这1左方和下方的系数（都在主对角线上）有相同的值\\
\ \\
即\quad约旦标准型的对角元素为矩阵特征值\lambda_i，紧邻对角线的上方元素为0或1，其余元素均为0$$
$$性质：\\
1.任何矩阵均可约旦对角化\\
2.约旦标准型中，重特征值有可能对应多个子约旦块（此类矩阵不考）\\
{\color{blue}某重特征值对应的几何重数=此特征向量对应的子约旦块个数}\\
例：
\left(
\begin{array}{}
3 & 1 & -1\\
-2 & 0 & 2 \\
-1 & -1 & 3
\end{array}
\right)\quad
\lambda_1=\lambda_2=\lambda_3=2\\
A的约旦标准型为\left(
\begin{array}{}
2 &0&0\\
0 & 2 & 1 \\
0 & 0 & 2
\end{array}
\right)$$

## 约旦标准型的变换阵

$$单特征值：求特征矢量即可\\
x=Tz\qquad T=(P_1,P_2,\dots, P_n)$$
$$重特征值(单根部分用单根方法求)：\\
此法由“单一标准型”反推得，仅可求重特征值仅对应一个约旦块情形\\
\lambda_1P_1-AP_1=0\qquad {\color{blue}（P_1只能是一维特征向量，即几何重数为1）}\\
\lambda_1P_2-AP_2=-P_1\\
\qquad\qquad\ \vdots\\
\lambda_1P_q-AP_q=-P_{q-1}\\
$$
$$注：
对角线标准型即为特征根均互异的约旦标准型$$

## 传递函数阵及其性质

**离散系统同理**
$$传递函数阵：\left\{\begin{array}{ll}
W_{ux}(s)=\frac{X(s)}{U(s)}=(sI-A)^{-1}b & W_{ux}(s)=\frac{X(s)}{U(s)}=(sI-A)^{-1}B\\
\ \\
W(s)=\frac{Y(s)}{U(s)}=c(sI-A)^{-1}b+d & W(s)=\frac{Y(s)}{U(s)}=C(sI-A)^{-1}B+D

\end{array}\right.$$
$$子系统组合的传递函数阵：\\
并联连接：W(s)=W_1(s)\pm W_2(s)\\
串联连接：W(s)=W_2(s) W_1(s)\quad （注意次序，“后”乘“前”；\quad 输入、输出维数对应）\\
负反馈连接：
\left\{\begin{array}{}
W(s)=W_1(s)[I+W_2(s)W_1(s)]^{-1}\\
W(s)=[I+W_1(s)W_2(s)]^{-1}W_1(s)
\end{array}\right.\quad （注意次序\quad 1,2,1；\quad  W_1(s)，W_2(s)维数对偶）$$

## 模拟结构图绘制典例

$$\left.\begin{array}{l}
能控标准型\\
能观标准型
\end{array}\right\}关键在系统的友矩阵绘制，
\left\{\begin{array}{}
A(x_n\to x_1\ +\  “归首”)\\
A^T(x_1\to x_n\ +\  “尾散”)
\end{array}\right.b,c直接引出即可$$
$$约旦标准型：\\
系统矩阵绘制
\left\{\begin{array}{l}
单根：独立\\
重根：x_n\to x_1\  +\ “元回路”
\end{array}\right.\quad
正反馈系数对应特征值\lambda；\quad
b,c直接引出即可$$
$$一般结构图：关键在确定状态变量先后关系（最多三阶，考查不会复杂）$$

## 状态变量选取及状态空间表达式建立

**整理思路：列写所有变量关系，消去中间变量**
$$一阶环节
\frac{1}{s},\quad\frac{s-1}{s+2},\quad \frac{3}{0.5s+1}\\
每个一阶环节后对应一个状态变量\\
变量间关系“去分式”后对应：\\
X_2=\frac{s-1}{s+2}X_1\\
X_2(s+2)=(s-1)X_1\longrightarrow \dot{x}_2+2x_2=\dot{x}_1-x_1\\
等式整理合并为
\left\{\begin{array}{l}
\dot{x}=Ax+bu\\
y=cx
\end{array}\right.变量对应绘制模拟结构图即可$$
$$注：线性系统均可消元整理出来$$

## 约旦标准化（对角化）题型

**各有特点，灵活运用**
$$系统实现：求出传递函数G(s)=c(sI-A)^{-1}b\\
因式分解(\frac{a}{s-\lambda_1}+\frac{b}{s-\lambda_2}+\cdots)，利用约旦标准型实现进行标准化\\

$$
[约旦标准型实现](#约旦标准型实现)

$$约旦变换：计算变换矩阵x=Tz进行线性变换\\
\overline{A}=T^{-1}AT \quad
\overline{b}=T^{-1}b\quad
\overline{c}=cT$$

# 状态空间表达式的解

## 连续状态转移矩阵及其性质

$$定义：x(t)=\Phi(t)x_0=e^{At}x_0\\
e^{At}=I+At+\frac{1}{2!}A^2t^2+\cdots+\frac{1}{n!}A^nt^n+\cdots

$$
$$\begin{array}{ll}
性质一：\Phi(t)\Phi(\tau)=\Phi(t+\tau)\quad & 即e^{At}e^{A\tau}=e^{A(T+\tau)}\\
\ \\
性质二：\Phi(t-t)=I\quad &即e^{A(t-t)}=\Phi(0)=I\\
\ \\
性质三：[\Phi(t)]^{-1}=\Phi(-t)\quad &即[e^{At}]^{-1}=e^{-At}\\
\ \\
性质四：\dot{\Phi}(t)=A\Phi(t)=\Phi(t)A &
\dot{\Phi}(0)=A\\
\ \\
性质五：当且仅当AB=BA时，e^{At}e^{Bt}=e^{(A+B)t} &（对于n\times n方阵A,B）
\end{array}$$
$$注：e^{At}为一种记法，与指数运算高度统一$$

## 状态转移矩阵的计算

**考研考查最多三维矩阵，灵活选择使用**
$$变换为对角线标准型：T^{-1}AT=\Lambda\\
{\color{blue}前提：可相似对角化}\\
\Phi(t)=e^{At}=T(I+\Lambda t+\frac{1}{2!}\Lambda^2t^2+\cdots+\frac{1}{n!}\Lambda^nt^n+\cdots)T^{-1}=

T
\left(
\begin{array}{}
e^{\lambda_1t}&\\
&e^{\lambda_2t}\\
&&\ddots\\
&&&e^{\lambda_nt}
\end{array}
\right)
T^{-1}$$

$$拉氏反变换（阶次\leqslant 3时）：e^{At}=\mathscr{L^{-1}}[(sI-A)^{-1}]\quad （实则对矩阵中元素\mathscr{L}^{-1}）
$$

## 线性定常非齐次的解

$$x(t)=\underbrace{\Phi(t)x(0)}_{初始状态转移}+\underbrace{\int_0^t\Phi(t-\tau)Bu(\tau)d\tau}_{激励状态转移}\quad (实则对矩阵中元素积分)$$
$$推导：sX-x(0) =AX(s) + BU(s) \\
\Rightarrow (sI-A)X(s)=x(0)+BU(s)\\
\Rightarrow X(s)= (sI-A)^{-1}x(0)+ \underbrace{(sI-A)^{-1}BU(s)}_{\mathscr{L}^{-1}略}$$

## 离散定常非齐次的解

$$\begin{array}{rl}
x(k)&=\underbrace{G^kx(0)}_{初始状态转移}+\underbrace{\sum_{j=0}^{k-1}G^{(k-1)-j}Hu(j)}_{激励状态转移}\\
\ \\
&=G^{k}x(0)+G^{k-1}Hu(0)+G^{k-2}Hu(1)+\cdots++GHu(k-2)+Hu(k-1)
\end{array}$$

## 状态转移矩阵反解系统

**考查状态转移矩阵的性质**
![](pic-theory-of-modern-control\Markji_1751378147398.png)
$$\Phi(0)=I\quad \dot{\Phi}(0)=A（或A=\dot{\Phi}(t)\Phi(-t)）$$

## 求解状态转移矩阵典例

![](pic-theory-of-modern-control\Markji_1751378160041.png)
$$e^{At}
\left(\begin{array}{l}
1&2\\
-1&-1
\end{array}\right)=
\left(\begin{array}{}
e^{-2t}&2e^{-2t}\\
-e^{-2t}&-e^{-t}
\end{array}\right)\\

e^{At}=\left(\begin{array}{}
e^{-2t}&2e^{-2t}\\
-e^{-2t}&-e^{-t}
\end{array}\right)
\left(\begin{array}{l}
1&2\\
-1&-1
\end{array}\right)^{-1}$$

# ""能控性能观性""

## 能控、能观性定义

$$u(t)对状态矢量x(t)的控制性（对任意状态均能控，则系统能控）：\\
存在一个分段连续的输入u(t)，能在有限时间区间内，使系统由某一初始状态x(t_0)，转移至指定的任意终端状态x(t)$$
$$y(t)对状态矢量x(t)的观测性（对任意状态均能观，则系统能观）：\\
对任意给定的u，在有限观测时间内t_f>t_0，使得根据[t_0,t_f]期间的输出y(t)能唯一地确定系统在初始时刻的状态x(t_0)\\
$$

## 离散化对系统性能影响

$$
1. 能控或能观的连续系统，离散化后不一定能保持其能控或能观性\\
2. 不能控或不能观的系统，无论采样周期如何选择，离散化后一定不能控或不能观$$

## 能控、能观的判定方法

$$是否友矩阵标准型\\
\ \\
约旦标准型判据\\
\ \\
能控、能观判别矩阵行、列满秩\\
\ \\
\text{SISO}系统W(s)=c(sI-A)^{-1}b是否零极点对消
$$

## 友矩阵标准型判定

$$系统矩阵A为友矩阵或其转置，对应b,c也应为标准型\\
观测量，控制量多了也不一定能控、能观$$

## 能控性、能观性判别矩阵

$$行满秩即能控：\\
M=(b, Ab, A^2b, \cdots, A^{n-1}b)\\
M=(B, AB, A^2B, \cdots, A^{n-1}B)\\
M=(H, GH, G^2H, \cdots, G^{n-1}H)$$
$$列满秩即能观：\\
N=\begin{pmatrix}
  c \\
 cA \\
\vdots \\
 cA^{n-1}
\end{pmatrix}\quad N=\begin{pmatrix}
  C \\
 CA \\
\vdots \\
 CA^{n-1}
\end{pmatrix}\quad
N=\begin{pmatrix}
  C \\
 CG \\
\vdots \\
 CG^{n-1}
\end{pmatrix}$$

## 约旦标准型判断能控、能观

$$能控性：\\
互异特征值：每个特征值对应的B阵的各行元素均不全为0\\
相同特征值：对于某重特征值，属于该特征值的各子约旦块的最后一行所对应的B的行均不全为0，且线性无关\\
\ \\
能观性：\\
互异特征值：每个特征值对应的C阵的各列元素均不全为0\\
相同特征值：对于某重特征值，属于该特征值的各子约旦块的首列所对应的C的列均不全为0，且线性无关
$$
$$注：零向量与其本身线性相关，零向量与任何向量线性相关\\
重特征值多个约旦块，B为单列（或C为单行），必线性相关$$

## 输出能控性判别矩阵

$$u(t)对y(t)的能控性\\\\
行满秩即能控：
M=(CB,CAB,CA^2B,\cdots,CA^{n-1}B,D)$$

## 零极点对消

$$W(s)=c(sI-A)^{-1}b\\
 (sI-A)^{-1}=\frac{(sI-A)^*}{|sI-A|}
\left\{
\begin{array}{l}
若无零极点对消，分母为s的n阶多项式\\
若存在零极点对消，分母阶次小于n
\end{array}
\right.$$

## 能控、能观的充分必要条件

$$\Sigma(A,B,C)为最小实现\Leftrightarrow 系统能控且能观\\
\ \\
单输入系统\Sigma(A,b,c)能控的充分必要条件：\\
W_{ux}=(sI-A)^{-1}b\ 无零极点对消\\
\ \\
单输入单输出系统\Sigma(A,b,c)能控能观的充分必要条件：\\
W(s)=c(sI-A)^{-1}b\ 无零极点对消$$
$$注：多输入多输出系统\Sigma(A,B,C)无零极点对消\ \substack{\Rightarrow\\
\not\Leftarrow}\ 系统\Sigma(A,B,C)能控能观（最小实现）$$

## 最小实现部分

$$寻找系统\Sigma(A,B,C)最小实现的方法：找出完全能控且能观的部分$$

## 系统的对偶关系与性质

$$系统\Sigma_1\left\{\begin{array}{l}
\dot{x_1}=A_1x_1+B_1u_1\\
y_1=C_1x_1
\end{array}{}
\right.\qquad
系统\Sigma_2\left\{\begin{array}{l}
\dot{x_2}=A_2x_2+B_2u_2\\
y_2=C_2x_2
\end{array}{}
\right.\\
\ \\
系统\Sigma_1与\Sigma_2互为对偶:
A_2=A_1^T\qquad
B_2=C_1^T\qquad
C_2=B_1^T$$
$$性质：\\
对偶系统的传递函数矩阵互为转置\\
\Sigma_1的能控性（能观性）等价于\Sigma_2的能观性（能控性）$$

## 能控标准Ⅰ型与能观标准Ⅱ型

**前提：判定系统能控、能观**
$$\begin{array}{ll}
能控标准Ⅰ型：&能观标准Ⅱ型：\\
\overline{A}=T^{-1}_{c1}AT_{c1}=
\begin{pmatrix}
  0&1&\cdots&0&0 \\
  0&0&\cdots&0&0 \\
  \vdots&\vdots&&\vdots&\vdots \\
 0&0&\cdots&0&1 \\
  -a_0&-a_1&\cdots &-a_{n-2}&-a_{n-1}
\end{pmatrix}
&
\overline{A}=T^{-1}_{o2}AT_{o2}=
\begin{pmatrix}
  0&0&\cdots&0&-a_0 \\
  1&0&\cdots&0&-a_1 \\
 0&1&\cdots&0&-a_2 \\
  \vdots&\vdots&&\vdots&\vdots \\
  0&0&\cdots &1&-a_{n-1}
\end{pmatrix}\\

\overline{b}=T^{-1}_{c1}b=
\begin{pmatrix}
0\\
0\\
\vdots \\
0 \\
1
\end{pmatrix}
&
\overline{b}=T^{-1}_{o2}b=
\begin{pmatrix}
\beta_0\\ \beta_1\\ \beta_2\\ \vdots\\ \beta_{n-1}
\end{pmatrix}
\\

\overline{c}=cT_{c1}=(\beta_0, \beta_1, \beta_2, \cdots, \beta_{n-1})
&
\overline{c}=cT_{o2}=(0, 0, 0, \cdots, 1)\\

\ \\
T_{c1}=(A^{n-1}b, A^{n-2}b, \dots, Ab, b)
\begin{pmatrix}
  1 \\
  a_{n-1}&1&&\text{{\huge 0}} \\
  \vdots&\vdots&\ddots \\
  a_2&a_3&\cdots&1 \\
  a_1&a_2&\cdots &a_{n-1}&1
\end{pmatrix}
&
T_{o2}^{-1}=
\begin{pmatrix}
  1&a_{n-1}&\cdots&a_2&a_1\\
  &1&\cdots&a_3&a_2 \\  &&\ddots&\vdots&\vdots \\
  &\text{{\huge 0}}&&1&a_{n-1} \\
  &&&&1
\end{pmatrix}
\begin{pmatrix}
cA^{n-1}\\
 cA^{n-2}\\
\vdots\\
 cA\\
 c
\end{pmatrix}

\end{array}$$
$$标准化步骤：
\left\{\begin{array}{l}
1. 特征多项式|\lambda I-A|=0求得a_i\\
2. 计算变换矩阵T
\end{array}\right.$$
$$注：(cT_{c1})^T=T_{o2}^{-1}b\\
能观标准Ⅰ型实现的计算矩阵为n+1维；能控标准Ⅰ型的变换矩阵为n维$$

## 能观标准Ⅰ型与能控标准Ⅱ型

**前提：判定能控、能观**
$$\begin{array}{ll}
能观标准Ⅰ型：&能控标准Ⅱ型：\\
\overline{A}=T^{-1}_{o1}AT_{o1}=
\begin{pmatrix}
  0&1&\cdots&0&0 \\
  0&0&\cdots&0&0 \\
  \vdots&\vdots&&\vdots&\vdots \\
 0&0&\cdots&0&1 \\
  -a_0&-a_1&\cdots &-a_{n-2}&-a_{n-1}
\end{pmatrix}
&
\overline{A}=T^{-1}_{c2}AT_{c2}=
\begin{pmatrix}
  0&0&\cdots&0&-a_0 \\
  1&0&\cdots&0&-a_1 \\
 0&1&\cdots&0&-a_2 \\
  \vdots&\vdots&&\vdots&\vdots \\
  0&0&\cdots &1&-a_{n-1}
\end{pmatrix}\\

\overline{b}=T^{-1}_{o1}b=
\begin{pmatrix}
\beta_0\\ \beta_1\\ \beta_2\\ \vdots\\ \beta_{n-1}
\end{pmatrix}
&

\overline{b}=T^{-1}_{c2}b=
\begin{pmatrix}
1\\
0\\
\vdots \\
0 \\
0
\end{pmatrix}\\

\overline{c}=cT_{o1}=(1, 0, 0, \cdots, 0)&\overline{c}=cT_{c2}=(\beta_0, \beta_1, \beta_2, \cdots, \beta_{n-1})\\
\ \\

T_{o1}^{-1}=
\begin{pmatrix}
c\\
cA\\
\vdots\\
cA^{n-1}
\end{pmatrix}&
T_{c2}=(b, Ab, \cdots, A^{n-1}b)
\end{array}$$
$$注：(\overline{c})^T=\overline{b}，即(cT_{c2})^T=T_{o1}^{-1}b$$

## 能控、能观标准化题型

$$若仅求标准型，直接求W(s)，利用\text{SISO}系统实现更快捷（标准化的通用方法较繁琐）$$
$$注：能控、能观标准化的考查仅为\text{SISO}系统，且阶数\leqslant3$$

## 能控性、能观性分解

**能控、能观的分解与能观I型、能控Ⅱ型的标准化本质相似（较深不必深究）**
$$\begin{array}{ll}
能控性分解：&能观性分解：\\
标准形式：& 标准形式：\\

\widehat{A}=R^{-1}_c AR_c=
\begin{pmatrix}
\widehat{A}_{11} & \widehat{A}_{12} \\
\\
0 & \widehat{A}_{22}
\end{pmatrix}
&
\widehat{A}=R^{-1}_o AR_o=
\begin{pmatrix}
\widehat{A}_{11} & 0\\
\\
\widehat{A}_{21} & \widehat{A}_{22}
\end{pmatrix}\\

\widehat{B}=R^{-1}_{c}B=
\begin{pmatrix}
\widehat{B}_1 \\
\\
\hdashline \\
0
\end{pmatrix}
&
\widehat{B}=R^{-1}_0B=
\begin{pmatrix}
\widehat{B}_1 \\
\\
\hdashline \\
\widehat{B}_2
\end{pmatrix}\\

\widehat{C}=CR_c=
\left(
\begin{array}{c:c}
\widehat{C}_1 & \widehat{C}_2
\end{array}
\right)
&
\widehat{C}=CR_0=
\left(
\begin{array}{c:c}
\widehat{C}_1 &0
\end{array}
\right)\\
\ \\

变换矩阵：R_c=(R_1, R_2, \cdots, R_{n_c}, \cdots, R_n)
&
变换矩阵：R^{-1}_o=
\begin{pmatrix}
R_1\\
R_2\\
\vdots \\
R_{n_o} \\
\vdots \\
R_n
\end{pmatrix}\\
\begin{array}{l}
前n_c个列矢量是能控性判别阵M的n_c个线性无关的列\\
其余n-n_c个列矢量保证变换矩阵可逆即可
\end{array}
&
\begin{array}{l}
前n_o个行矢量是能观性判别阵N的n_o个线性无关的行\\
其余n-n_o个行矢量保证变换矩阵可逆即可
\end{array}\\
\ \\
\Sigma(\widehat{A}_{11},\widehat{B}_1,\widehat{C}_1)能控 \qquad{\color{blue}（能控子系统维数为n_c）}& \Sigma(\widehat{A}_{11},\widehat{B}_1,\widehat{C}_1)能观\qquad {\color{blue}（能观子系统维数为n_o）}
\end{array}$$

$$注：{\color{blue}涉及矩阵运算很多，R^{-1},R；考查不会超过三阶}\\
对角线上为子系统，A下标从后往前读表示输出方向$$

## 能控能观结构分解的标准形式

$$\widehat{A}=
\begin{pmatrix}
A_{11} & 0 & A_{13} & 0 \\
A_{21} & A_{22} & A_{23} & A_{24} \\
0 & 0 & A_{33} & 0 \\
0 & 0 & A_{43} &A_{44}
\end{pmatrix}\qquad

\widehat{B}=
\begin{pmatrix}
B_1 \\
B_2 \\
0 \\
0
\end{pmatrix}\\
\ \\
\widehat{C}=
\ \begin{pmatrix}
\ \ C_1\ &\ 0\ &\ \ C_3\ &\ \ 0\ \
\end{pmatrix}
$$
$$注：能控右上角，能观左下角$$

## 能控能观性结构分解

**能控、能观的分解与能观I型、能控Ⅱ型的标准化本质相似（较深不必深究）**
$$\Sigma(A,B,C)能控性分解x=R_c\left(\begin{array}{}x_c\\x_{\overline{c}}\end{array}\right)\\
\qquad
\begin{array}{rl}
\left(\begin{array}{}\dot{x}_c\\\dot{x}_{\overline{c}}\end{array}\right)=&R_c^{-1}AR_c\left(\begin{array}{}x_c\\x_{\overline{c}}\end{array}\right)+R^{-1}Bu
=\left(\begin{array}{}\overline{A}_1&\overline{A}_2\\
0&\overline{A}_4\\
\end{array}\right)
\left(\begin{array}{}x_c\\x_{\overline{c}}\end{array}\right)+
\left(\begin{array}{}
\overline{B}\\
0
\end{array}\right)u\\
\\
y=&CR_c\left(\begin{array}{}
x_c\\x_{\overline{c}}\end{array}\right)
=(\overline{C}_1,\overline{C}_2)\left(\begin{array}{}x_c\\x_{\overline{c}}\end{array}\right)

\end{array}$$
$$\begin{array}{}不能控子系统\Sigma_{\overline{c}}(\overline{A}_4,0,\overline{C}_2)能观性分解x_{\overline{c}}=
R_{02}\left(\begin{array}{}
x_{\overline{c}\ o}\\
x_{\overline{c}\ \overline{o}}
\end{array}\right)
&
能控子系统\Sigma_c(\overline{A}_1,\overline{B},\overline{C}_1)能观性分解
x_{c}=
R_{01}\left(\begin{array}{}
x_{c\ o}\\
x_{c\ \overline{o}}
\end{array}\right)\\
\ \\

\begin{array}{}
\dot{x_{\overline{c}}}=\overline{A}_4x_{\overline{c}}\\
\ \\
\begin{array}{rl}
\left(\begin{array}{}
\dot{x}_{\overline{c}\ o}\\
\dot{x}_{\overline{c}\ \overline{o}}
\end{array}\right)=&
R_{02}^{-1}\overline{A}_4R_{02}\left(\begin{array}{}
x_{\overline{c}\ o}\\
x_{\overline{c}\ \overline{o}}
\end{array}\right)\\
=&
\left(\begin{array}{}
A_{33}&0\\
A_{43}&A_{44}
\end{array}\right)
\left(\begin{array}{}
x_{\overline{c}\ o}\\
x_{\overline{c}\ \overline{o}}
\end{array}\right)
\end{array}\\
\ \\
y=\overline{C}_2R_{02}\left(\begin{array}{}
x_{\overline{c}\ o}\\
x_{\overline{c}\ \overline{o}}
\end{array}\right)=(C_3,0)\left(\begin{array}{}
x_{\overline{c}\ o}\\
x_{\overline{c}\ \overline{o}}
\end{array}\right)
\end{array}

&

\begin{array}{}

\dot{x}_c=\overline{A}_1x_c+\overline{A}_2x_{\overline{c}}+Bu\\
\ \\
\left(\begin{array}{}
\dot{x}_{c\ o}\\
\dot{x}_{c\ \overline{o}}
\end{array}\right)
=
R_{01}^{-1}\overline{A}_1R_{01}\left(\begin{array}{}
x_{c\ o}\\
x_{c\ \overline{o}}
\end{array}\right)+
R_{01}^{-1}\overline{A}_2R_{02}
\left(\begin{array}{}
x_{\overline{c}\ o}\\
x_{\overline{c}\ \overline{o}}
\end{array}\right)+R_{01}^{-1}Bu\\

=
\left(\begin{array}{}
A_{11}&0\\
A_{21}&A_{22}
\end{array}\right)x_c+
\left(\begin{array}{}
A_{13}&0\\
A_{23}&A_{24}
\end{array}\right)x_{\overline{c}}+
\left(\begin{array}{}
B_1\\
B_2
\end{array}\right)u\\
\ \\
y=\overline{C}_1R_{01}\left(\begin{array}{}x_{co}\\x_{c\overline{o}}\end{array}\right)=(C_1,0)\left(\begin{array}{}x_{co}\\x_{c\overline{o}}\end{array}\right)
\end{array}

\end{array}$$
$$注：{\color{blue}涉及矩阵运算多；考查不会超过三阶}\\
每一步判断能控、能观性\left\{\begin{array}{l}
能控或能观，相应不用分解\\
一维子系统无需分解，直接判断即可\\
非一维不能观子系统才需分解

\end{array}\right.$$

## 传递函数不同能控、能观性实现

![](pic-theory-of-modern-control\Markji_1751378200640.png)
$$可控不可观、可观不可控对应\frac{s+1}{s^2+3s+2}的可控、可观标准型实现即可$$
$$不可控不可观实现：\frac{Y(s)}{U(s)}=\frac{s+1}{(s+1)(s+2)}=\frac{0}{s+1}+\frac{1}{s+2}\\
不可控、不可观
\left\{\begin{array}{l}

A=
\left(\begin{array}{l}
-1\\&-2
\end{array}\right)\quad
b=
\left(\begin{array}{l}
0\\1
\end{array}\right)\\
\ c=(0\quad 1)

\end{array}\right.$$
$$对角线标准型可灵活构造可控不可观、可观不可控标准型：\\
可控、不可观
\left\{\begin{array}{l}

A=
\left(\begin{array}{l}
-1\\&-2
\end{array}\right)\quad
b=
\left(\begin{array}{l}
1\\1
\end{array}\right)\\
\ c=(0\quad 1)

\end{array}\right.\qquad 可观、不可控
\left\{\begin{array}{l}

A=
\left(\begin{array}{l}
-1\\&-2
\end{array}\right)\quad
b=
\left(\begin{array}{l}
0\\1
\end{array}\right)\\
\ c=(1\quad 1)

\end{array}\right.$$

# 李雅普诺夫稳定性分析

## 考情分析

线性时变系统、非线性系统的李雅普诺夫方程法不考

## 李雅普诺夫方法选择

$$\begin{array}{}
第一法\#线性系统（特征值；\quad 连续，离散） & 第一法\#非线性系统（平衡点线性化；\quad 临界失效）\\
\ \\
第二法\#线性系统（李雅普诺夫方程；\quad连续，离散）& 第二法\#非线性系统（李雅普诺夫函数；定义法）
\end{array}$$

## 李雅普诺夫第一法（连续系统）

$$状态稳定性（平衡状态x_e=0处渐进稳定的充要条件）：\\
系统矩阵A的所有特征值均具有负实部，即|\lambda I-A|=0根的实部均为负值\\

\left\{\begin{array}{l}
低阶|\lambda I-A|=0解根\\
高阶|\lambda I-A|=0用劳斯判据
\end{array}\right.\\
注：状态稳定性与(sI-A)^{-1}b实部均为负值有区别，可能零极点相消$$
$$
\text{BIBO}稳定性（有界输入输出稳定的充要条件）：\\
 W(s)=c(sI-A)^{-1}b的极点全部位于s的左半平面$$
$$注：状态稳定\Rightarrow \text{BIBO}稳定\\
\qquad\qquad\qquad \not\Leftarrow \qquad\qquad\quad
（W(s)=c(sI-A)^{-1}b可能出现零极点对消）\\
\text{BIBO}稳定，且能控能观\Rightarrow 系统渐进稳定（一维系统成立）$$

## 李雅普诺夫第一法（离散系统）

$$状态稳定性（平衡状态x_e=0处渐进稳定的充要条件）：\\
系统矩阵G的所有特征值均位于单位圆内\\

\left\{\begin{array}{l}
低阶|\lambda I-G|=0解根\\
高阶|\lambda I-G|=0用劳斯判据
\end{array}\right.\\
注：状态稳定性与(zI-G)^{-1}b的根均在单位圆内有区别，可能零极点相消$$
$$
\text{BIBO}稳定性（有界输入输出稳定的充要条件）：\\
 W(s)=c(zI-G)^{-1}b的极点全部位于单位圆内$$
[离散稳定判定](#离散稳定判定)

## 非线性系统线性化判稳

$$非线性系统：\dot{x}=f(x)\\
令\dot{x}=0解得平衡点x_e\\
A=\frac{\partial f}{\partial x}\bigg|_{x_e}=
\left.\left(
\begin{array}{}
\frac{\partial f_1}{\partial x_1}&\frac{\partial f_1}{\partial x_2}&\cdots & \frac{\partial f_1}{\partial x_n}\\
\ \\
\frac{\partial f_2}{\partial x_1}&\frac{\partial f_2}{\partial x_2}&\cdots & \frac{\partial f_2}{\partial x_n}\\
\ \\
&\cdots&\cdots\\
 \ \\
\frac{\partial f_n}{\partial x_1}&\frac{\partial f_n}{\partial x_2}&\cdots & \frac{\partial f_n}{\partial x_n}\\
\end{array}
\right)\right|_{x_e}$$
$$A即为系统在平衡点处线性化后的系统矩阵\\
\ \\
渐进稳定：A的所有特征值均具有负实部\\
不稳定：A的特征值中存在正实部\\
\ \\
失效：A的特征值中存在虚根，稳定性无法根据A判断$$

## 李雅普诺夫第二法

$$平衡点x_e处的稳定性{\color{blue}（基本只考x_e=0处）}：系统在微小扰动下保持一定状态的性能\\
取正定函数V(x)\quad （仅在x_e处V(\textbf{x})=0）\\
\dot{\textbf{x}}表达式代入\dot{V}(x)
\left\{
\begin{array}{ll}
\dot{V}负定&\left\{\begin{array}{}
平衡点附近&渐进稳定\\
||x||\to \infty,V(x)\to \infty&大范围渐进稳定
\end{array}\right.\\
\dot{V}半负定&\left\{\begin{array}{}
存在\dot{V}(x)恒为零&李雅普诺夫稳定\\
除x_0=0外，\dot{V}(x)不恒为零，且||x||\to \infty,V(x)\to \infty&大范围渐进稳定
\end{array}\right.\\
\dot{V}正定&不稳定
\end{array}
\right.$$
$$仅\dot{V}(x)恒为零、\dot{V}(x)不恒为零：\\
典例（适当凑即可，考研V(x)均不难找）：\\
V(x)=2x_1^2+3x_2^2+x_3^2,\quad \dot{V}(x)=-2x_3^2\quad 半负定\\
x_1,x_2\neq0,x_3=0时，\dot{V}(x)=0，但\dot{x}_3=-2x_1^2+3x_2-x_3^2\not\equiv 0\\
即，轻微扰动下，系统无法保持\dot{V}(x)\equiv0，且||x||\to \infty,V(x)\to \infty，故系统大范围渐进稳定$$
$$注：李雅普诺夫第二法仅为充分判据，以上条件均不满足代表没找到可定性的V(x)$$

## 李雅普诺夫方程

$$线性定常连续系统的渐进稳定判据（在x_e=0处）：\\
A^TP+PA=-Q\qquad(Q一般取I)\\
解出P，若P正定，则系统大范围渐进稳定$$
$$线性定常离散系统的渐进稳定判据（在x_e=0处）：\\
G^TPG-P=-Q\qquad(Q一般取I)\\
解出P，若P正定，则系统大范围渐进稳定$$

## 极限环判定

$$非线性微分方程组为特殊凑得
\\李雅普诺夫函数一般取V(x)=\sum (x_i-x_e)^2 即可\\
\left\{\begin{array}{l}
\dot{V}(x)=0判定极限环\\
\dot{V}(x)正定、负定判定极限环稳定性
\end{array}\right.$$
[李雅普诺夫第二法](#李雅普诺夫第二法)

# ""线性定常系统综合""

## 考情分析

系统解耦不考

## 三大线性反馈控制

$$系统\Sigma(A,B,C)，假设D=0$$
$$状态反馈控制律：u=Kx+v \qquad \Sigma_K((A+BK),B,C)$$
$$输出反馈控制律：u=Hy+v=HCx+v\qquad
\Sigma_H((A+BHC),B,C)$$
$$输出到\dot{x}反馈：\dot{x}=Ax+Gy+Bu\qquad
\Sigma_G((A+GC),B,C)$$

$$注意区别：(A-BK)\quad (A-BHC)\quad (A-GC)\\
具体题型具体调整，谨记$$

## 极点配置的前提

$$定理一：状态反馈\Sigma(A+bK,b,c)对系统任意配置极点的充要条件：\Sigma(A,b,c)完全能控\\
\ \\
定理二：输出到\dot{x}的线性反馈\Sigma(A+Gc,b,c)对系统实现闭环极点任意配置的充要条件：\Sigma(A,b,c)完全能观$$

## 系统的极点配置

[T#B,!5c2fa6#离散极点配置同理]
[T#B,!275bd1#极点配置“基本”只考SISO系统  ]
$$前提：判能控、能观，满足才可任意配置极点$$
$$
直接计算{\color{blue}（维数\leqslant3）}：比较系数即可\\
|\lambda I-(A+bK)|=f^*(\lambda)\quad状态反馈的极点配置\\
|\lambda I-(A+Gc)|=f^*(\lambda)\quad 输出到\dot{x}反馈的极点配置$$
$$能控标准I型、能观标准Ⅱ型计算{\color{blue}（应试用途不大）}：\\
线性变换x=T\overline{x}，化为能控标准I型、能观标准Ⅱ型\ \Sigma(\overline{A},\overline{b},\overline{c})\\
\left.\begin{array}{l}
|\lambda I-(\overline{A}+\overline{b}\ \overline{K})|=f^*(\lambda)\quad {\color{blue}最后一行}对应还原特征多项式系数\\
|\lambda I-(\overline{A}+\overline{G}\ \overline{c})|=f^*(\lambda)\quad {\color{blue}最后一列}对应还原特征多项式系数
\end{array}\right\}友矩阵不变形（理解原理）\\
谨记线性变换回原系数阵\left\{\begin{array}{}
 K=\overline{K}T_{c1}^{-1}\\
 G=T_{o2}\overline{G}
\end{array}\right.$$
$$注：K=(k_1,k_2,\cdots,k_n)\quad
G=(g_1,g_2,\cdots,g_n)^T$$

## 系统镇定

$$系统\Sigma(A,b,c)通过极点配置使其极点均具有负实部$$

## 状态观测器原理

$$系统极点的任意配置离不开全状态变量，但系统的状态变量不都是易于观测的\\
状态观测器构造出与系统等价的全状态可观测系统，用于提供系统状态$$

## 状态观测器的可实现性

$$定理：若线性系统\Sigma(A,b,c)完全能观，则其状态矢量x可由输出y与输入u进行重构$$

## 全维状态观测器方程

[T#B,!275bd1#全维观测器“基本”只考SISO系统]
$$存在前提：判定系统\Sigma(A,b,c)能观性\\
\ \\
类似输出到\dot{x}的反馈情形\\

\dot{\widehat{x}}=A\widehat{x}  +bu + G(y-\widehat{y})\\

\dot{\widehat{x}}=(A-Gc)\widehat{x}  +bu + Gy=\underbrace{A\widehat{x}+bu+G(y-\widehat{y})}_{结构图表达式}\\
对A-Gc配置极点，解出G：|\lambda I-(A-Gc)|=f^*(\lambda)，G代入状态观测器方程即可
$$
$$注：可构造能控、能观标准型\ 全维状态观测器，与降维状态观测器线性变换处理方式相似同理，考研不太会涉及$$

## 状态观测器的渐进速度

$$
G为状态观测器的输出误差反馈矩阵，影响系统的渐进速度\\
使\widehat{x}以一定速度与精度趋近于系统真实状态x\\
默认定义：\widetilde{x}=x-\widehat{x}\quad \widetilde{y}=y-\widehat{y}\\
\begin{array}{rl}
\dot{\widetilde{x}}&=\dot{x}-\dot{\widehat{x}}\\
&=Ax+Bu-[(A-GC)\widehat{x}+Gy+Bu]\\
&=Ax-(A-GC)\widehat{x}-GCx\\
&=(A-GC)(x-\widehat{x})\\
&=(A-GC)\tilde{x}
\end{array}\\
故\tilde{x}(t)=e^{(A-GC)t}\tilde{x}(0)$$

## 降维状态观测器标准型

$$\begin{array}{}\overline{y}=(0,I)\left(\begin{array}{}
\overline{x}_1\\
\overline{x}_2
\end{array}\right)=\overline{x}_2\\
\left\{\begin{array}{}
\dot{\widehat{\overline{w}}}=(\overline{A}_{11}-\overline{G}\  \overline{A}_{21})\widehat{\overline{x}}_1+(\overline{A}_{12}-\overline{G}\ \overline{A}_{22})\overline{y}\ +(\overline{B}_1-\overline{G}\ \overline{B}_2)u \quad （“上减\overline{G}下”）\\
\widehat{\overline{x}}_1=\widehat{\overline{w}} \ +\overline{G}\ \overline{y}
\end{array}\right.
&

\end{array}

$$
$$\begin{array}{}\overline{y}=(I,0)\left(\begin{array}{}
\overline{x}_1\\
\overline{x}_2
\end{array}\right)=\overline{x}_1\\
\left\{\begin{array}{}
\dot{\widehat{\overline{w}}}=(\overline{A}_{22}-\overline{G}\  \overline{A}_{12})\widehat{\overline{x}}_2+(\overline{A}_{21}-\overline{G}\ \overline{A}_{11})\overline{y}\ +(\overline{B}_2-\overline{G}\ \overline{B}_1)u\quad （“下减\overline{G}上”）\\
\widehat{\overline{x}}_2=\widehat{\overline{w}} \ +\overline{G}\ \overline{y}
\end{array}\right.
\end{array}$$

## 降维状态观测器方程

[T#B,!275bd1#降维状态观测器“基本”只考SISO系统]
$$存在前提：判定系统\Sigma(A,b,c)能观\\
\ \\化标准型（先判断是否为标准型）：\\
x=T\overline{x}，变换矩阵T，使\overline{y}=(0,I)\overline{x}\\
T^{-1}=
\left(\begin{array}{}
C_0\\
C
\end{array}\right)\quad C_0保证T可逆即可（考试中越简单越好，主对角）\\
\left(\begin{array}{}
\dot{\overline{x}}_1\\
\dot{\overline{x}}_2
\end{array}\right)=
\left(\begin{array}{}
\overline{A}_{11}&\overline{A}_{12}\\
\overline{A}_{21}&\overline{A}_{22}
\end{array}\right)
\left(\begin{array}{}
\overline{x}_1\\
\overline{x}_2
\end{array}\right)+
\left(\begin{array}{}
\overline{B}_1\\
\overline{B}_2
\end{array}\right)u
\\
\overline{y}=(0,I)\left(\begin{array}{}
\overline{x}_1\\
\overline{x}_2
\end{array}\right)=\overline{x}_2\qquad {\color{blue}（利用I的维数区分子系统\overline{A}_{ij}的维数）}$$
$$\left\{\begin{array}{}
\dot{\widehat{\overline{w}}}_1=(\overline{A}_{11}-\overline{G}\  \overline{A}_{21})\widehat{\overline{x}}_1+(\overline{A}_{12}-\overline{G}\ \overline{A}_{22})\overline{y}\ +(\overline{B}_1-\overline{G}\ \overline{B}_2)u\qquad \textcircled{1}\\
\widehat{\overline{x}}_1=\widehat{\overline{w}} \ +\overline{G}\ \overline{y}\qquad\textcircled{2}\\
\end{array}\right.\\

对矩阵(\overline{A}_{11}-\overline{G}\  \overline{A}_{21})进行极点配置：|\lambda I-(\overline{A}_{11}-\overline{G}\ \overline{A}_{21})|=f^*(\lambda)，解得\overline{G}

$$
$$\widehat{\overline{x}}=
\left(\begin{array}{}
\widehat{\overline{x}}_1\\
\widehat{\overline{x}}_2
\end{array}\right)=
\left(\begin{array}{}
\widehat{\overline{w}}+\overline{G}\overline{y}\\
\overline{y}
\end{array}\right)\\
\widehat{x}=T\widehat{\overline{x}}=T\left(\begin{array}{}
\widehat{\overline{w}}+\overline{G}\overline{y}\\
\overline{y}
\end{array}\right)\\
画结构图时，已知系数，\textcircled{2}式代入\textcircled{1}式\\
先画\widehat{\overline{w}}的状态结构，再组合\widehat{\overline{w}},\overline{y}得\widehat{\overline{x}}，T变换得\widehat{x}$$
$$注：若系统为降维标准型，则无需进行T线性变换，运算时去掉\overline{\Delta}上的一杠符号\\
实际上\overline{y}=cT\overline{x}=cx=y$$

## 利用状态观测器实现状态反馈

$$前提：系统能控能观才可利用状态观测器进行状态反馈任意极点配置$$
$$受控系统\Sigma_0\left\{\begin{array}{l}
\dot{x}=Ax+bu\\
y=cx
\end{array}
\right.\qquad
 状态观测器\Sigma_G \left\{\begin{array}{c}
\dot{\widehat{x}}=(A-Gc)\widehat{x}+Gy+bu\\
\\
\dot{\widehat{x}}=A\widehat{x}  +bu + G(y-\widehat{y})
\end{array}
\right.\\
由于极点设计的分离性：|sI-\overline{A}|=|sI-(A+BK)||sI-(A-GC)|\\
观测器的极点、状态反馈的极点分开设计\\
\ \\
画结构图时，先绘制观测器，状态反馈最后从观测器状态变量引至输入即可
$$
$$注：
极点设计的分离性，全维、降维状态观测器均满足，无需深究\\（状态反馈在状态观测器上，而非原系统上）\\
绘制的增益G框，反馈K框等均只包含系数\\
\left\{\begin{array}{l}状态观测器特征值决定状态误差的衰减速度\\
系统特征值决定系统稳定的速度\\
\end{array}\right.（特征值仅决定衰减速度，不决定相关系数）
$$

## 极点配置典例

![](pic-theory-of-modern-control\Markji_1751378225556.png)
$$(1)\quad 写出状态空间表达式\\
(2)\quad 当所有状态变量都用于反馈时，确定合适的反馈增益，使得r(t)=1时，e_{ss}=0，且\sigma\%<3\%$$
$$(1)\quad \dot{x}=
\left(\begin{array}{}
0&1\\
0&-1
\end{array}\right)x
\qquad
b=
\left(\begin{array}{}
0\\
2
\end{array}\right)\\

\qquad\ y=
\left(\begin{array}{}
1&0
\end{array}\right)x$$
$$(2)\quad {\color{blue}题目有问题}：
e_{ss}=0转化为y_{ss}=1处理\\
f(\lambda)=|\lambda I-(A-bK)|=\lambda^2+(1+2k_2)\lambda+2k_1\\
\Phi(s)=c(sI-(A-bK))^{-1}b=\frac{2}{\lambda^2+(1+2k_2)\lambda+2k_1}\\

\left\{\begin{array}{l}
y_{ss}=\lim\limits_{s\to 0}s\cdot \Phi(s)\cdot R(s)=\frac{1}{k_1}=1\Rightarrow k_1=1\\

\sigma\%<3\%\Rightarrow \xi>0.745\Rightarrow \frac{1+2k_2}{2\sqrt{2}}>0.745\Rightarrow k_2>0.553
\end{array}\right.$$
$$两个方向
\left\{\begin{array}{l}
条件直接给出闭环极点\\
待定系数配置极点，系统特征反解参数

\end{array}\right.$$

## 非线性方程的空间表达式

![](pic-theory-of-modern-control\Markji_1751378241527.png)
![](pic-theory-of-modern-control\Markji_1751378255854.png)
$$令\left\{\begin{array}{}
x_1=x\\
x_2=\dot{x}
\end{array}\right.
则系统状态方程为
\left\{\begin{array}{l}
\dot{x}_1=x_2\\
\dot{x}_2=-x_1^2-x_2+1
\end{array}\right.\\
\ \\
求平衡点，平衡点处线性化判稳$$

# 备用知识点

## 约旦块计算

$$重特征值的子约旦块：\\
r_k(A,\lambda_i)=\text{rank}[(A-\lambda_i I)^k];\qquad r_0(A,\lambda_i)=n\\

\omega_k(A,\lambda_i)=[r_{k-1}(A,\lambda_i)-r_{k}(A,\lambda_i)];\qquad \omega_1(A,\lambda_i)表示\lambda_i对应的子约旦块个数\\\\
\omega_{k}(A,\lambda_i)-\omega_{k+1}(A,\lambda_i)：表示以\lambda_i为重特征值的k阶约旦块个数\\
\ \\
单特征值，重特征值的各个约旦块最后拼合即可$$

## 零极点对消的不确定结论

$$(sI-A)^{-1}，(sI-A)^{-1}b也可能存在零极点对消（不确定）

$$
$$影响：\\
1.\quad(sI-A)^{-1}b不一定可判断状态稳定性\\

2.\quad\Phi(t)拉氏变换(sI-A)^{-1}不一定可反解得出|sI-A|，可能零极点相消$$

## 观测器分离特性证明

$$u=v+K\widehat{x}\\
\left\{\begin{array}{rl}
\dot{x}&=Ax+Bu\\
&=Ax+BK\widehat{x}+Bv\\
&=Ax+BKx-BK(x-\widehat{x})+Bv\\
&=(A+BK)x-BK\tilde{x}+Bv
\end{array}\right.\qquad

\dot{\widetilde{x}}=(A-GC)\widetilde{x}\\
\ \\
\left(\begin{array}{}
\dot{x}\\
\dot{\tilde{x}}
\end{array}\right)=

\left(\begin{array}{}
A+BK & -BK\\
0 & A-GC
\end{array}\right)
\left(\begin{array}{}
x\\
\tilde{x}
\end{array}\right)+

\left(\begin{array}{}
B\\
0
\end{array}\right)v\\
\ \\
\left|\begin{array}{}
\lambda-(A+BK) & BK\\
0 & \lambda-(A-GC)
\end{array}\right|=0\\
\ \\
|\lambda-(A+BK)|\ |\lambda-(A-GC)|=0$$
