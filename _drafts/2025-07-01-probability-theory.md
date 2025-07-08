概率论与数理统计

概率论与数理统计内容不多，概念性较弱，主要考察点在计算量

# 默认章节

## 考情分析

选择题：3道
填空题：1道
大题：1道（多元随机变量+点估计）

难度近几年持平

## 考查轻重点讨论

重点：
一维、二维随机变量及其分布，数字特征，参数估计
偏冷、较繁：
假设检验
难点：
古典概型

计算不复杂，但计算量很大，易算错，一步错步步错

# 随机事件与概率

## 考情分析

古典概型较难，但考查不深，若计算复杂，考虑处理复杂化了
重点：事件的运算、条件概率与全概率、贝叶斯公式

## 随机事件重要运算公式

**关键在集合运算，而非代数运算**
$$结合律：\\
(A\cup B)\cup C=A\cup (B\cup C)=A\cup B\cup C\\
(A\cap B)\cap C=A\cap (B\cap C)=A\cap B\cap C\\
\ \\
分配律：\\
A\cup (B\cap C)=(A\cup B)\cap (A\cup C)\\
A\cap (B\cup C)=(A\cap B)\cup (A\cap C)\\
\ \\
对偶律：\\
\overline{A\cup B}=\overline{A}\cap \overline{B};
\overline{A\cap B}=\overline{A}\cup \overline{B}$$
$$注：\\
AB=A\cap B\\
A+B=A\cup B\\
A-B=A\overline{B}=A-AB\quad{\color{blue}\neq A+\overline{B}}\\
（加减运算易出错，慎用）$$

## 事件关系

$$AB与\overline{A}B互斥\\
AB=A\Leftrightarrow A\subset B\Leftrightarrow A\cup B=B\\
AB=\varnothing\Leftrightarrow A\subset\overline{B}或B\subset\overline{A}$$

## 概率重要运算公式

**善用概率运算关系简化计算，逆事件可简化计算，灵活使用**
$$减法公式：P(\overline{A})=1-P(A),P(A-B)=P(A\overline{B})=P(A)-P(AB)\\
加法公式：P(A\cup B\cup C)=\\
P(A)+P(B)+P(C)-P(AB)-P(AC)-P(BC)+P(ABC)（奇正偶负，各维同理）$$
$$条件概率公式：P(A|B)=\frac{P(AB)}{P(B)}\quad (定义P(B)>0)（划分范围,运算公式依旧满足）\\
\begin{array}{ll}
P(\overline{B}|A)=1-P(B|A)&\quad (P(A)>0)\\
P(B-C|A)=P(B|A)-P(BC|A)&\quad(P(A)>0)\\
 P(B\cup C|A)=P(B|A)+P(C|A)-P(BC|A)&\quad(P(A)>0)\\
\end{array}
（仅加减可按“划分范围”理解，独立不可）
\ \\
乘法公式：P(A_1A_2\cdots A_n)=P(A_1)P(A_2|A_1)P(A_3|A_1A_2)\cdots P(A_n|A_1A_2\cdots A_{n-1})\quad (P(A_1A_2\cdots A_{n-1})>0)$$

## 全概率公式与贝叶斯公式

**有因有果，分两步走，特征明显，“因果”，敏锐察觉**
$$全概率公式：某条件的概率与该条件下事件发生概率之积求和\\
P(B)=\sum_{i=1}^{n}P(BA_i)=\sum_{i=1}^{n}P(A_i)P(B|A_i)\qquad （由因索果）\\

$$
$$贝叶斯公式：P(A_j|B)=\frac{P(A_jB)}{P(B)}=\frac{P(A_j)P(B|A_j)}{\sum_{i=1}^{n}P(A_i)P(B|A_i)}\quad（由果索因）$$

## 概率运算重要结论

$$P(AB)\leqslant \{P(A),P(B)\}（概率越积越小）\\
P(A\cup B)\geqslant \{P(A),P(B)\}$$

## 随机事件独立的定义

$$设A_1,A_2,\cdots,A_n为n个事件（有限个），若对其中任意个事件
A_{1_i},A_{2_i},\cdots,A_{n_i}(2\leqslant k\leqslant n)，有\\
\ \\
P(A_{1_i},A_{2_i},\cdots,A_{n_i})=P(A_{1_i})(A_{2_i})\cdots P(A_{n_i})\\
\ \\
则称n个事件A_1,A_2,\cdots,A_n相互独立$$

## 随机事件独立的性质

$$1.A与B,A与\overline{B},\overline{A}与B,\overline{A}与\overline{B}中任意一对相互独立，则其余三对相互独立\\
注：P(A\overline{B})=P(A)-P(AB)=P(A)-P(A)P(B)=P(A)[1-P(B)]（可类比推广）\\
\ \\
2.若A,B,C,D相互独立，则AB与C\overline{D}相互独立，但AB与\overline{BCD}\textbf{不一定}相互独立（B，\overline{B}代表同一元素）\\
注：A_i与B_j相互独立，则\sigma_1(\sum A_i)与\sigma_2(\sum B_j)相互独立，反之不然（\sigma代表事件组合）\\
\ \\
3.若P(A)=0或P(A)=1，则事件A与任意事件独立

$$

## 独立与相容、互斥的关系

$$A,B独立\left\{
\begin{array}{l}P(A)>0,P(B)>0\Rightarrow AB\neq \varnothing\\
P(A)=0或P(B)=0 \quad未知
\end{array}
\right.\\
\ \\
P(A)>0,P(B)>0
\left\{
\begin{array}{l}
AB=\varnothing
\Rightarrow A与B互不独立\\
A\subset B\Rightarrow A与B互不独立
\end{array}
\right.\\
$$
$$注：\\
P(A)=0,1的事件较特别，举反例时常用\\
A=\varnothing\ \substack{\Rightarrow\\ \not\Leftarrow}\ P(A)=0;\quad A=\Omega\ \substack{\Rightarrow\\ \not\Leftarrow}\ P(A)=1$$

## 独立的充要条件

**回归至定义证**
$$\quad\ P(AB)=P(A)P(B)\\
\Leftrightarrow P(B|A)=P(B)\quad (P(A)>0)\\
\Leftrightarrow P(B|A)=P(B|\overline{A})\quad (0<P(A)<1)\\
\Leftrightarrow P(B|A)+P(\overline{B}|\overline{A})=1\quad(0<P(A)<1)$$

$$\Leftrightarrow P(AB)=P(A)P(B)$$
$$\Leftrightarrow P(A|B)=P(A)\quad (P(A)>0)\\
(\Leftarrow)P(AB)=P(B)P(A|B)=P(A)P(B)$$
$$\Leftrightarrow P(B|A)=P(B|\overline{A})\quad (0<P(A)<1)\\
(\Leftrightarrow) \frac{P(AB)}{P(A)}=\frac{P(B)-P(AB)}{1-P(A)}\\
(\Leftrightarrow)P(AB)-P(AB)P(A)=P(A)P(B)-P(A)P(AB)\\
(\Leftrightarrow)P(AB)=P(A)P(B)$$
$$\Leftrightarrow P(B|A)+P(\overline{B}|\overline{A})=1\quad(0<P(A)<1)\\
(\Leftrightarrow)P(B|A)=1-P(\overline{B}|\overline{A})\\
(\Leftrightarrow)P(B|A)=P(B|\overline{A})\\
(\Leftrightarrow)......$$

## 事件概率不等式

$$P(A)\leqslant P(A|B)\\
\begin{array}{ll}
P(A|B)=1&\Rightarrow P(A)\geqslant P(B)\\
&\not\Rightarrow B\subset A
\end{array}$$

## 古典概型总述

**“有序”古典概型考察不深，先考虑“无序”能否做**
$$\begin{array}{ll}组合C_N^n=\frac{P_N^n}{n!}（去序）& C_N^n=C_N^{(N-n)}\\
\\
排列P_N^n=\frac{N!}{(N-n)!}（去尾）
\end{array}
$$
$$古典概型关键：\frac{事件样本点数}{样本空间的样本点数}（通用思路，具体问题具体分析，较灵活）\\
\ \\
（总体考虑顺序，则事件考虑顺序，一致即可）
$$
$$注：难在题义的转化$$

## 古典概型-随机分配

$$随机分配（质点选盒子）： N代表盒数，n代表质点数\\
\begin{array}{cc}
分配方式&总体\Omega\\
每盒可容纳任意多质点（有序）&N^n\\
每盒可容纳至多一个质点（有序）&P_N^n\\
\end{array}
$$
$$\star\star组合排列\\
9个A，3个B，随机均分到3个盒子\\
1)每个盒子各含一个B\qquad
P=\frac{3!\times C_9^3C_6^3C_3^3}{C_{12}^4C_8^4C_4^4}（组间含排列）\\
2)3个B均在一个盒子\qquad P=\frac{C_3^1\times C_9^4C_5^4}{C_{12}^4C_8^4C_4^4}（组间含排列）$$
$$注：\\
“质点”与“盒”勿颠倒\\
\star\ 质点与质点之间是不同的\\
“同质”:排列即可，勿“重复排列”$$

## 古典概型-简单随机抽样

$$简单随机抽样：N代表总质点数，n代表抽取次数\\
 \qquad\qquad
\begin{array}{cc}
抽样方式&总体\Omega\\
先后有放回取n次（有序）&N^n\\
先后无放回去n次（有序）&P_N^n\\
任取n个（无序）&C_N^n\\
\end{array}$$
$$8良，2坏，逐个检测，不超过4次检测出\\
\frac{C_8^2\cdot C_2^2}{C_{10}^4}\qquad （按无序处理，简化模型）$$
$$注：
\star\ 红球与红球之间是不同的\\

$$

## 条件概率概型

$$P(A_1A_2\cdots A_n)=P(A_1)P(A_2|A_1)P(A_3|A_1A_2)\cdots P(A_n|A_1A_2\cdots A_{n-1})\quad (条件的概率 >0)\\
\ \\
\left\{
\begin{array}{l}
无放回概型\\
“放回但有影响”概型
\end{array}
\right.$$

## 重要古典概型题型

$$抓阄模型：\\
4个白球，6个红球\\
先后无放回取n次，各次取到白球概率均为\frac{4}{10}$$

## 古典概型与二项分布相通概型

**相当于伯努利概型**
$$
红球3个，白球4个，先后放回取6个，取2红4白的概率\\
\frac{C_6^2\cdot3^2\cdot 4^4}{7^6}=C_6^2(\frac{3}{7})^2(\frac{4}{7})^4$$

# 一维随机变量

## 考情分析

重难点：分布函数法求函数分布、概率密度

## 分布函数的充要条件与性质

$$F(x)=P(X\leqslant x),\quad F(x)=\int_{-\infty}^xf(x)dx $$
$$充要条件：\\
\Leftrightarrow F(x)单调不减\\
\quad\ F(x)右连续\\
\quad\ {\color{blue}F(-\infty)=0,F(+\infty)=1}\\
\quad\ 0\leqslant F(x)\leqslant 1\\（前三条为最简条件）$$
$$性质：\\
P(x_1<X\leqslant x_2)=F(x_2)-F(x_1)\\
P(X=x)=F(x)-F(x-0)（连续时为0）$$
$$分布函数：F^2(x),\quad F_1(x)F_2(x)\\
1-[1-F(x)]^k,\quad 1-[1-F_1(x)][1-F_2(x)]\cdots$$

## 分布律、概率密度的充要条件

$$分布律：\\
0\leqslant p_i\leqslant 1;\\
\sum_ip_i=1$$
$$概率密度：\\
\left\{
\begin{array}{l}
f(x)\geqslant 0;\\
\int_{-\infty}^{+\infty}f(x)dx=1
\end{array}
\right.\\
\ \\
定义法：\\
 f(x)=F'(x)或\int_{-\infty}^xf(x)dx=F(x)，其中F(x)为分布函数$$
$$注：
概率密度：2f(x)F(x),\quad f_1(x)F_2(x)+f_2(x)F_1(x)$$

## 常用离散型分布及其期望、方差
$$0-1分布B(1,p)\\
二项分布B(n,p)\\
泊松分布P(\lambda)\\
几何分布G(p)\\
\sout{超几何分布H(n,N,M)}

$$

**注意起始项k**
$$\begin{array}{cccc}
& 分布列 & 期望 & 方差\\
\\
0-1分布 & P\{X=k\}=(1-p)^{1-k}p^k,k=0,1 & p & p(1-p)\\
\\
\begin{array}{c}二项分布\\B(n,p) \end{array}& P\{X=k\}=C_n^k(1-p)^{n-k}p^k,k=0,1,\cdots,n & np & np(1-p)\\
\\
\begin{array}{c}泊松分布\\P(\lambda) \end{array}& P\{X=k\}=\frac{\lambda^k}{k!}e^{-\lambda},k=0,1,\cdots & \lambda & \lambda&(\lambda>0)\\
\\
\begin{array}{c}几何分布\\G(p) \end{array}& P\{X=k\}=(1-p)^{k-1}p,k=1,2,\cdots & \frac{1}{p} & \frac{1-p}{p^2}\\
\\
\begin{array}{c}超几何分布\\H(n,N,M) \end{array} & P\{X=k\}=\frac{C_M^k C_{N-M}^{n-k}}{C_N^n} & \backslash& \backslash
\end{array}$$

## 常用连续型分布及其期望、方差
$$正态分布N(\mu,\sigma^2)\\
均匀分布U(a,b)\\
指数分布E(\lambda)$$

$$\begin{array}{ccccc}
& 概率密度 & 分布函数 & 期望 & 方差\\
\\
\begin{array}{c}正态分布\\N(\mu,\sigma^2)\end{array} &\begin{array}{c} f(x)=\frac{1}{\sqrt{2\pi}\sigma}e^{-\frac{(x-\mu)^2}{2\sigma^2}},-\infty<x<+\infty\end{array} &\Phi(x)& \mu & \sigma^2\\
\\
\begin{array}{c}均匀分布\\U(a,b) \end{array} & f(x)=\left\{\begin{array}{cl}\frac{1}{b-a},&a<x<b \\ \\ 0,&其他\end{array}\right.& F(x)=\left\{\begin{array}{cl}0,&x<a\\\\\frac{x-a}{b-a},&a\leqslant x<b\\\\ 1,& x\geqslant b\end{array}\right.&\frac{a+b}{2} & \frac{(b-a)^2}{12}\\
\\
\begin{array}{c}指数分布\\E(\lambda)\end{array} & f(x)=\left\{\begin{array}{cl}\lambda e^{-\lambda x},&x>0 \\ \\ 0,&其他\end{array}\right.&F(x)=\left\{\begin{array}{cl}1-e^{-\lambda x},&x\geqslant0 \\ \\ 0,&x<0\end{array}\right.& \frac{1}{\lambda}& \frac{1}{\lambda^2}&(\lambda>0)
\end{array}$$

## 泊松定理（二项分布与泊松分布）

$$若\lim\limits_{n\to \infty}np_n=\lambda>0,则对任意非负整数k,有\\
\lim\limits_{n\to \infty}C_n^kp_n^k(1-p_n)^{n-k}=\frac{\lambda^k }{k!}e^{-\lambda}\qquad 且\sum_{k=0}^{\infty}\frac{\lambda^k }{k!}e^{-\lambda}=e^{-\lambda}\sum_{k=0}^{\infty}\frac{\lambda^k }{k!}=1\\
$$
$$注：
当n很大，p很小时，二项分布可用泊松分布近似$$

## 泊松过程（泊松分布与指数分布）

$$t时间内发生k次的概率：\\
P\{N(t)=k\}=\frac{(\lambda t)^k}{k!}e^{-\lambda t}\quad \lambda t为t时间内的数学期望\\
$$
$$泊松分布：t=1时间内发生k次的概率\\
t=1\quad P\{N(1)=k\}=\frac{\lambda^k}{k!}e^{-\lambda }\\
指数分布：t时间内一次也没有发生的概率\\
k=0\quad P\{T<t\}=1-P\{N(t)=0\}=1-e^{-\lambda t}$$

## 分布的无记忆性

$$关键：P\{X>m+k\}=P\{X>k\}P\{X>m\}（条件必须取“>”号）\\
有且仅有几何分布、指数分布有无记忆性$$
$$几何分布：\\
P\{X=m+k|X>m\}=P\{X=k\}\qquad P\{X=m+k\}=P\{X>m\}P\{X=k\}=(1-p)^m\cdot (1-p)^{k-1}p\\
P\{X>m+k|X>m\}=P\{X>k\}\qquad P\{X>m+k\}=P\{X>m\}P\{X>k\}=(1-p)^m\cdot (1-p)^k\\
（n重伯努利实验每次实验均独立）
$$
$$指数分布：\\
P\{X\geqslant t+s|X\geqslant t\}=P\{X\geqslant s\}\qquad
P\{X\geqslant t+s\}=P\{X\geqslant t\}P\{X\geqslant s\}=e^{-\lambda t}\cdot e^{-\lambda s}\\

（元件无损耗才有无记忆性）$$
$$注：
泊松分布不满足无记忆性$$

## 连续型分布的性质

$$必要条件：
F(x)连续$$

## 正态分布的性质

$$1.X\sim N(\mu,\sigma^2)\Rightarrow aX+b\sim N(a\mu+b,a^2\sigma^2)\\
2.X\sim N(\mu_1,\sigma_1^2),Y\sim N(\mu_2,\sigma_2^2)
\left\{\begin{array}{l}\xRightarrow{X,Y相互独立} aX+bY\sim N(a\mu_1+b\mu_2,a^2\sigma^2+b^2\sigma^2)\\
\not\xRightarrow {X,Y不相互独立}aX+bY\sim N
\end{array}\right.\\
3.标准化：X\sim N(\mu,\sigma^2),则\frac{X-\mu}{\sigma}\sim N(0,1)$$
![](pic-probability-theory\Markji_1751362016607.png)
$$\mu为对称轴位置，\frac{1}{\sqrt{2\pi}\sigma}为图像高度$$

## 一维随机变量重要经验

离散型分布注意合理设事件

## 由F(x)求f(x)问题

$$F(x)=\int_{-\infty}^xf(t)dt（所涉不深，勿深究）$$
$$已知F(x)，直接求导即可\\
\left\{
\begin{array}{l}
F'(x)连续区间，f(x)即为所求\\
F'(x)不存在点处，左右极限按区间分开即可
\end{array}
\right.$$

## 连续型随机变量函数的分布

$$Y=g(X)单调:公式法\\
y=g(x)的反函数x=g^{-1}(y)=h(y)\\

f_Y(y)=
\left\{
\begin{array}{cl}
f_X[h(y)]|h'(y)|&,a<y<b\quad（x有效范围对应至y的有效范围）\\
0&,其他
\end{array}
\right.$$
$$注：\begin{array}{l}
g(x)单增：F_Y(y)=P\{Y\leqslant y\}=P\{g(X)\leqslant y\}=P\{X\leqslant g^{-1}(y)\}=F_X[g^{-1}(y)]\\
g(x)单减：F_Y(y)=P\{Y\leqslant y\}=P\{g(X)\leqslant y\}=P\{X\geqslant g^{-1}(y)\}=1-F_X[g^{-1}(y)]
\end{array}$$
$$Y=g(X)不单调：分布函数法\\
F_Y(y)=\int_{\varphi_1(y)}^{\varphi_2(y)} f(x)dx$$

## 分段函数的函数分布

**对应区间积分即可，对应好变量范围**
$$Y=\left\{
\begin{array}{cc}
2,&X\leqslant 1\\
3X,&1<X<2\\
1,&X\geqslant 2
\end{array}
\right.$$
$$\left\{
\begin{array}{cc}
\int_{-\infty}^1f(x)dx &y=2\\
\int_2^{+\infty}f(x)dx &y=1\\
\int_1^{\frac{y}{3}}f(x)dx &  3<y<6 & \qquad 关键：P\{3<Y<y\}=P\{1<X<\frac{y}{3}\}
\end{array}
\right.$$

## 重要结论

$$Y=F(X)（F(x)是X的分布函数）与X的概率密度无关\\
且Y=F(X)在[0,1]上服从均匀分布$$

## 一维随机变量处理技巧

$$典例：区间(0,2)上随机取一点，将区间分为两段，较短的一段记为X\\
X=\min\{W,2-W\}\quad即 0<x<1\quad 记W为该点位置\\F(x)=P\{\min\{W,2-W\}\leqslant x\}\\
\qquad\ =1-P\{\min\{W,2-W\}>x\}\\
\qquad\ =1-P\{W>x,2-W>x\}\\
\qquad\ =1-P\{x<W<2-x\}\\
\qquad \ =1-\frac{(2-x)-x}{2}\\
\qquad \ =x$$

## 连续型书写规范

$$F(x)=
\left\{
\begin{array}{l}
\cdots,a\leqslant x <b（分布函数，右连续，左闭右开）\\
0,其他
\end{array}
\right.\\
\ \\
 f(x)=
\left\{
\begin{array}{l}
\cdots,\cdots（概率密度对右连续无要求，开区间） \\
0,其他
\end{array}
\right.\\
\ \\
连续型分布函数与概率密度定义域均为(-\infty,+\infty)$$

# 二维随机变量

## 考情分析

重难点：
多维随机变量函数的分布、独立性的判断与使用（区间讨论略难）
分布函数法求函数分布、概率密度

## 二维离散型随机变量分布

$$联合概率分布：\\
P(X=x_i,Y=y_j)=p_{ij}\\
边缘概率分布：\\
P(X=x_i)=\sum_{j=1}^{\infty}p_{ij}=p_{i\cdot}\\
条件概率分布：\\
P(X=x_i|Y=y_j)=\frac{P(X=x_i,Y=y_j)}{P(Y=y_j)}=\frac{p_{ij}}{p_{\cdot j}}\quad(p_{\cdot j}>0)\\
联合分布函数：\\
F(x,y)=\sum_{x_i\leqslant x}\sum_{y_j\leqslant y} p_{ij}

$$

## 二维连续型随机变量分布

$$联合概率密度：\\
f(x,y)=\frac{\partial^2F(x,y)}{\partial x\partial y}（f(x,y)连续处）\\
\begin{array}{ll}
边缘分布函数：&边缘概率密度：\\
F_X(x)=\int_{-\infty}^{x}du\int_{-\infty}^{+\infty}f(u,y)dy={\color{blue}F(x,+\infty)}
&f_X(x)=\int_{-\infty}^{+\infty}f(x,y)dy\\
条件分布函数：&条件概率密度：\\
F_{X|Y}(x|y)=\int_{-\infty}^x\frac{f(u,y)}{f_Y(y)}du\quad (f_Y(y)>0)
&
f_{X|Y}(x|y)=\frac{f(x,y)}{f_Y(y)}\quad (f_Y(y)>0)
\end{array}\\
联合概率分布：\\
F(x,y)=\int_{-\infty}^{x}\int_{-\infty}^{y}f(u,v)dudv$$

## 二维条件概率理解

**先有条件分布函数，后有条件概率密度**
$$条件分布函数：\\
F_{X|Y}(x|y)=\int_{-\infty}^x\frac{f(u,y)}{f_Y(y)}du\quad (f_Y(y)>0)\\
（已知事件Y=y发生的条件下F(x,y)的概率，“线积分”）\\
\ \\
条件概率密度：\\
f_{X|Y}(x|y)=\frac{f(x,y)}{f_Y(y)}\quad (f_Y(y)>0)$$

## 联合分布函数的充要条件

$$充要条件：\\
\Leftrightarrow F(x,y)单调不减\\
\quad\ F(x,y)是x,y的右连续函数\\
\quad\ {\color{blue}F(-\infty,y)=F(x,-\infty)=F(-\infty,-\infty)=0,F(+\infty,+\infty)=1}\\
\quad\ 0\leqslant F(x,y)\leqslant 1\\（前三条为最简条件）$$
$$性质：\\
P\{x_1<X\leqslant x_2,y_1<Y\leqslant y_2\}=F(x_2,y_2)-F(x_1,y_2)-F(x_2,y_1)+F(x_1,y_1)$$

## 联合分布律、联合概率密度的充要条件

$$联合分布律：\\
0\leqslant p_{ij}\leqslant 1;\\
\sum_i\sum_j p_{ij}=1$$
$$联合概率密度：\\
f(x,y)\geqslant 0;\\
\int_{-\infty}^{+\infty}\int_{-\infty}^{+\infty}f(x,y)dxdy=1$$

## 多维随机变量独立的充要条件

**定义式：**
$$\begin{array}{ll}
\forall (x,y)\quad& F(x,y)=F_X(x)\cdot F_Y(y)\\
\forall (x_1,x_2,\cdots,x_n)\quad&F(x_1,x_2,\cdots,x_n)=F(x_1)F(x_2)\cdots F(x_n)\\
&{\color{blue}（含任意变量，与事件独立有区别）}

\end{array}$$
**充要条件:**
$$离散型\quad \forall x_i,y_i\\
\Leftrightarrow P\{X=x_i,Y=y_j\}=P(X=x_i)\cdot P(Y=y_j)\\
\Leftrightarrow P(X=x_i|Y=y_j)=P(X=x_i)\ 或\ P(Y=y_i|X=x_j)=P(Y=y_j)\quad(P(Y=y_j),P(X=x_i)>0)\\
\Leftrightarrow P\{X_1=x_1,\cdots,X_n=x_n\}=\prod_{i=1}^{n}P(X=x_1)\\
\ \\
连续型\\
\Leftrightarrow f(x,y)=f_X(x)\cdot f_Y(y)\\
\Leftrightarrow f_{X|Y}(x|y)=f_X(x)\ 或\ f_{Y|X}(y|x)=f_Y(y)\quad (f_Y(y),f_X(x)>0)\\
\Leftrightarrow f(x_1,x_2,\cdots,x_n)=\prod_{i=1}^{n}f_i(x_i)
$$

## 多维随机变量独立的性质

$$若X_1,X_2,\cdots,X_n相互独立，则\\
其中任意k(2\leqslant k\leqslant n)个随机变量相互独立\\
$$
$$若X_1,X_2,\cdots,X_n相互独立，且g_1(x),g_2(x),\cdots,g_n(x)连续（有效区间连续即可），则\\
g_1(X_1),g_2(X_2),\cdots,g_n(X_n)相互独立，反之不然
$$
$$注：
变量独立与否与变量有无复用无必然联系$$

## 二维正态分布
$$(X,Y)\sim N(\mu_1,\mu_2;\sigma_1^2,\sigma_2^2;\rho)$$

$$f(x,y)=\frac{1}{2\pi \sigma_1\sigma_2\sqrt{1-\rho^2}}e^{-\frac{1}{2(1-\rho^2)}[(\frac{x-\mu_1}{\sigma_1})^2-2\rho(\frac{x-\mu_1}{\sigma_1})(\frac{y-\mu_2}{\sigma_2})+(\frac{y-\mu_2}{\sigma_2})^2]},\quad(\sigma_1,\sigma_2>0,-1<\rho<1)$$
$$
性质：\\
\rho=0\Leftrightarrow X与Y相互独立\Leftrightarrow (X,Y)\sim N(\mu_1,\mu_2,\sigma_1,\sigma_2,0)\\
\ \\
X\sim N(\mu_1,\sigma_1^2)
,\quad Y\sim N(\mu_2,\sigma_2^2)\\

\ \\
D(aX+bY)=a^2DX+b^2DY+2ab\ \rho\sigma_1\sigma_2\\
\ \\
aX+bY\sim N(a\mu_1+b\mu_2,a^2\sigma_1^2+b^2\sigma_2^2+2ab\ \rho\sigma_1\sigma_2)\\
\ \\
f_{X|Y}(x|y)\sim N,\quad f_{Y|X}(y|x)\sim N\\
\ \\
\left\{
\begin{array}{l}
U=aX+bY\\
V=cX+dY
\end{array}
\right.且
\left|
\begin{array}{}
a&b\\
c&d
\end{array}
\right|\neq0,则U,V\sim N\\
\left|
\begin{array}{}
a&b\\
c&d
\end{array}
\right|=0,则U,V满足线性关系$$

## 二维正态分布积分技巧

$$\int_{-\infty}^{+\infty}dy\int_{-\infty}^{+\infty}e^{-2x^2+2xy-y^2}dx=\int_{-\infty}^{+\infty}e^{-x^2}dx\int_{-\infty}^{+\infty}e^{-(y-x)^2}d(y-x)$$

## 重要经验

涉及二维，先求联合分布律或联合概率密度
涉及连续型分布、概率密度，谨慎注意有效区间，切记标注有效区间，否则意义不同，如：计算条件概率密度

## 重要结论

$$X为离散型（有限个），Y为连续型，X+Y为连续型\\
P\{X+Y=t_0\}=\sum P\{X+Y=t_0,X=x_i\}\leqslant \sum  P\{Y=t_0-x_i\}=0$$
$$f(x,y)=\left\{
\begin{array}{cl}
g(x)\cdot f(y),\quad &a<x<b,c<y<d\\
0,&其他
\end{array}
\right.\substack{\Rightarrow \\ \not\Leftarrow }\ X,Y相互独立$$

## 二维重要积分技巧

$$I=\iint\limits_{D}e^{-x^2}dxdy
=\iint\limits_{D} e^{-r^2}rdrd\theta
=\cdots$$

## 常见分布可加性

$$X,Y相互独立\\
X\sim B(n,p),Y\sim B(m,p),则X+Y\sim B(m+n,p)\\
X\sim P(\lambda_1),Y\sim P(\lambda_2),则X+Y\sim P(\lambda_1+\lambda_2)\\
X\sim N(\mu_1,\sigma_1^2),Y\sim N(\mu_2,\sigma_2^2),则X+Y\sim N(\mu_1+\mu_2,\sigma_1^2+\sigma_2^2)\\
X\sim \chi^2(n),Y\sim \chi^2(m),则X+Y\sim \chi^2(m+n)$$
$$注：谨记--非线性叠加性\\
X\sim B(n,p),\quad aX\not\sim B(n,p)且aX\not\sim B(an,p)\\
其余分布同理，仅起到系数的作用，不影响变量分布，X\sim N(\mu,\sigma^2)除外$$

## 卷积公式

$$Z=X+Y\qquad f_Z(z)=\int_{-\infty}^{+\infty}f(x,z-x)dx=\int_{-\infty}^{+\infty}f(z-y,y)dy\\
Z=X-Y\qquad f_Z(z)=\int_{-\infty}^{+\infty}f(x,x-z)dx=\int_{-\infty}^{+\infty}f(y+z,y)dy\\
Z=XY\qquad f_Z(z)=\int_{-\infty}^{+\infty}\frac{1}{|x|}f(x,\frac{z}{x})dx=\int_{-\infty}^{+\infty}\frac{1}{|y|}f(\frac{z}{y},y)dy\\
Z=\frac{X}{Y}\qquad f_Z(z)=\int_{-\infty}^{+\infty}|y|f(yz,y)dy
$$
$$推导原理：\\
F_{Z}(z)=P\{X+Y\leqslant z\}=P\{Y\leqslant z-X\}=\int_{-\infty}^{+\infty}dx \int_{-\infty}^{z-x}f(x,y)dy\\
f_{Z}(z)=F_{Z}'(z)=\int_{-\infty}^{+\infty} f(x,z-x)dx$$

## 离散型、连续型求函数分布、概率密度

$$离散型：对应项相加即可$$
$$连续型：\\
1.画出联合概率密度的有效区间\\
2.分段讨论z不同范围下的积分\\
$$
$$注：\\
Z=X+Y,Z=X-Y移项即可画出积分区域\\
Z=\frac{Y}{X}分类讨论X,z正负即可画出积分区域\\
Z=XY分类讨论X,z的正负可画出积分区域\\
Z=|X-Y|双斜线中间区域$$

## 二维随机变量函数的分布处理技巧

$$F(x,y)=P\{X\leqslant x,Y\leqslant y\}（善用事件运算）$$
$$Z=\max(X,Y):\\
(X,Y)\sim F(X,Y),则\\
F_Z(z)=P(\max(X,Y)\leqslant z)=P(X\leqslant x,Y\leqslant y)=F(z,z)\\
当X与Y独立时,F_Z(z)=F_X(z)\cdot F_Y(z)\\
n维独立同分布，F_Z(z)=[F_X(z)]^n;\quad f_Z(z)=n[F_X(z)]^{n-1}f_X(z)$$
$$Z=\min(X,Y):\\
(X,Y)\sim F(X,Y),则\\
\begin{array}{rl}
F_Z(z)=&P(\min(X,Y)\leqslant z)=1-P(\min(X,Y)\geqslant z)=1-P(X\geqslant x,Y\geqslant y)\\
=&P\{(X\leqslant z)\cup(Y\leqslant z)\}
=P(X\leqslant z)+P(Y\leqslant z)-P(X\leqslant z,Y\leqslant z)
=F_X(z)+F_Y(z)-F(z,z)
\end{array}\\
当X与Y独立时,F_Z(z)=1-P(X\geqslant x,Y\geqslant y)=1-[(1-F_X(z))(1-F_Y(z))]\\
n维独立同分布，F_Z(z)=1-[1-F_X(z)]^n;\quad f_Z(z)=n[1-F_X(z)]^{n-1}f_X(z)$$
$$P\{2< \min\{X,Y\}\leqslant 3\}=P\{\min\{X,Y\}\leqslant 3\}-P\{\min\{X,Y\}\leqslant 2\}\\
P\{\max\{X_1,X_2,X_3\}\leqslant X_4\}=P\{Y\leqslant X_4\}（X_i间相互独立，利用联合概率密度函数分布计算）$$
$$\max\{X,Y\}=\frac{X+Y+|X-Y|}{2},\quad \min\{X,Y\}=\frac{X+Y-|X-Y|}{2}\\
\max\{X,Y\}+ \min\{X,Y\}=X+Y,\quad \max\{X,Y\}\cdot \min\{X,Y\}=X\cdot Y$$
$${\color{blue}若无法处理，直接计算函数分布，利用新分布计算}$$

## 二维连续型分布函数的区间分段讨论

$$五个区间分段讨论：\\
有效区间左方、下方\rightarrow 有效区间
\begin{array}{l}
\rightarrow 有效区间右方\\
\rightarrow 有效区间上方\\
\rightarrow 有效区间右上方
\end{array}$$

## 混合型求函数分布、概率密度

**全概率公式、分布函数法**
$$一般X，Y相互独立\\
F_Z(z)=  P\{X+Y\leqslant z,Y=-1\}+P\{X+Y\leqslant z,Y=1\}\\
=P\{X\leqslant z+1,Y=-1\}+P\{X\leqslant z-1,Y=1\}\\
=F_X(z+1)P(Y=-1)+F_X(z-1)P(Y=1)
$$
$$F_Z(z)= P\{XY\leqslant z,Y=0\}+P\{XY\leqslant z,Y=1\}\\
=P\{z\geqslant 0,Y=0\}+P\{X\leqslant z,Y=1\}\\
=P\{z\geqslant 0\}P\{Y=0\}+P\{X\leqslant z\}P\{Y=1\}\\
F_Z(z)=\left\{\begin{array}{l}
P\{X\leqslant z\}P\{Y=1\},&z<0\\
\ \\
P\{Y=0\}+P\{X\leqslant z\}P\{Y=1\},&z\geqslant 0\end{array}\right.$$
$$注：
X,Y相互独立，不是X+Y,Y相互独立$$

# 随机变量数字特征

## 考情分析

数字特征主要考察计算
归根结底在期望E(x)的计算

## 期望的定义

$$离散型：若\sum_{i=1}^{\infty}x_ip_i绝对收敛，则EX=\sum_{i=1}^{\infty}x_ip_i（若为可列无限个，级数改变次序，值不变）\\
E[g(X)]=\sum_{i=1}^{\infty}g(x_i)p_{i}\quad E[g(X,Y)]=\sum_{i=1}^{\infty}\sum_{j=1}^{\infty}g(x_i,y_j)p_{ij}$$
$$连续型：若\int_{-\infty}^{+\infty}xf(x)dx绝对收敛，则EX=\int_{-\infty}^{+\infty}xf(x)dx\\
E[g(X)]=\int_{-\infty}^{+\infty}g(x)f(x)dx\quad E[g(X,Y)]=\int_{-\infty}^{+\infty}\int_{-\infty}^{+\infty} g(x,y)f(x,y)dxdy$$
$$注：绝对收敛知道即可，不作考查$$

## 期望的性质

$$Ec=c,\quad E(aX+c)=aEX+c,\quad E(aX+ bY)=aEX+ bEY（线性叠加性）\\
E[f(X)+ g(Y)]=E[f(X)]+ E[g(Y)]（叠加性）$$
$$X,Y相互独立：\\
E(XY)=EX\cdot EY\\
E[f(X)g(Y)]=E[f(X)]E[g(Y)],其中f(x),g(x)连续（针对连续型）$$

## 方差的性质

$$DX=E[(X-EX)^2]=E(X^2)-(EX)^2$$
$$DX\geqslant 0,\quad E(X^2)=DX+(EX)^2\geqslant0\\
Dc=0,\quad D(aX+c)=a^2DX,\quad D(aX+bY)=a^2DX+b^2DY+2\text{Co}v(aX,bY)\\
D[f(X)+g(Y)]=D[f(X)]+D[g(Y)]+2\text{Cov}[f(X),g(Y)]（叠加性）\\
\ \\
DX=E[(X-EX)^2]\leqslant E[(X-c)^2]（c为任意常数）$$
$$X,Y相互独立:\\
D(aX+bY)=a^2DX+b^2DY\\
D[f(X)+g(Y)]=D[f(X)]+D[g(Y)],其中f(x),g(x)连续（针对连续型）\\
D(XY)=E[X^2Y^2]-E^2(XY)=E(X^2)E(Y^2)-(EX)^2(EY)^2=\cdots$$

## 协方差的定义与性质

$$如果DX,DY存在，且DX>0,DY>0,\\
则称E[(X-EX)(X-EY)]为协方差，记为\text{Cov}(X,Y)\\
\ \\
\text{Cov}(X,Y)=E[(X-EX)(Y-EY)]=E(XY)-EX\cdot EY$$
$$性质：\\
\text{Cov}(X,X)=DX,\quad \rho=1\\
\text{Cov}(X,c)=0（不符合协方差定义DX,DY>0，但方便计算）\\
\text{Cov}(X_1+X_2,Y)=\text{Cov}(X_1,Y)+\text{Cov}(X_2,Y)（组合拆分性）\\
\text{Cov}(aX+c,bY+d)=ab\ \text{Cov}(X,Y)=ab\ \rho\ \sqrt{DX}\cdot\sqrt{DY}$$

## 皮尔逊相关系数（线性相关性）

$$\rho=\frac{\text{Cov}(X,Y)}{\sqrt{DX}\sqrt{DY}}\qquad(DX>0,DY>0)$$
$$性质：
|\rho|\leqslant 1\\
\rho_{XY}=0\Leftrightarrow \text{Cov}(X,Y)=0\Leftrightarrow X,Y不相关\Leftrightarrow  \\{\color{blue}E(XY)=E(X)E(Y)}\Leftrightarrow D(X\pm Y)=DX+ DY\\
$$

## 相关系数的性质拓展

$$\left\{
\begin{array}{l}
X,Y满足线性关系(aX+bY=c)\Rightarrow \rho_{XY}=\pm1\\
\ \\
\rho_{XY}=1\Leftrightarrow X,Y正相关\Leftrightarrow P(Y=aX+b,a>0)=1,a=\sqrt{\frac{DY}{DX}}\\
\rho_{XY}=-1\Leftrightarrow X,Y负相关\Leftrightarrow P(Y=aX+b,a<0)=1,a=-\sqrt{\frac{DY}{DX}}\\
（有限点不满足此线性关系，但不影响总体）

\end{array}
\right.$$
$$标准化随机变量：
\text{Cov}(X^*,Y^*)=\rho_{XY},\quad X^*=\frac{X-EX}{\sqrt{DX}},Y^*=\frac{Y-EY}
{\sqrt{DY}}\qquad$$

## 随机变量标准化

$$X^*=\frac{X-EX}{\sqrt{DX}}，即随机变量函数的平移伸缩$$

## 变量独立与相关的关系

$$X与Y独立\ \substack{\Rightarrow \\ \not\Leftarrow}\ X,Y不相关\Leftrightarrow \rho_{XY}=\text{Cov}(X,Y)=0\\
X,Y相关\Rightarrow X,Y不独立
$$
$$注：独立、相关对事件与变量来说不一样\\
相关性只探讨变量的线性相关性，而非事件$$

## 求期望、方差、协方差方法

$$1.利用期望、方差、协方差的运算性质\\
E(aX+bY)=aE(X)+bE(Y)\\
D(aX+b)=a^2D(X)\\
\text{Cov}(aX,bY)=ab\ \text{Cov}(X,Y)=ab\ [E(XY)-EXEY]=ab\sqrt{DX}\sqrt{DY}\\
......\\
2.利用分布函数计算\\
f(x,y),Z=\sqrt{X^2+Y^2}\\
F_Z(z),f_Z(z)\\

$$
$$例：F(x)=0.3\Phi(x)+0.7\Phi(\frac{x-1}{2})\\
计算概率密度，定义法计算\int_{-\infty}^{+\infty}x[0.3\varphi(x)+0.7\times \frac{1}{2}\varphi(\frac{x-1}{2})]dx$$

## 离散型求期望

$$级数求和，灵活寻找与幂级数的关系，和函数计算$$

# 大数定律与中心极限定理

## 依概率收敛

$$\quad\ X_n\xrightarrow{P}X \\\Leftrightarrow\lim\limits_{n\to \infty}P\{|X_n-X|\geqslant\varepsilon\}=0或\lim\limits_{n\to \infty}P\{|X_n-X|\leqslant\varepsilon\}=1$$

## 切比雪夫不等式

$$设X的期望EX与方差DX均存在，则对任意给定的\varepsilon >0，有\\
P\{|X-EX|\geqslant \varepsilon\}\leqslant \frac{DX}{\varepsilon^2}\qquad
P\{|X-EX|<\varepsilon\}\geqslant 1-\frac{DX}{\varepsilon^2}$$
$$注：留意EX=0情形$$

## 大数定律

**互相独立是前提**
**切比雪夫大数定理:**
$$\{X_i\}相互独立（可放宽至两两不相关），DX_i存在且一致有上界(DX_i\leqslant C)，则\\
\frac{1}{n}\sum_{i=1}^n X_i \xrightarrow{P}\frac{1}{n}\sum_{i=1}^n EX_i\\
\ \\
注：高阶矩收敛，则低阶矩收敛；故DX存在，则EX存在（勿深究）$$
**伯努利大数定理:**
$$伯努利实验中B(n,P)，n_A为发生次数\\
\frac{n_A}{n}\xrightarrow{P}p$$
**辛钦大数定理:**
$$\{X_i\}独立同分布，且EX_i=\mu，则\\
\frac{1}{n}\sum_{i=1}^n X_i \xrightarrow{P}\mu$$

## 中心极限定理

**互相独立是前提**
**列维-林德伯格定理：**
$$\{X_n\}独立同分布，且EX_i=\mu,DX_i=\sigma^2，则\\
\lim\limits_{n\to \infty}P\left\{\frac{\sum_{i=1}^nX_i-n\mu}{\sqrt{n}\sigma}\leqslant x\right\}=\frac{1}{\sqrt{2\pi}}\int_{-\infty}^xe^{-\frac{1}{2}t^2}dt=\Phi(x)$$
**棣莫弗-拉普拉斯定理：**
$$Y_n\sim B(n,p)\\
\lim\limits_{n\to \infty}P\left\{\frac{Y_n-np}{\sqrt{np(1-p)}}\leqslant x\right\}=\frac{1}{\sqrt{2\pi}}\int_{-\infty}^xe^{-\frac{1}{2}t^2}dt=\Phi(x)$$
$$注：
n\gg1时，\overline{X}\sim N(EX,DX)（近似）$$

# 数理统计的基本概念

## 简单随机样本

$$独立、同分布$$

## 分位数

$$上\alpha分位数：P\{X>v_\alpha\}=\int_{v_\alpha}^{+\infty}f(x)dx=\alpha\\
\ \\
下\alpha分位数：P\{X<v_\alpha\}=\int_{-\infty}^{v_\alpha}f(x)dx=\alpha $$
$$分位数的伸缩：\\
t=\frac{X}{a}\sim N(0,1),\quad P\{X>v_{\alpha}\}=\int^{+\infty}_{v_{\alpha}} f(x)dx=\alpha\\
\Rightarrow t=\frac{X}{a}=v_{\alpha}，即X=av_{\alpha}$$
$$注：考研范围内，默认为上\alpha分位数\\

下\alpha分位数=上(1-\alpha)分位数\\
若概率密度关于y轴对称，则下\alpha分位数=-（上\alpha分位数）$$

## 常用统计量

**关键：不含总体未知参数的样本**
$$样本均值：\overline{X}=\frac{1}{n}\sum_{i=1}^{n}X_i\\
样本方差：S^2=\frac{1}{n-1}\sum_{i=1}^{n}(X_i-\overline{X})^2\quad（无偏估计）\\
k阶样本原点矩：A_k=\frac{1}{n}\sum_{i=1}^nX_i^k\\
k阶样本中心矩：B_k=\frac{1}{n}\sum_{i=1}^n(X_i-\overline{X})^k\\
B_2=\frac{1}{n}\sum_{i=1}^n(X_i-\overline{X})^2=\frac{n-1}{n}S^2$$
$$对于任意分布的统计量：\\
D(\overline{X})=\frac{1}{n}DX,\quad
E(S^2)=DX,
\quad
E(B_2)=\frac{n-1}{n}DX$$

## $\chi^2$分布

**标准正态总体下**
$$\chi^2分布：\\
\{X_n\}相互独立且服从标准正态，X=\sum_{i=1}^nX_i^2\sim \chi^2(n)\\
性质：\\
X_1\sim \chi^2(n_1),X_2\sim \chi^2(n_2),X_1与X_2相互独立，则X_1+X_2\sim \chi^2(n_1+n_2)\\

X\sim \chi^2(n)，则EX=n,DX=2n$$

## t分布

**标准正态总体下**
$$t分布：\\
X\sim N(0,1),Y\sim \chi^2(n),X与Y相互独立，则t=\frac{X}{\sqrt{\frac{Y}{n}}}\sim t(n)\\
性质：\\
概率密度图像关于y轴对称\\
n\gg1时，t\sim N(0,1)（近似）\\
t^2\sim F(1,n)\\
E(t)=0,D(t)=\frac{n}{n-2}(n>2)\\
\ \\
注：形为\frac{U}{\sqrt{V}}\quad \frac{U}{|V|}，考虑 t分布，整理为标准形式$$

## $F$分布

**标准正态总体下**
$$F分布：
\\
X\sim \chi^2(n_1),Y\sim \chi^2(n_2),X与Y相互独立，则F=\frac{\frac{X}{n_1}}{\frac{Y}{n_2}}\sim F(n_1,n_2)\\
性质：\\
F\sim F(n_1,n_2),则\frac{1}{F}=\frac{\frac{Y}{n_2}}{\frac{X}{n_1}}\sim F(n_2,n_1)\\
F_{1-\alpha}(n_1,n_2)=\frac{1}{F_{\alpha}(n_2,n_1)}\quad “记”$$

## 单个正态总体下的抽样分布及数字特征

$$抽样分布：\\
\overline{X}\sim N(\mu,\frac{\sigma^2}{n})，即\frac{\overline{X}-\mu}{\frac{\sigma}{\sqrt{n}}}\sim N(0,1)\\

\sum_{i=1}^n\left(\frac{X_i-\mu}{\sigma}\right)^2\sim \chi^2(n)\\

\frac{(n-1)S^2}{\sigma^2}={\color{blue}\sum_{i=1}^n\left(\frac{X_i-\overline{X}}{\sigma}\right)^2}\sim \chi^2(n-1)\quad（证明极其复杂）\\

\frac{(\overline{X}-\mu)}{\frac{S}{\sqrt{n}}}=\frac{\frac{(\overline{X}-\mu)}{\frac{\sigma}{\sqrt{n}}}}{\sqrt{\frac{S^2}{\sigma^2}}}\sim t(n-1);\quad\frac{(\overline{X}-\mu)^2}{\frac{S^2}{n}}=\frac{\frac{(\overline{X}-\mu)^2}{\frac{\sigma^2}{n}}}{\frac{S^2}{\sigma^2}}\sim F(1,n-1)\quad{\color{blue}（\overline{X}与S^2相互独立）}$$
$$数字特征：D(S^2)=\frac{\sigma^4}{(n-1)^2}D[\frac{(n-1)S^2}{\sigma^2}**=\frac{\sigma^4}{(n-1)^2}D[\chi^2(n-1)]=\frac{2\sigma^4}{n-1}$$

## 两个正态总体下的抽样分布
$$\{X_n\},\{Y_m\}相互独立$$

$$\overline{X}\pm\overline{Y}\sim N(\mu_1\pm\mu_2,\frac{\sigma_1^2}{n}+\frac{\sigma_2^2}{m})，即\frac{\overline{X}\pm\overline{Y}-(\mu_1\pm\mu_2)}{\sqrt{\frac{\sigma_1^2}{n}+\frac{\sigma_2^2}{m}}}\sim N(0,1)
$$
$$\sigma_1=\sigma_2=\sigma时，\\
\frac{\overline{X}\pm\overline{Y}-(\mu_1\pm\mu_2)}{\sqrt{\frac{\sigma^2}{n}+\frac{\sigma^2}{m}}}\left/\sqrt{\frac{\sum_{i=1}^{n}(X_i-\overline{X})^2+\sum_{i=1}^{m}(Y_i-\overline{Y})^2}{(n+m-2)\sigma^2}}\right.\sim t(n+m-2)$$
$$\frac{S_1^2/ \sigma_1^2}{S_2^2/\sigma_2^2}\sim F(n-1,m-1)$$

# 参数估计

## 考情分析

区间估计：仅考查单个、两个正态总体下的（两个正态总体几乎不考）

## 矩估计

$$总体k阶矩E(X^k)（含参）=样本原点矩A_k\\
\left.\begin{array}{l}连续：E(X^k)=\int_{-\infty}^{+\infty}x^kf(x;\theta)dx\\
离散：E(X^k)=\sum_{i=1}^n x_i^kf(x_i;\theta)
\end{array}\right\}=A_k(\frac{1}{n}\sum_{i=1}^n X_i^k )（样本必然是离散点）\\
反解得估计量\hat{\theta}(X_1,X_2,\cdots,X_n)\quad估计值\hat{\theta}(x_1,x_2,\cdots,x_n)\\
 \ \\
若涉及估计量的评判标准，A_k的样本值最后代入；否则直接代入，简化计算$$
$$典例：\\
1.若一阶矩不含\theta，利用二阶矩估计\theta（考研大纲仅要求到二阶矩）\\
2.若总体分布含有两个未知参数
\left\{\begin{array}{}f(x_i;\theta_1,\theta_2)\\
f(x_i;\theta_1,\theta_2)
\end{array}\right.则分别求出一阶矩、二阶矩，解方程
$$
$$注：f(x_i;\theta)表示x_i的函数，x_i为总体可能取值，\theta为参数$$

## 最大似然估计法

$$\left.\begin{array}{l}
离散：L(\theta)=\ln[\prod_{i=1}^{n}P(x_i;\theta)]\quad 离散只能确定估计值（直接代入；样本不同似然函数不同）\\
连续：L(\theta)=\ln[\prod_{i=1}^{n}f(x_i;\theta)]\quad 概率密度的累乘（样本不同不影响似然函数表达式）
\end{array}\right\}n为样本个数\\

令\frac{d[L(\theta)]}{d\theta}=0
，解得\hat{\theta}(x_1,x_2,\cdots,x_n) \\
估计值\hat{\theta}(x_1,x_2,\cdots,x_n)\quad 估计量\hat{\theta}(X_1,X_2,\cdots,X_n)\\
\ \\
若涉及估计量的标准，样本值x_i最后代入；否则直接代入，简化计算$$
$$典例：\\
1.若导数为0的点不存在
\left\{\begin{array}{ll}
超出取值范围\\
导数\neq0
\end{array}\right.，则取\theta（样本值相关）使L(\theta)最大\\
2.若总体分布含有两个未知参数L(\theta_1,\theta_2)，则令偏导为0
\left\{\begin{array}{ll}
\frac{\partial L(\theta_1,\theta_2)}{\partial \theta_1}=0\\
\ \\
\frac{\partial L(\theta_1,\theta_2)}{\partial \theta_2}=0
\end{array}\right.\\
解估计值
\left\{\begin{array}{ll}
\hat{\theta}_1(x_1,x_2,\cdots,x_n)\\
\hat{\theta}_2(x_1,x_2,\cdots,x_n)
\end{array}\right.，
估计量
\left\{\begin{array}{ll}
\hat{\theta}_1(X_1,X_2,\cdots,X_n)\\
\hat{\theta}_2(X_1,X_2,\cdots,X_n)
\end{array}\right.$$
$$注：f(x_i;\theta)表示x_i的函数，x_i为发生的样本值，\theta为参数$$

## 估计量的评判标准

$$无偏性：E\hat{\theta}=E\theta\\
$$
$$有效性：D\hat{\theta_1}<D\hat{\theta_2}$$
$$一致性（相合性）：\hat{\theta}\xrightarrow {P}\theta(n\to \infty)\\
注：一致性与无偏性无关
\left\{\begin{array}{l}
有偏估计量的一致性\\
无偏估计量的一致性
\end{array}\right.$$

## 一致性判别

思路一：[切比雪夫不等式](#切比雪夫不等式)
$$\forall \varepsilon>0，当n\to \infty时，有\\ P\{|\hat{\theta}_1-\theta|\geqslant \varepsilon\}\leqslant \frac{D(\hat{\theta}_1)}{\varepsilon^2}=\frac{\frac{\theta^2}{3n}}{\quad\varepsilon^2\quad}\to 0$$
思路二：[大数定律](#大数定律)
$$X_i独立同分布，E(X_i^2)=\theta，根据辛钦大数定律，有\\
\hat{\theta}_n=\frac{1}{n}\sum_{i=1}^{n}X_i^2依概率收敛于\theta，即\lim\limits_{n\to \infty}P\{|\hat{\theta}_n-\theta|\geqslant\varepsilon\}=0$$

## 单个正态总体期望的区间估计（双侧置信区间）

$$\sigma^2已知：
-u_{\frac{\alpha}{2}}<\frac{\overline{X}-\mu}{\frac{\sigma}{\sqrt{n}}}<u_{\frac{\alpha}{2}} \\

\mu的置信区间为：
\left(\overline{X}-u_{\frac{\alpha}{2}}\cdot\frac{\sigma}{\sqrt{n}},\quad \overline{X}+u_{\frac{\alpha}{2}}\cdot\frac{\sigma}{\sqrt{n}}\right)\\
 \ \\
\sigma^2未知：
-t_{\frac{\alpha}{2}}(n-1)<\frac{\overline{X}-\mu}{\frac{S}{\sqrt{n}}}<t_{\frac{\alpha}{2}}(n-1)\\

\mu的置信区间为：
\left(\overline{X}-t_{\frac{\alpha}{2}}(n-1)\frac{S}{\sqrt{n}},\quad \overline{X}+t_{\frac{\alpha}{2}}(n-1)\frac{S}{\sqrt{n}}\right)$$
$$推导原理：P\{\}=1-\alpha\qquad \{\}内不等式变形$$

## 单个正态总体方差的区间估计（双侧置信区间）

$$\mu已知：\chi^2_{1-\frac{\alpha}{2}}(n)<\sum_{i=1}^n\left(\frac{X_i-\mu}{\sigma}\right)^2<\chi^2_\frac{\alpha}{2}(n)\\
\sigma^2的置信区间
\left(\frac{\sum_{i=1}^n\left({X_i-\mu}\right)^2}{\chi^2_\frac{\alpha}{2}(n)},\quad \frac{\sum_{i=1}^n\left({X_i-\mu}\right)^2}{\chi^2_{1-\frac{\alpha}{2}}(n)}\right)\qquad \sigma的置信区间\left(\sqrt{\frac{\sum_{i=1}^n\left({X_i-\mu}\right)^2}{\chi^2_\frac{\alpha}{2}(n)}},\quad \sqrt{\frac{\sum_{i=1}^n\left({X_i-\mu}\right)^2}{\chi^2_{1-\frac{\alpha}{2}}(n)}}\right)$$
$$\mu未知：\chi^2_{1-\frac{\alpha}{2}}(n-1)<\sum_{i=1}^n\left(\frac{X_i-\overline{X}}{\sigma}\right)^2=\frac{(n-1)S^2}{\sigma^2}<\chi^2_\frac{\alpha}{2}(n-1)\\
\sigma^2的置信区间
\left(\frac{\sum_{i=1}^n\left({X_i-\overline{X}}\right)^2}{\chi^2_\frac{\alpha}{2}(n-1)},\quad \frac{\sum_{i=1}^n\left({X_i-\overline{X}}\right)^2}{\chi^2_{1-\frac{\alpha}{2}}(n-1)}\right)\qquad \sigma的置信区间\left({\frac{\sqrt{n-1}S}{\sqrt{\chi^2_\frac{\alpha}{2}(n-1)}}},\quad \frac{\sqrt{n-1}S}{\sqrt{\chi^2_{1-\frac{\alpha}{2}}(n-1)}}\right)$$
$$推导原理：P\{\}=1-\alpha\qquad \{\}内不等式变形\\
注：-u_{\frac{\alpha}{2}}<\frac{\overline{X}-\mu_0}{\frac{\sigma}{\sqrt{n}}}<u_{\frac{\alpha}{2}}
\qquad

\chi^2_{1-\frac{\alpha}{2}}(n)<\sum_{i=1}^n\left(\frac{X_i-\mu}{\sigma}\right)^2<\chi^2_\frac{\alpha}{2}(n)$$

# 假设检验

## 考情分析

参数假设检验：仅考查正态总体下的

## 假设检验

$$备择假设与原假设为对立的$$

## 正态总体下的期望检验域与拒绝域

**关键：统计量与拒绝域的关系判断是否拒绝假设**
$$H_0：\mu=\mu_0\\
\sigma^2已知：-u_{\frac{\alpha}{2}}<\frac{\overline{X}-\mu_0}{\frac{\sigma}{\sqrt{n}}}<u_{\frac{\alpha}{2}}\\
\mu的接受域（统计量\overline{X}）：
\left(\mu_0-u_{\frac{\alpha}{2}}\frac{\sigma}{\sqrt{n}},\quad \mu_0+u_{\frac{\alpha}{2}}\frac{\sigma}{\sqrt{n}}\right)\\
\sigma^2未知：-t_{\frac{\alpha}{2}}(n-1)<\frac{\overline{X}-\mu_0}{\frac{S}{\sqrt{n}}}<t_{\frac{\alpha}{2}}(n-1)\\
\mu的接受域（统计量\overline{X}）：
\left(\mu_0-t_{\frac{\alpha}{2}}(n-1)\frac{S}{\sqrt{n}},\quad \mu_0+t_{\frac{\alpha}{2}}(n-1)\frac{S}{\sqrt{n}}\right)$$
$$推导原理：P\{\}=1-\alpha\qquad \{\}内不等式变形$$
$$H_0：\mu\leqslant \mu_0,\quad \mu\geqslant \mu_0\\
统计量\overline{X}的接受域：
\left(-\infty,\quad \mu_0+u_{\frac{\alpha}{2}}\frac{\sigma}{\sqrt{n}}\right),\qquad
\left(\mu_0-u_{\frac{\alpha}{2}}\frac{\sigma}{\sqrt{n}},\quad +\infty\right)\\

\left(-\infty,\quad \mu_0+t_{\frac{\alpha}{2}}(n-1)\frac{S}{\sqrt{n}}\right),\qquad \left(\mu_0-t_{\frac{\alpha}{2}}(n-1)\frac{S}{\sqrt{n}},\quad +\infty\right)$$

## 正态总体下的方差检验域与拒绝域

$$H_0:\sigma=\sigma_0\\
\mu已知：\chi^2_{1-\frac{\alpha}{2}}(n)<\sum_{i=1}^n\left(\frac{X_i-\mu}{\sigma_0}\right)^2<\chi^2_\frac{\alpha}{2}(n)\\
\sigma的接受域（统计量\sum_{i=1}^n\left({X_i-\mu}\right)^2）：\left(\chi^2_{1-\frac{\alpha}{2}}(n)\cdot\sigma_0^2,\quad \chi^2_\frac{\alpha}{2}(n)\cdot\sigma_0^2\right)\\

\mu未知：\chi^2_{1-\frac{\alpha}{2}}(n-1)<\frac{(n-1)S^2}{\sigma_0^2}=\sum_{i=1}^n\left(\frac{X_i-\overline{X}}{\sigma_0}\right)^2<\chi^2_\frac{\alpha}{2}(n-1)\\
\sigma的接受域（统计量\sum_{i=1}^n\left({X_i-\overline{X}}\right)^2）：\left(\chi^2_{1-\frac{\alpha}{2}}(n-1)\cdot\sigma_0^2,\quad \chi^2_\frac{\alpha}{2}(n-1)\cdot\sigma_0^2\right)$$
$$推导原理：P\{\}=1-\alpha\qquad \{\}内不等式变形$$

## 两类错误

$$第一类错误（弃真）：\alpha=P\{拒绝H_0|H_0为真\}\\
第二类错误（取伪）：\beta=P\{接受H_0|H_0为假\}=P\{接受H_0|H_1为真\}\quad(\beta\neq1-\alpha)\\
\ \\
注：
\left\{\begin{array}{l}
H_0为假\Leftrightarrow H_1为真\\
接受H_0或拒绝H_0由具体事件确定（即给定接受域或拒绝域）
\end{array}\right.$$
$$典例：假设X是连续型随机变量，U是对X的一次观测值；其概率分布有以下假设：\\
H_0:f(x)=
\left\{\begin{array}{l}
\frac{1}{2},& 0\leqslant x\leqslant 2\\
\ \\
0,&其他
\end{array}\right.\quad

H_1:f(x)=
\left\{\begin{array}{l}
\frac{x}{2},& 0\leqslant x\leqslant 2\\
\ \\
0,&其他
\end{array}\right.\\

当V=\{U>\frac{3}{2}\}出现时，否定假设H_0，接受H_1.则\\
犯第一类错误的概率\alpha=P\{U>\frac{3}{2}\bigg|H_0\}=\int_\frac{3}{2}^2\frac{1}{2}dx=\frac{1}{4}\\
犯第二类错误的概率\beta=P\{U\leqslant\frac{3}{2}\bigg|H_1\}=\int_0^\frac{3}{2}\frac{x}{2}dx=\frac{9}{16}$$

# 熟记小结论

$$\sum_{i=0}^nC_n^i=(1+1)^n=2^n$$

## 泊松积分

$$I=\int_{-\infty}^{+\infty}e^{-x^2}dx=\sqrt{\pi}\\
I^2=\int_{-\infty}^{+\infty}e^{-x^2}dx\int_{-\infty}^{+\infty}e^{-y^2}dy=\iint\limits_{D}e^{-(x^2+y^2)}d\sigma$$

## $\int_0^{+\infty}e^{-ax}dx$

$$\int_0^{+\infty}e^{-ax}dx=\frac{1}{a}(a>0)$$

# 计算严谨性问题
