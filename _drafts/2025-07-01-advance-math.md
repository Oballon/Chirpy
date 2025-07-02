高数知识量很大，理解相较容易，但灵活性较高       总结必要的概念、结论、方法、经验、典例等，仅为知识体系，不覆盖做题分析能力（灵活使用，掌握足够的技巧方法，面对题目“非无之无”）考试面前，适当理解以对抗风险，但应用为先！

# 默认章节

## 考情分析

选择题：4道
填空题：4道
大题：4道

## 考查轻重点讨论

1. 数列极限证明题：中上上难度
2. 中值定理证明题：中上上难度
3. 微分方程：中等难度
4. 不定积分：中上难度
5. 数项级数：中上难度

## 重要技巧（解题技巧 > 计算方法）

1. 指数化与对数化（解函数，极限，求导）（应用空间不尽相同）

$$\Delta=e^{\ln\Delta}\quad （可能影响定义域）\\
\Delta=\ln e^\Delta$$
2. 特值法
选择题善用

# 重要概念补充

## 系数对应问题注意

$$\quad \ ax+by=x+y（即\forall x,y）\\
\Leftrightarrow a,b=1$$
$$\quad \ \xi a+\mu b=a+b（对特定的a,b,有特定的\xi,\mu）\\
\not\Leftrightarrow \xi,\mu=1$$

## 去绝对值问题

$$因变量去绝对值，要加“\pm”$$
$$自变量去绝对值，
应分类讨论$$

## 易失误问题

**约分问题：**
$$\Delta=\alpha\Delta（须分类讨论\Delta=0）\\
\Delta\neq0,则\alpha=1\\
\Delta=0,则\alpha未知$$

## 变量代换求函数问题

**注意代换回原变量**
$$f[\varphi(t)]\neq f(t)\\
f[\varphi(t)]\xlongequal{t=\varphi^{-1}(x)}f[\varphi(\varphi^{-1}(x))]=f(x)$$

# 预备知识

## 泰勒展开
$$e^x,a^x,\ln(1+x) \qquad

\frac{1}{1+x} ,\ \frac{1}{1-x}\qquad

\sin x,  \cos x,  \arctan x\qquad

(1+x)^\alpha\qquad

\tan x,  \arcsin x
$$

$$x_0=0,x\to0时$$
$$\mathrm{e}^x=1+x+\frac{x^2}{2!}+ \cdots+ \frac{x^n}{n !}+\circ(x^n)\\

\mathrm{a}^x=e^{x\ln a}=1+x\ln a+\frac{(x\ln a)^2}{2!}+ \cdots+ \frac{(x\ln a)^n}{n !}+\circ(x^n)\\

\ln (1+x)=x-\frac{x^2}{2}+\frac{x^3}{3}-\cdots+\frac{(-1)^{n-1} x^n}{n}+\circ(x^n) $$
$$\frac{1}{1+x}=1-x+x^2-\cdots+(-1)^n x^n+\circ(x^n)\\

\frac{1}{1-x}=1+x+x^2+\cdots+ x^n+\circ(x^n)$$
$$\sin x = x - \frac{x^3}{3!} + \frac{x^5}{5!} - \cdots +\frac{(-1)^n}{(2n+1)!} x^{2n+1} +\circ(x^{2n+1})\\

\cos x =1 - \frac{x^2}{2!} + \frac{x^4}{4!} - \cdots +  \frac{(-1)^n}{(2n)!} x^{2n}+\circ(x^{2n})\\

\arctan x =x-\frac{x^3}{3} + \frac{x^5}{5}-\cdots +\frac{(-1)^n}{2n+1} x^{2n+1}+\circ(x^{2n+1})
$$
$$(1+x)^\alpha=1+\alpha x+ \frac{\alpha(\alpha-1)}{2!}x^2+\cdots+\circ(x^{n})\quad {\color{blue}（\alpha为任意常数，此式可无限展开）}$$
**记前两项：**
$$
\tan x =x + \frac{x^3}{3} + \frac{2 x^5}{15} + \cdots  +\frac{B_{2n} (-4)^n \left(1-4^n\right)}{(2n)!} x^{2n-1} +\circ(x^{2n-1})\\

\arcsin x =x+\frac{x^3}{6}+\frac{3x^5}{40}+\cdots    \frac{(2n)!}{4^n (n!)^2 (2n+1)} x^{2n+1} +\circ(x^{2n+1})$$

## 数列重要公式
等差、等比求和
$$1^2+2^2+3^3+\cdots+n^2$$

$$S_n=\frac{n(a_1+a_n)}{2}$$
$$S_n=\frac{a_1(1-q^n)}{1-q}$$
$$1^2+2^2+3^3+\cdots+n^2=\frac{n(n+1)(2n+1)}{6}$$

## 三角函数常用公式
$$(\sin^2x,\cos^2x),(\tan^2x, \sec^2x), (\cot^2x, \csc^2x) $$
$$\sin2\alpha, \cos2\alpha$$
$$\sin(\alpha\pm \beta), \cos(\alpha\pm \beta), \tan(\alpha\pm \beta)$$

$$\begin{array}{lll}
\sin^2x+\cos^2x=1 & 1+\tan^2x=\sec^2x & 1+\cot^2x=\csc^2x \\
\\
\sin2\alpha=2\sin\alpha \cos\alpha
&\cos2\alpha=\cos^2\alpha-\sin^2\alpha=2\cos^2\alpha-1=1-2\sin^2\alpha \\
\\
\sin(\alpha\pm \beta)=\sin\alpha \cos\beta\pm \cos\alpha \sin\beta &
\cos(\alpha\pm \beta)=\cos\alpha  \cos\beta \mp \sin\alpha \sin\beta & \tan(\alpha\pm \beta)=\frac{\tan\alpha\pm \tan\beta}{1\mp \tan\alpha \tan\beta}
\end{array}$$

## 积化和差、和差化积
$$\sin\alpha \cos\beta,\cos\alpha \sin\beta,\cos\alpha\cos\beta,\sin\alpha \sin\beta$$
$$\sin\theta+\sin\gamma,\sin\theta-\sin\gamma,\cos\theta+\cos\gamma,\cos\theta-\cos\gamma$$

**积化和差：**
$$\begin{array}{l}
\sin\alpha \cos\beta=\frac{1}{2}[\sin(\alpha+\beta)+\sin(\alpha-\beta)]\\
\\
\cos\ \alpha \sin\beta=\frac{1}{2}[\sin(\alpha+\beta)-\sin(\alpha-\beta)]\\
\\
\cos\ \alpha \cos\beta=\frac{1}{2}[\cos(\alpha+\beta)+\cos(\alpha-\beta)]\\
\\
\sin\ \alpha \sin\beta=\frac{1}{2}[\cos(\alpha-\beta)-\cos(\alpha+\beta)]
\end{array}$$
**和差化积（由积化和差公式反得）：**
$$\theta=(\alpha+\beta),\gamma=(\alpha-\beta)\\
\left\{\begin{array}{l}
\textcircled{1}拆项整理\\
\textcircled{2}反解变量
\left\{\begin{array}{l}
\alpha=\frac{\theta+\gamma}{2}\\
\ \\
\beta=\frac{\theta-\gamma}{2}
\end{array}\right.
\end{array}\right.
$$

## 因式分解公式

$$a^3-b^3, a^3+b^3$$

$$a^3-b^3=(a-b)(a^2+ab+b^2)$$
$$a^3+b^3=(a+b)(a^2-ab+b^2)$$

## 常用不等式（等号成立条件）

$$(|a\pm b|, |a|+|b|, ||a|-|b||)$$
$$(\frac{2}{\frac{1}{a}+\frac{1}{b}},\sqrt{\frac{a^2+b^2}{2}},\sqrt{ab}, \frac{a+b}{2}) $$
$$(\sin x, x, \tan x)
(\arctan x, x, \arcsin x,)
(e^x-1,x, \ln(x+1))$$
$$\left(\frac{1}{1+x}, \ln(1+\frac{1}{x}), \frac{1}{x}\ \ (x>0)\right)\left(\frac{x}{1+x},\ln(1+x),x\ (x>0)\right)$$

**不等式灵活使用，形式多样本质不变，勿固化**
$$||a|-|b|| \leqslant |a\pm b| \leqslant |a|+|b|  $$
$$\frac{2}{\frac{1}{a}+\frac{1}{b}}\leqslant\sqrt{ab}\leqslant \frac{a+b}{2}\leqslant \sqrt{\frac{a^2+b^2}{2}} {(a,b>0,a=b时等号成立;\quad 高维同样成立)}\\
{\color{blue}注：灵活取平方}$$
$$\begin{array}{l}
\sin x \leqslant x \leqslant \tan x \\
\arctan x \leqslant x \leqslant \arcsin x \\
\ln(x+1) \leqslant x \leqslant e^x-1
\end{array}$$
$$\frac{1}{1+x}<\ln(1+\frac{1}{x})< \frac{1}{x}   \ \ (x>0)\qquad\frac{x}{1+x}<\ln(1+x)<x\ \ (x>0)\\
{\color{blue}注：\Delta>0前提下，灵活替换x}$$

## 双阶乘
$$(2n)!!\ \ \ \ \  (2n-1)!!$$

$$(2n)!!=2\cdot 4 \cdot 6\cdots=2^n\cdot n!$$
$$(2n-1)!!=1\cdot 3\cdot 5\cdots$$

## 函数图像1
$$x^u(u=-1,\frac{1}{2},\frac{1}{3},1,2,3)\\
a^x(a>0且a\neq1),e^x \\
 \log_ax(a>0 且a\neq 1) ,\ln x\\
\sin x,\cos x\\
$$

![](pic-advance-math\Markji_1751353264015.png)
![](pic-advance-math\Markji_1751353816728.png)
![](pic-advance-math\Markji_1751353825922.png)
![](pic-advance-math\Markji_1751353833996.png)

## 函数图像2

$$\tan x,\cot x\\
\sec x,\csc x \\
\arcsin x,\arccos x\\
\arctan x,arccot x$$

![](pic-advance-math\Markji_1751353948396.png)
![](pic-advance-math\Markji_1751353963485.png)
![](pic-advance-math\Markji_1751353980035.png)
![](pic-advance-math\Markji_1751353993815.png)

## 取整函数

$$x-1<[x] ≤x$$
![](pic-advance-math\Markji_1751354029715.png)

## 摆线

$$\left\{
\begin{array}{l}
x=2(t-\sin t)\\

y=2(1-\cos t)
\end{array}
\right.\qquad a=2时$$
![](pic-advance-math\Markji_1751354091294.png)
$$a代表半径，t代表旋转角度，
几何意义\left\{
\begin{array}{l}
x=2t-2\sin t\\

y=2-2\cos t
\end{array}\right.$$

## 星形线

$$\left\{
\begin{array}{l}
x=a\cos^3 t\\

y=a\sin^3 t
\end{array}
\right.\quad 顶点距离原点为a$$
<img src="pic-advance-math\Markji_1751354129262.png" width="30%">

## 双纽线

$$直角坐标：(x^2+y^2)^2=2a^2(x^2-y^2)\\
极坐标：r^2=2a^2\cos2\theta$$
![](pic-advance-math\Markji_1751354158851.png)

## 常见几何计算公式

$$V_{球}=\frac{4}{3}\pi r^3\quad S_{球}=4\pi r^2$$
$$V_{圆锥}=\frac{1}{3}\pi r^2h\quad S_{圆锥侧}=\pi r l \quad
{\color{blue}V_{锥体}=\frac{1}{3}Sh（一般圆锥，棱锥）}$$
$$V_{椭球}=\frac{4}{3}\pi abc\quad S_{椭圆}=\pi ab$$
$$S_{扇}=\frac{1}{2}\rho^2\theta$$

## 过曲线外一点做切线，求切线

$$曲线y=\ln x，设切点为(x,\ln x)\\
Y-\ln x=\frac{1}{x}(X-x)，代入点(x_0,y_0)，解x即可$$

# 函数

## 反函数存在条件

函数自变量 x 与因变量 y 一 一对应（函数单调，等等）

## 如何理解反三角函数

反三角函数是三角函数在特定区间的反函数
$$y=\arcsin x, \ \ x\in[-1,1],y\in[-\frac{\pi}{2},\frac{\pi}{2}]$$
$$\arcsin(\sin x)\neq x （未限制x定义域，左x不一定等于右x）$$
$$\sin(\arcsin x)=x$$

## 隐函数与方程的关系

隐函数也是函数，满足函数的定义，一个方程可确定多个隐函数

## 函数的x、y对应及函数的决定要素

x->y: 一对一，多对一（唯一的x对应y）
定义域、对应关系（与变量符号无关）

## 函数奇偶性定义

$$函数f(x)的定义域D关于原点对称，\\
如果\forall x\in D，\left\{
\begin{array}{ll}
f(x)=f(-x)，则称f(x)为偶函数\\
f(x)=-f(-x)，则称f(x)为奇函数
\end{array}\right.$$
$$注：定义域D不一定连续，但考研几乎不考察不连续情形$$

## 函数单调性定义

$$函数f(x)的定义域为D，\forall x_1,x_2\in D，\\
当x_1<x_2时，恒有
\left\{\begin{array}{l}
f(x_1)<f(x_2)，则称f(x)单调递增\\
f(x_1)>f(x_2)，则称f(x)单调递减
\end{array}\right.$$
$$注：定义域D不一定连续，但考研几乎不考察不连续情形$$

## 函数周期性定义

$$函数f(x)的定义域为D，如果存在一个正数l，\\
使得\forall x\in D，有(x\pm l)\in D且f(x\pm l)=f(x)\\
则称f(x)为周期函数$$
$$注：定义域D不一定连续，但考研几乎不考察不连续情形
$$

## 函数对称性

关于x=a，(a,0)对称

$$ 关于x=a：\\
以x=a为参照：f(x+a)=f(a-x)\\
以x=0,2a为参照：f(x)=f(2a-x) \\
(且f(x+a)与f(a-x)关于x是偶函数)$$
$$关于(a,0)对称：\\
以x=a为参照：f(x+a)=-f(a-x)\\
以x=0,2a为参照：f(x)=-f(2a-x) \\
(且f(x+a)与f(a-x)关于x是奇函数)$$

## 函数拆奇偶

$$任意f(x)\Rightarrow
\left\{\begin{array}{l}
f(x)+f(-x)为偶函数\\
f(x)-f(-x)为奇函数

\end{array}\right.$$
$$f(x)可拆解为：
\left\{\begin{array}{}
\frac{1}{2}[f(x)+f(-x)] \quad偶函数\\
\ \\
\frac{1}{2}[f(x)-f(-x)]\quad奇函数
\end{array}\right.$$

## 判断函数奇偶性的方法
定义法，复合函数，乘法

1. 定义法
$f(x), f(-x)$
2. 复合函数：内偶则偶，内奇同外
3. 乘法：奇×奇=偶，偶×偶=偶，奇×偶=奇

## 判断函数有界的三条结论

$$f(x)在[a,b]上连续或单调\Rightarrow f(x)在[a,b]上有界$$
$$f(x)在(a,b)，(-\infty,+\infty)内连续或单调,且\lim\limits_{x\to a+,-\infty}f(x)\ \exist, \lim\limits_{x\to b^-,+\infty}f(x)\ \exist\Rightarrow f(x)在(a,b)内有界$$
$$f'(x)在有限区间(a,b)内有界([a,b]上判断(a,b)即可，端点另行判断)\Rightarrow f(x)在(a,b)内有界$$

## 函数的平移放缩

$$标准形式：y=f(ax+b)\quad先位移，后放缩\\
位移：左加右减\\
放缩：\frac{1}{a}\quad （a<0直接翻转）$$

## 函数放缩变换后的最小正周期 T

$$y^*=f(ax+b),\ T^*=\frac{T}{|a|}$$
$$注：常函数为周期函数，但无最小正周期 T$$

## 复合函数问题重要思路

**整体代换**
$$1.\ f[\varphi(x)]=e^{\varphi^2(x)}=1-x$$
$$2.\ f[f(x)]=
\left\{
\begin{array}{}
\ln\sqrt{f(x)}, f(x)\geqslant1\\
\\
2f(x)-1,f(x)<1
\end{array}
\right.
$$

## 非定义区间求反三角函数问题

$$y=\sin x \quad x\in(\frac{\pi}{2},\frac{3\pi}{2})\\
令t=x-\pi,即x=t+\pi\\
y=\sin(t+\pi)\quad t\in(-\frac{\pi}{2},\frac{\pi}{2})\\
y=-\sin t\quad\quad\ \  y\in(-1,1)\\
t=\arcsin(-y)=-\arcsin y\\
即x-\pi=-\arcsin y\\
\quad x=\pi-\arcsin y\\
故y^{-1}=\pi-\arcsin x,\quad x\in(-1,1)$$

## 特殊求解反函数题型
$$y=\ln(x+\sqrt{1+x^2})$$

$$\left\{
\begin{array}{}
\sqrt{1+x^2}+x=e^y\\
\sqrt{1+x^2}-x=e^{-y}\\
\end{array}
\right.联立求解$$

## 特殊求解f(x)表达式题型
$$af(x)+bf(\frac{1}{x})=\frac{c}{x}$$

$$\left\{
\begin{array}{}
af(x)+bf(\frac{1}{x})=\frac{c}{x}\\
af(\frac{1}{x})+bf(x)=cx
\end{array}
\right.联立求解$$

# 极限

## $\circ(\Delta)$理解关键

$$凡出现\circ(\Delta),即默认\Delta\to 0,强调动态性$$

## 无界与无穷大，发散与无界的关系

无界包含：无穷大，无界振荡，无界分段函数等等

发散包含：无界，有界振荡，有界分段函数等等

（收敛是很狭隘的）

## 无穷小与无穷大的关系

$$\lim\limits_{x\to a}f(x)=\infty \ \Rightarrow \ \lim\limits_{x\to a}\frac{1}{f(x)}=0$$
$$\lim\limits_{x\to a}f(x)=0 \ 且 \ f(x)\neq 0 \ \Rightarrow \ \lim\limits_{x\to a}\frac{1}{f(x)}=\infty$$

## 极限的三条性质

**以极限的“趋向特质”把握**
$$唯一性\\
\left\{
\begin{array}{}
有界性\\
保号性
\end{array}
\right.
$$

## 极限关键理解

$$\lim\limits_{x\to a}f(x)=A $$
$$\Leftrightarrow x\to a时，f(x)\to A$$
$$\not\Leftrightarrow x\to a时，f(x)=A$$

## 极限四则运算前提及用法

$$前提：极限均存在时，才可拆分运算$$
$$\lim\limits_{x\to \infty}f(x)与\lim\limits_{x\to \infty}g(x)（x\to \infty的方式不同）\\
存在+存在=存在\\
存在+不存在=不存在\\
不存在+不存在=不确定（正负相消）\\
（若同号，则极限不存在）$$
$$因子极限存在（不定式视作整式因子）\\
实际应用中，一直后验使用（不一定所有因子均可判断极限存在）\\
例：非零因子常数化

$$

## 函数极限定义注意

$$1. x\to x_0 \Leftrightarrow
\left\{
\begin{array}{}
x\to x_0^+ \\
x\to x_0^- \\
x \neq x_0
\end{array}
\right.$$
$$2. x\to \infty \Leftrightarrow
\left\{
\begin{array}{}
x\to -\infty \\
x\to +\infty
\end{array}
\right.$$
$$3. \lim\limits_{x\to a}f(x)=A \Leftrightarrow
\lim\limits_{x\to a^+}f(x)=\lim\limits_{x\to a^-}f(x)=A
$$

## 常用的等价无穷小量

$$\sin x,\tan x,\arcsin x,\arctan x,\ln(1+x),e^x-1,\ln(x+\sqrt{x^2+1}) \\
(1+x)^\alpha-1(\alpha\neq0),a^x-1(a>0且 a\neq1),\log_a(1+x) \\
1-\cos x\\
x-\sin x,x-\tan x,x-\ln(1+x),x-\arcsin x,x-\arctan x$$

$$（x替换为\Delta均成立）$$
$$\sin x\sim \tan x\sim \arcsin x \sim \arctan x \sim \ln(1+x) \sim e^x-1 \sim \ln(x+\sqrt{x^2+1})$$
$$(1+x)^\alpha-1\sim \alpha x, a^x-1 \sim x\ln a, \log_a(1+x)\sim\frac{x}{\ln a}$$
$$1-\cos x \sim \frac{1}{2}x^2 $$
$$x-\sin x \sim \frac{1}{6}x^3, x-\tan x \sim -\frac{1}{3}x^3, x-\ln(1+x)\sim\frac{1}{2}x^2,x-\arcsin x \sim -\frac{1}{6}x^3,x-\arctan x \sim \frac{1}{3}x^3$$

## 特殊等价无穷小

$$(1+\Delta)^\Box-1\sim\Delta\cdot\Box\\
前提\left\{\begin{array}{l}(1+\Delta)^\Box\rightarrow 1\\ \Delta\to 0\ \end{array} \right.\\
\lim\limits_{x\to0}\frac{e^{\Box\ln(1+\Delta)}-1}{x^b}=\lim\limits_{x\to0}\frac{\Box\ln(1+\Delta)}{x^b}=\lim\limits_{x\to0}\frac{\Box\cdot\Delta}{x^b}$$

## 等价无穷小可作加减运算

$$\quad f(x)-x^a\sim x^b\\
=f(x)\sim x^b+x^a$$

## 倒代换

$$令t=\frac{1}{x}，便于分析，部分情形不一定$$

## 极限指数化与对数化

$$e^\Delta-\Box=e^\Delta-e^{\ln\Box}=e^{\ln\Box}(e^{(\Delta-\ln\Box)}-1)$$
$$\ln\Delta-\Box=\ln\Delta-\ln e^\Box=\ln\frac{\Delta}{e^\Box}$$

## 乘除“试凑”，加减“试凑”

$$\lim\limits_{\Delta\to0}\frac{\sin\Delta}{\Delta}=1$$
$$\lim\limits_{\Delta\to0}(1+\Delta)^\frac{1}{\Delta}=e  \  或  \ \lim\limits_{\Delta\to\infty}(1+\frac{1}{\Delta})^\Delta=e$$
**加减试凑：**
$$\lim\limits\frac{\ln(\Delta-1+1)}{\Box}=\lim\frac{\Delta-1}{\Box}$$
$$\lim\limits_{x\to 0}\frac{\alpha-\beta}{\alpha}=1-\lim\limits_{x\to 0}\frac{\beta}{\alpha}$$
$$\lim\limits_{x\to0}\frac{\beta}{\alpha}=\lim\limits_{x\to0}\frac{\beta-\alpha+\alpha}{\alpha}=1+\lim\limits_{x\to 0}\frac{\beta-\alpha}{\alpha}$$

## 无穷小比阶
高阶，低阶，同阶，等价，k阶

$$注意比阶的定义方式\\
等价：\lim\frac{\alpha(x)}{\beta(x)}=1(\neq -1){\color{blue}（等价替换本质在于此）}\\
（其他不要求正负）$$

## 抓大放小

$$1.\ x\to \infty,\ \log_ax (a>1)\ll x^a(a>0) \ll a^x(a>1)\\
 2. 幂函数阶次\\
 3. 复杂极限分子、分母内部比阶\\
\ \\
规范步骤：分子分母同除“大项”，构造无穷小项

$$
$$显式：
\left\{\begin{array}{l}
\lim\limits_{x\to -\infty}[\sqrt{x^2-x+1}-(ax+b)]\Rightarrow a=-1\\
\lim\limits_{x\to 0}(\frac{\sqrt{4x^2+x}}{x^a})=b(b\neq0), 则a=\frac{1}{2}\\
\end{array}\right.\\
隐式：
\lim\limits_{x\to0}\frac{(3+2\tan x)^x-3^x}{3\sin^2x+x^3\cos\frac{1}{x}}, 分母\lim\limits_{x\to0}\frac{x^3\cos\frac{1}{x}}{3\sin^2x}=0$$

## 非零因子常数化
（加减乘除，变上限积分）

**关键在于不定式**
加减慎用；若无加减，乘除直接用

**所给函数均连续**
$$非零因子常数化：\\
\lim\limits_{x\to 0}f(x)=A\neq 0,\lim\limits_{x\to 0}h(x)=0,且x\to 0时，h(x)\neq0,则x\to 0时,
\int_0^{h(x)}f(t)dt\sim Ah(x)$$

## 等价无穷小替换
（加减乘除，复合函数，变上限积分）

**关键在于不定式**
加减慎用；若无加减，乘除直接用、复合函数（复合函数各层均无穷小的前提下，由外向内替换）

**所给函数均连续**
$$等价无穷小替换：\\

x\to0 时，f(x)\sim ax^m, a\neq 0,m\in Z^+, 则\int_0^xf(t)dt\sim \int_0^x at^m dt=\frac{a}{m+1}x^{m+1}\\
x\to0 时，f(x)\sim ax^m, g(x)\sim bx^n, ab\neq 0,m,n\in Z^+, 则\int_0^{g(x)}f(t)dt\sim \int_0^{bx^n} at^m dt=\frac{a}{m+1}(bx^n)^{m+1}$$
$$注：\\
\lim\limits_{x\to0}\frac{\int_0^x f(t)dt}{\int_0^x ax^mdt}\xRightarrow{洛必达}\lim\limits_{x\to 0}\frac{f(x)}{ax^m}=1\\
f(x)须等价于m阶无穷小，即\lim\limits_{x\to 0}\frac{f(x)}{ax^m}=1（ x^k\sin\frac{1}{x}在x=0处无等价无穷小）$$

## 不定式极限计算
$$\frac{0}{0},\frac{\infty}{\infty},\infty-\infty,0\cdot\infty, 0^0,\infty^0,1^\infty$$

**都向分式化归**
$$少数情况是被动的：\\\lim\limits_{x\to \infty}x^2(\arctan\frac{1}{x}-\arctan\frac{1}{1+x})$$
$$仅少数须拆分（泰勒首阶次无相消）：\\
\lim\limits_{x\to0}\frac{\sqrt{\cos x}-\sqrt[3]{1+\sin^2x}}{(\arcsin x)^2}=\lim\limits_{x\to0}\frac{\sqrt{\cos x}-1-(\sqrt[3]{1+\sin^2x}-1)}{x^2}$$
$$1^\infty: \lim u^v=e^{\lim(u-1)v}；
{\color{blue}对复合函数使用了非零因子常数化,整式可如此处理，分式谨慎}\\
\lim\limits_{x\to +\infty}\frac{(1+\frac{1}{x})^{x^2}}{e^x}=e^{-\frac{1}{2}},\quad \lim\limits_{x\to +\infty}\frac{(1+\frac{1}{x})^{x^2}}{(1+\frac{1}{2x})^{2x^2}}=e^{-\frac{3}{8}} \quad （指数化）$$
[Card#ID/1XS81#极限指数化与对数化]

## 泰勒展开原则及注意
$$A-B型，\frac{A}{B}型$$

**几为通法：遇加减，难处理，泰勒展开**
$$\frac{A}{B}型：“上下同阶”原则$$
$$A-B型：“幂次最低”原则$$
$$ \lim\limits_{x\to 0}\frac{2\arctan x-\ln\frac{1+x}{1-x}}{x^p}=c\rightarrow
\lim\limits_{x\to 0}\frac{2\arctan x-\ln(1+x)+\ln(1-x)}{x^p}=c （泰勒展开）$$
$$注：
泰勒展开不便处理所有极限（复合函数不宜展开，洛必达处理）$$

## 洛必达法则三项使用条件

**严格遵循使用条件**
$$三项使用条件：\\
1. \ x\to a,\infty时，f(x),g(x)\to 0,\infty\\
\ \\
2. \  f(x),F(x)在x\in \mathring{U}(a,\delta)内，x\to \infty时可导\\
\ \\
3. \lim\limits_{x\to a,\infty}\frac{f'(x)}{F'(x)}=A,\infty$$

## 洛必达法则易错用法

**易错用法：**
$$\lim\frac{f(x)}{g(x)}=A,\infty\not\Rightarrow \lim\frac{f'(x)}{g'(x)}=A,\infty$$
$$例：
\lim\limits_{x\to 0}\frac{x^2\cdot \sin\frac{1}{x}}{x}=0\not\Rightarrow \lim\limits_{x\to 0}\frac{(x^2\cdot \sin\frac{1}{x})'}{x'}=0$$

**但洛必达反求参数可用：**
$$\lim\limits_{x\to (\frac{1}{2})^+}\frac{\pi-4\arccos\sqrt{2}x}{a(x-\frac{1}{2})^b}=1
\Longleftarrow
\lim\limits_{x\to (\frac{1}{2})^+}\frac{\frac{4\sqrt{2}}{\sqrt{1-2x^2}}}{ab(x-\frac{1}{2})^{b-1}}=1$$

## 中值定理计算极限
拉格朗日中值、柯西中值定理、积分中值定理

**中值定理求极限方法可能出现无法无法判断情形**
$$（\xi与x关系未知）$$
$$拉格朗日中值：\\
\lim\limits_{x\to 0}\frac{e^{\tan x}-e^{\sin x}}{x^3}\ \ \ \ f=e^t \\
\lim\limits_{x\to 0}\frac{\sqrt{\tan x}-\sqrt{\sin x}}{x^2}=\lim\limits_{x\to 0}\frac{\frac{1}{2\sqrt{\xi}}\cdot\frac{x^3}{6}}{x^2}（无法判断）$$
$$柯西中值：\\

\lim\limits_{x\to 0}\frac{\ln(1+\tan x)-\ln(1+\sin x)}{\sqrt{1+\tan x}-\sqrt{1+\sin x}}

\left\{
\begin{array}{}
f=\ln(1+t) \\
\\
g=\sqrt{1+t}
\end{array}

\right.$$
$$积分中值定理：\\

\lim\limits_{x\to 0}\frac{\int_x^{\sin x}e^xdx}{x^3}=\lim\limits_{x\to 0}\frac{e^\xi(\sin x-x)}{x^3}$$
$$注：a^x-b^x\xrightarrow{同型化} e^{x\ln a}-e^{x\ln b}$$

## 等式脱帽法

$$\lim\limits_{x\to \cdot} \frac{f(x)}{x^k}=A,f(x)=Ax^k+\alpha x^k\ (\lim\limits_{x\to \cdot}\alpha=0)\\
(或f(x)=Ax^k+\circ(x^k))\qquad
 （可利用此变换f(x)）$$
[Card#ID/1VS7M#][Card#ID/1Xwj8#无穷小求导函数]

## 极限定义函数

$$f(x)=\lim\limits_{n\to \infty}\frac{x^{n+2}-x^{-n}}{x^n+x^{-n}}（注意无定义点）\\
\ \\f(x)=\lim\limits_{t\to x}\left(\frac{\sin t}{\sin x}\right)^{\frac{x}{\sin t-\sin x}}$$
$$注：t,n 取极限x看作常量$$

## 常用极限分左右

$$\frac{1}{\infty},e^\infty, a^\infty, \arctan\infty, \mathrm{arccot}\infty, 分段点，\cdots$$

## 极限计算重要经验

1. 灵活是关键，勿固化
2. 预处理：等价替换，根式有理化
3. 泰勒展开不通用
4. 巧用洛必达（直接不好用）：无法处理时，用洛必达转换形式......
$$适用具体型极限\\
\lim\limits_{x\to a}f(x)(a\neq0,\infty)时，推荐$$
5. 中值定理计算极限有其不可替代性
6. 少数情形考虑两个重要准则：夹逼准则、单调有界准则

## 变限积分计算极限

**首先考虑洛必达**
$$\begin{array}{rl}\quad\ &\lim\limits_{t\to 0^+}\frac{\int_0^t dx\int_t^x e^{-(x-y)^2}dy}{1-e^{-t^2}}（二重积分被积函数含积分限变量，交换积分次序）\\
=&\lim\limits_{t\to 0^+}\frac{\int_0^t dy\int_0^y e^{-(x-y)^2}dx}{-t^2}\\
\xrightarrow{洛}&\lim\limits_{t\to 0^+}\frac{\int_0^t e^{-(x-t)^2}dx}{-2t}（一元积分被积函数含积分限变量，变量代换）
\end{array}$$

## 微分方程求等价无穷小
$$y''+2y'+y=e^{3x},y(0)=y'(0)=0，y(x)一阶连续可导\\求x\to0时,y(x)的等价无穷小$$

$$不建议解微分方程，分析法，洛必达讨论\\
y''(0)=1\qquad\lim\limits_{x\to 0}\frac{y(x)}{x^b}\xrightarrow{洛}\lim\limits_{x\to 0}\frac{y'(x)}{bx^{b-1}}\xrightarrow{洛}\lim\limits_{x\to 0}\frac{y''(x)}{b(b-1)x^{b-2}}
=1$$
$$注：微分方程形式低阶连续可导的高阶传递性$$

# """数列极限"""

## 考情分析

难点：“数列递推关系”题型、“方程的根”题型
关键：单调有界准则、夹逼定理

## 海涅定理（归结原则）

**计算时正向使用，反向难以操作**
**具体数列“n”直接当"x"使用（抓大放小、等价无穷小、泰勒展开等等均可用）**
$$f(x)在\mathring{U}(x_0)内有定义\\
\lim\limits_{x\to x_0}f(x)=A\Leftrightarrow对任意以x_0为极限的数列\{x_n\}（x_n\neq x_0）,都有\lim\limits_{n\to \infty}f(x_n)=A\\
f(x)在\ \infty\ 处有定义\\
\lim\limits_{x\to +\infty}f(x)=A,\infty\Leftrightarrow对任意趋于\infty的数列\{x_n\}（x_n\neq x_0）,都有\lim\limits_{n\to \infty}f(x_n)=A,\infty$$
$$\lim\limits_{x\to +\infty}f(x)=A \Rightarrow \lim\limits_{n\to \infty}f(n)=A $$
$$\lim\limits_{x\to +\infty}f(x)=A \nLeftarrow \lim\limits_{n\to \infty}f(n)=A $$

## 无穷大的比较

$$n\to \infty时\\
\ln\ n \ll n^\alpha(\alpha>0) \ll a^n(a>1)\ll n!\ll n^n$$
$$注：\lim\limits_{n\to \infty}\frac{2^n\cdot n!}{n^n}=0;\quad

\lim\limits_{n\to \infty}\frac{2^n\cdot n!\cdot n^9}{n^n}=0;\quad

\lim\limits_{n\to \infty}\frac{3^n\cdot n!}{n^n}=\infty$$

## 数列极限定义注意

1. 数列极限的间断性
$$\ \ \ \ (n\in Z^+)$$
2. 数列极限的单边性
$$\ \ \ \ (n\in Z^+)$$

## 单调有界准则“两条件”判断顺序

$$先判上下界，再判单调性（单调性判断多数情况依赖上下界，上下界依赖单调性较少）$$

## 数列递推关系处理（不等式）
上下界、单调性

**上下界：**
$$x_{n+1}=\sqrt{x_n(4-x_n)}\Rightarrow \\x_{n+1}=\sqrt{x_n(4-x_n)}\leqslant\frac{x_n+4-x_n}{2}=2$$
**单调性：**
$$(1-x_n)\cdot x_{n+1}>\frac{1}{4}\Rightarrow \\
{\color{blue}构造}\ \frac{x_n\cdot (1-x_n)\cdot x_{n+1}}{x_n}>\frac{1}{4}\Rightarrow \frac{x_{n+1}}{x_n}>\frac{1}{4x_n\cdot (1-x_n)}\geqslant \frac{1}{4(\frac{x_n+ (1-x_n)}{2})^2}=1$$
$$x_{n+1}+\frac{1}{x_n}<2\Rightarrow \\\sqrt{\frac{x_{n+1}}{x_n} }\leqslant \frac{x_{n+1}+\frac{1}{x_n}}{2}<1$$
$$x_{n+1}=\sin x_n\Rightarrow \frac{x_{n+1}}{x_n}<1,|x_n|\leqslant 1$$
$$\left\{
\begin{array}{l}
\cos\ x_{n+1}-x_{n+1}=\cos\ x_n(0<x_n<\frac{\pi}{2})\Rightarrow \\
\cos\ x_{n+1}-\cos\ x_n=x_{n+1}\Rightarrow
......\\
\\
e^{x_n}-x_n=e^{x_{n+1}}(x_n>0)\Rightarrow\\
e^{x_n}-e^{x_{n+1}}=x_n\Rightarrow......
\\
\\
\cos\ a_n-a_n=\cos\ b_n,\lim\limits_{n\to \infty}b_n=0(0<a_n,b_n<\frac{\pi}{2})\Rightarrow\\
\cos\ a_n-\cos\ b_n=a_n\Rightarrow0<a_n<b_n\Rightarrow......
\end{array}
\right.$$
$$拉格朗日中值定理：\\
x_{n+1}=\ln(\frac{e^{x_n}-1}{x_n})\Rightarrow \\e^{x_{n+1}}=\frac{e^{x_n}-1}{x_n}=\frac{e^{x_n}-e^0}{x_n-0}=e^{\xi_n}(0<\xi_n<x_n)$$

## 数列递推式bug法（典型题型）
$$x_1=\sqrt{2}, x_{n+1}=\sqrt{2+x_n},\cdots$$

$$单调有界准则证明\\
1. 假设极限存在为A，解A\\
2. 归纳法证上下界A\\
3. 归纳法证单调性

$$
重要方法：[Card#ID/1XSak#连续放缩法]

## 利用函数单调性判断数列单调性

**适用于单调函数**
$$x_{n+1}=f(x_n),取f(x)\\

f'(x)>0,且a_2>a_1\Rightarrow \{x_n\}\nearrow\\
f'(x)>0,且a_2<a_1\Rightarrow \{x_n\}\searrow\\
结论证明：\\
x_{n+1}-x_n=f(x_{n})-f(x_{n-1})=f'(\xi_1)(x_n-x_{n-1})=\cdots=f'(\xi_1)f'(\xi_2)\cdots f'(\xi_{n-1})(x_2-x_1)$$
$$注：由x_{n+1}=f(x_n)型单增递推式变化规律可知（见下图），x_n极限只可能等于x=f(x)交点$$

$$f'(x)<0,\{x_n\}不单调，振荡$$
$$即使f(x)不单调，\{x_n\}也可能单调（数列值域只落在f(x)单调区间内）$$
$$\{x_n\}增减性与f(x)的关系$$
![](pic-advance-math\Markji_1751354211654.png)

## 数列计算常用结论

$$\lim\limits_{n\to \infty}\sqrt[n]{a_1^n+a_2^n+\cdots+a_k^n}=\max\{a_1,a_2,\cdots,a_k\}=a^*\\
a^*=\sqrt[n]{{a^*}^n}\leqslant\sqrt[n]{a_1^n+a_2^n+\cdots+a_k^n}\leqslant\sqrt[n]{n{a^*}^n}=a^*$$

## 数列敛散性结论

$$\lim\limits_{n\to \infty}x_n=a\Leftrightarrow \lim\limits_{n\to \infty}x_{2n}=\lim\limits_{n\to \infty}x_{2n+1}=a（高维同理）$$
$$\lim\limits_{n\to \infty}x_n\ \exists\ \substack{\Rightarrow\\ \not\Leftarrow}\lim\limits_{n\to\infty}(x_{n+1}-x_n)=0（反例：x_n=\sum_{n=1}^{\infty}\frac{1}{n}）$$
$$
\lim\limits_{n\to \infty}\{x_n-y_n\}=0\not\Rightarrow
\lim\limits_{n\to \infty}\frac{\{x_n\}}{\{y_n\}}=1\quad（反例：x_n=\frac{1}{n^2}+\frac{1}{n},y_n=\frac{1}{n^2}）\\
\qquad\qquad\qquad\qquad  \not\Leftarrow \qquad\qquad\qquad\qquad（反例：x_n=n(n+1),y_n=n^2）\\

\lim\limits_{n\to\infty}(x_{n+1}-x_n)=0\not\Rightarrow\lim\limits_{n\to\infty}\frac{x_{n+1}}{x_n}=1（\lim\limits_{n\to \infty}x_n\neq0时成立，反例：x_n=\frac{1}{n!}）\\

\qquad\qquad\qquad\qquad\quad  \not\Leftarrow \qquad\qquad\qquad\quad（反例：x_n=n）$$
$$\lim\limits_{n\to \infty}x_n=a \ \  \substack{\Rightarrow \\ \nLeftarrow}\ \ \lim\limits_{n\to \infty}|x_n|=\pm a(a\neq0)\\
$$
$$\lim\limits_{n\to \infty}x_n= 0\Leftrightarrow\lim\limits_{n\to \infty}|x_n|=0$$

## 三项递推式

**构造两两相邻项之间的递推关系**
$$求和型（等差）：\\
\quad\ x_{n+2}=2x_{n+1}-x_n\\
\Rightarrow x_{n+2}-x_{n+1}=x_{n+1}-x_n\quad
（同侧系数须化一致，否则无法求和）$$
$$递推型：\\
\textcircled{1}逐层向下得两两递推：x_{n+2}-ax_{n+1}=a(x_{n+1}-ax_n)=\cdots=a^n(x_2-ax_1)=a^n b\\
\textcircled{2}两两递推向下的通式：x_{n+2}=a^n b+ a x_{n+1}=a^nb+a(a^{n-1}b+ax_{n})=\cdots=(n+1)a^nb+a^{n+1}x_1\\
（两侧系数须化统一，否则无法向下递推）$$

## 级数求和式

**1. 直接求和、有理化、裂项相消等**

**2. 夹逼准则（放缩）：**
无法求和极限，用放缩法夹逼求和
**3. 单调有界准则：**
判单调性、放缩看上界、下界

**4. 积分定义式：**
注意“n”对应，注意整理变形
$$\lim\limits_{n\to \infty}\sum_{i=1}^{n}f[a+\frac{(b-a)i}{n}]\frac{b-a}{n}=\int_a^b f(x)dx$$
$$\lim\limits_{n\to \infty}\frac{1}{n}(\frac{\sqrt{n^2-1^2}}{n}+\frac{\sqrt{n^2-2^2}}{n}+\cdots+\frac{\sqrt{n^2-n^2}}{n})\Rightarrow f(x)=\sqrt{1-x^2}$$
$$\lim\limits_{n\to \infty}\sqrt[n]{(1+\frac{1}{n})^2(1+\frac{2}{n})^2\cdots(1+\frac{n}{n})^2}\xRightarrow{指数化}f(x)=\ln(1+x)^2$$
**5. 构造导数定义**
$$f(0)=0,f'(0)=1,求\lim\limits_{n\to \infty}\big[f(\frac{1}{n^2})+f(\frac{2}{n^2})+\cdots+f(\frac{n}{n^2})\big]\\
\lim\limits_{n\to \infty}[\frac{f(\frac{1}{n^2})-f(0)}{(\frac{1}{n^2})}\frac{1}{n^2}+\frac{f(\frac{2}{n^2})-f(0)}{(\frac{2}{n^2})}\frac{2}{n^2}+\cdots+\frac{f(\frac{n}{n^2})-f(0)}{(\frac{n}{n^2})}\frac{n}{n^2}]\\
\lim\limits_{n\to \infty}[\frac{1}{n^2}+\frac{2}{n^2}+\cdots+\frac{n}{n^2}]$$

## 连续放缩法

**根据极限构造不等式**
$$\lim\limits_{n\to \infty}x_n=c\rightarrow|x_n-c|（若x_n-c>0,可去绝对值）\\
|x_n-c|\leqslant \frac{3}{4}|x_n-c|\leqslant\cdots \left|\frac{3}{4}\right|^n|x_1-c|\\
\frac{y_{n+1}}{x_{n+1}}=\frac{y_n^2}{\sin x_n}<\frac{\pi}{4}\frac{y_n}{x_n}<\cdots \left(\frac{\pi}{4}\right)^2\frac{y_1}{x_1}$$
$${\color{blue}\star\star重要情形：}\\
x_{n+1}=f(x_n),\ |f'(x)|<1\\
令A=f(A)\\
n\to \infty时，|x_n-A|=|f(x_{n-1})-f(A)|<|f'(\xi_1)||x_{n-1}-A|<\cdots<|f'(\xi_1)\cdots f'(\xi_{n-1})||x_1-A|=0\\
\ \\
n\to \infty时，|x_{n+1}-x_n|<|f'(\xi_1)||x_n-x_{n-1}|<\cdots<|f'(\xi_1)\cdots f'(\xi_{n-1})||x_2-x_1|=0$$

## 极限凑“q<1”技巧

$$0<a_1<a_2,\lim\limits_{n\to \infty}(a_1^{-n}+a_2^{-n})^{\frac{1}{n}}$$
$$I=\lim\limits_{n\to \infty}a_1^{-1}[1+(\frac{a_1}{a_2})^{n}]^{\frac{1}{n}}=a_1^{-1}$$
$$x_n=(1+a)^n+(1-a)^n,证:\lim\limits_{n\to \infty}\frac{x_{x+1}}{x_n}=
\left\{
\begin{array}{ll}
1+|a|, &a\neq0\\
\\
1,& a=0
\end{array}
\right.$$
$$a>0时,\lim\limits_{n\to \infty}\frac{x_{n+1}}{x_n}=\lim\limits_{n\to \infty}\frac{1+a+(\frac{1-a}{1+a})^n(1-a)}{1+(\frac{1-a}{1+a})^n}=1+a\\
a<0时，......$$

## 数列极限$\lim\limits_{n\to \infty}(\Delta)^{\frac{1}{n}}$问题

**首先考虑放缩法**
$$\lim\limits_{n\to \infty}\sqrt[n]{n}=1,\lim\limits_{n\to \infty}\sqrt[n]{a}=1,\lim\limits_{n\to \infty}\sqrt[n]{\frac{1}{n}}=1\\
灵活拆分，根号下为有限项多项式、有限项多项式的倒数、(n,\frac{1}{n})的有限项多项式也成立
$$

## 压轴题型一

$$\star \star“方程的根”类型问题$$

$$证单根：零点定理+单调\\
\ \\
证根的极限（难点）：无统一特征

$$

## 数列极限特例

$$x_1=\sqrt{a}(a>0),x_{n+1}=\sqrt{a+x_n}\ ,......$$

$$\{x_n\}>\sqrt{a}\\
单增：\\
x_{n+1}-x_n=\frac{x_n-x_{n-1}}{\sqrt{a+x_n}+\sqrt{a+x_{n-1}}}=\cdots=\frac{x_2-x_1}{......}>0
\\
有上界：\\
x^2_{n+1}=a+x_n\Rightarrow x_{n+1}=\frac{a}{x_{n+1}}+\frac{x_n}{x_{n+1}}<\sqrt{a}+1$$

# 连续

## 间断点定义及分类

1. 定义注意：
$$\mathring{U}(x_0,\delta)内有定义，且具备以下情形之一：\\

\left\{
\begin{array}{l}
f(x_0)无定义\\
\\
\lim\limits_{x\to x_0^+}f(x)\ 且\lim\limits_{x\to x_0^-}f(x)存在，但\neq f(x_0)\\
\\
\lim\limits_{x\to x_0^+}f(x)\ 或 \lim\limits_{x\to x_0^-}f(x)不存在
\end{array}
\right.$$
2. 间断点分类：
$$
\begin{array}{l}
\lim\limits_{x\to x_0^+}f(x)\ 且\lim\limits_{x\to x_0^-}f(x) \ \exists, \ 第一类间断点
\left\{
\begin{array}{l}
\lim\limits_{x\to x_0^+}f(x)\ =\lim\limits_{x\to x_0^-}f(x)\neq f(x_0),\ 可去间断点 \\
\\
\lim\limits_{x\to x_0^+}f(x)\ \neq\lim\limits_{x\to x_0^-}f(x), \ 跳跃间断点
\end{array}
\right.
\\
\\
\lim\limits_{x\to x_0^+}f(x)\ 或\lim\limits_{x\to x_0^-}f(x)\ \nexists, \ 第二类间断点
\left\{
\begin{array}{l}
无穷间断点\\
振荡间断点\\
\cdots
\end{array}
\right.
\end{array}
$$

## 求间断点思路
（两步走）

1. 在定义域内找无定义点、分段点
2. 逐个求左右极限判断（“无定义点”已知后约分即可）
（函数分式约分前后的区别，仅在于无定义点）

## 无定义间断点的消去问题

$$f(x)=\frac{x-a}{x^2(x-a)}:若分母被分子消去，则为可去间断点$$
$$f(x)=\frac{x-a}{x^2(x-a)^3}:若分母无法被消去，则为无穷间断点\\
相消后，分母在间断点处\left\{
\begin{array}{l}
左右异号，则为异号无穷\\
\\
左右同号，则为同号无穷
\end{array}
\right.$$

## 连续函数运算的连续性
（加减乘除、反函数、复合函数）
  初等函数

$$1. 连续函数四则运算：\\
f(x_0),g(x_0)连续，则f(x_0)\pm g(x_0), f(x_0)g(x_0),\frac{f(x_0)}{g(x_0)}(g(x_0)\neq0)都连续\\
2. 连续函数的反函数连续\\
3. 连续函数的复合函数连续\\
4. 一切初等函数在其定义区间连续\\

$$

# 导数与微分

## 一元微分的定义与构成

$$\Delta y=f'(x_0)\Delta x+\circ(\Delta x)\\
线性主部：f'(x_0)\Delta x$$
![](pic-advance-math\Markji_1751354284917.png)
$$注：可微代表光滑，一阶可微等价于一阶可导（高阶不然）$$

## 导数与极限关系

$$x\to 0时，\frac{f(x)-f(a)}{x-a}\rightarrow A,则称f'(a)=A,\\即\frac{f(x)-f(a)}{x-a}\rightarrow f'(a)\\
$$
$$例:
\lim\limits_{x\to a}\frac{\frac{f(x)-f(a)}{x-a}-f'(a)}{x-a}\neq \lim\limits_{x\to a}\frac{f'(a)-f'(a)}{x-a}$$

## 重要结论

$$有切线不一定有导数\\
y=x^{\frac{1}{3}}在x=0处有切线，但导数无穷大$$

## 定义求导的三要素

$$1. 增量对应\\
\lim\limits_{x\to 0}\frac{f(1+x)-f(1)}{x}\Leftrightarrow \lim\limits_{x\to 1}\frac{f(x)-f(1)}{x-1}\\
2. 一动一静（定点性）\\
3. 双侧性（增量有正有负）

$$
$$双动点导数：\\
\lim\limits_{x\to 0}\frac{f(a+x)-f(a)}{x}\exists=f'(a)\substack{\Rightarrow\\ \not\Leftarrow}\lim\limits_{x\to 0}\frac{f(a+\Delta_1)-f(a+\Delta_2)}{\Delta_1-\Delta_2}=f'(a)\\\left(
\lim\limits_{\Delta_i\to 0}\left[\Delta_1\frac{f(a+\Delta_1)-f(a)}{\Delta_1}-\Delta_2\frac{f(a+\Delta_2)-f(a)}{\Delta_2}\right]\frac{1}{(\Delta_1-\Delta_2)}=f'(a)\right)$$

## 导数存在充要判据

$$直接判断：左导＝右导\\
前提：函数连续、导数存在（若不满足，直接不可导）$$

## 导函数的奇偶性、周期性

$$各阶可导的前提下：\\
\ \\
f(x) 偶 \Rightarrow f'(x) 奇\\
\ \\
g(x) 奇 \Rightarrow g'(x) 偶\\
\ \\
f(x) 偶 \Rightarrow f'(x) 奇  \Rightarrow f''(x) 偶 ......\\
\ \\
f(x) T \Rightarrow f'(x) T  \Rightarrow f''(x) T  \Rightarrow....

$$

## 可导，左导、右导与连续的关系

**用图像记忆**
$$左导  \Rightarrow 左连续，右导  \Rightarrow 右连续\\
\ \\
左导、右导  \Rightarrow 连续（无需左导等于右导）\\
\ \\
可导 \Rightarrow 连续

$$

## 左导右导、导函数的左右极限关系

$$\lim\limits_{x\to x_0^+}\frac{f(x)-f(x_0)}{x-x_0}\neq \lim\limits_{\begin{array}{l}x\to x_1^+ \\x_1\to x_0^+ \end{array}}\frac{f(x)-f(x_1)}{x-x_1}$$
$$注：导数与导函数极限相互独立，互不影响$$

## $f(x_0)$可导与$|f(x_0)|$可导的关系

$$f(x)在x_0处可导，则$$
$$\left\{
\begin{array}{l}
f(x_0)\neq 0时，y=|f(x)|在x_0处可导\\
\\
f(x_0)= 0\ 且f'(x_0)\neq0时，y=|f(x)|在x_0处不可导\\
\\
f(x_0)= 0\ 且f'(x_0)=0时，y=|f(x)|在x_0处可导(y'|_{x_0}=0)\\
\end{array}
\right.$$

## 高阶无穷小求导数问题
$$g(x)=2x+3x^2+x^3+\underbrace{\circ(x^3)}_{f(x)},求g^{(k)}(0)$$

**泰勒公式法直接对应即可**
$$结论：f(x)\ 在x=0处n阶可导,f(x)=\circ{(x^n)}（即\lim\limits_{x\to0}\frac{f(x)}{x^n}=0）, 则\\
\left\{\begin{array}{l}
f^{(k)}(0)=0,k=1,2,\cdots,n\\

g^{(k)}(0)=a_k\cdot k!,k=1,2,\cdots\\

\end{array}\right.$$
$$证f(x)在x=0处的低阶导数，构造低阶即可$$
$$
x=0处f(x)n阶可导，则\exists \ x=0的某邻域，使f(x)\ n-1阶可导$$
$$\begin{array}{rl}
&\lim\limits_{x\to 0}\frac{f(x)}{x^{n-1}}=0\\
\underrightarrow{n-1次洛必达}&\lim\limits_{x\to0}\frac{f^{(n-1)}(x)}{(n-1)!}\ \exists\\
\therefore & \lim\limits_{x\to0}\frac{f^{(n-1)}(x)}{(n-1)!}=\lim\limits_{x\to 0}\frac{f(x)}{x^{n-1}}=0,即\lim\limits_{x\to 0}f^{(n-1)}(x)=0\\
\because & f(x)\ n阶可导\\
\therefore & f^{(n-1)}(0)=0\\
\\
&\lim\limits_{x\to 0}\frac{f(x)}{x^n}=0\\
\underrightarrow{n-1次洛必达} & \lim\limits_{x\to 0}\frac{f^{(n-1)}(x)}{(n-1)!x}=\frac{1}{(n-1)!}\lim\limits_{x\to0}\frac{f^{(n-1)}(x)-f^{(n-1)}(0)}{x-0}=\frac{1}{(n-1)!}f^{(n)}(0)\ \exists\\
\therefore & \frac{1}{(n-1)!}f^{(n)}(0)=\lim\limits_{x\to 0}\frac{f(x)}{x^n}=0
\end{array}$$

## 同阶无穷小求导数问题
$$g(x)\sim ax^2,且二阶可导$$

**泰勒公式法直接对应即可**
$$结论：f(x)在x=0处n阶可导，且\lim\limits_{x\to 0}\frac{f(x)}{ax^n}=1，则f^{(n)}(0)=an!$$
$$
x=0处f(x)n阶可导，则\exists \ x=0的某邻域，使f(x)\ n-1阶可导$$
$$\begin{array}{rl}
&\lim\limits_{x\to 0}\frac{f(x)}{x^{n-1}}=0\\
\underrightarrow{n-1次洛必达}&\lim\limits_{x\to0}\frac{f^{(n-1)}(x)}{(n-1)!}\ \exists\\
\therefore & \lim\limits_{x\to0}\frac{f^{(n-1)}(x)}{(n-1)!}=\lim\limits_{x\to 0}\frac{f(x)}{x^{n-1}}=0,即\lim\limits_{x\to 0}f^{(n-1)}(x)=0\\
\because & f(x)\ n阶可导\\
\therefore & f^{(n-1)}(0)=0
\end{array}$$
$$\begin{array}{rl}
&\lim\limits_{x\to 0}\frac{f(x)}{ax^n}=1\\
\underrightarrow{n-1次洛必达} & \lim\limits_{x\to 0}\frac{f^{(n-1)}(x)}{(n-1)!ax}=\frac{1}{a(n-1)!}\lim\limits_{x\to0}\frac{f^{(n-1)}(x)-f^{(n-1)}(0)}{x-0}=\frac{1}{a(n-1)!}f^{(n)}(0)\ \exists\\
\therefore & \frac{1}{a(n-1)!}f^{(n)}(0)=\lim\limits_{x\to 0}\frac{f(x)}{ax^n}=1
\end{array}$$

## 等价无穷小与导数问题

$$f^{(k)}(x_0)存在，低阶导均为0，则f(x)\sim f^{(k)}(x_0)x^k\\
即f^{(k)}(x_0)存在，且低阶导均为0，则f(x)\sim ax^k\Leftrightarrow  f^{(k)}(0)=ak!$$

## 高阶无穷小求导函数
$$\not\Leftrightarrow$$
幂函数求导函数

$$f(x)=x^{20}\sin\frac{1}{x}$$
$$\left\{
\begin{array}{l}
f(x)\sim\circ(x^{19})\\
f^{(9)}(x)\sim\circ{(x)}\\

\end{array}
\right.$$
$$g(x)=x^{20}\sin\frac{1}{x^5}$$
......

## 幂函数在原点的可导性讨论

$$y=x^u$$
$$\left\{
\begin{array}{ll}
u\geqslant1,& 原点处一定可导\\
0< u<1,&原点一定不可导\\
u<0,&原点处无定义
\end{array}
\right.
\\
\lim\limits_{x\to 0}\frac{x^k-0}{x-0}=\lim\limits_{x\to 0}x^{k-1}(0<k<1)\ \nexists$$

## 基本导数公式
$$(x^ u)',
(a^ x)',(e^ x)',
(\sin x)',(\cos x)',
(\tan x)', (\cot x)',
(\sec x)', (\csc x)',
\\
(\log_a x)', (\ln x)',
(\arcsin x)', (\arccos x)',
(\arctan x)',(\mathrm{arccot} x)',
[\ln(\sqrt{x^2+a^2}+x)]',[\ln|\sqrt{x^2-a^2}+x|]'$$

$$\begin{array}{ll}
(x^ u)'=u x^{u-1}(u=C)\\
\\
(a^ x)'=\ln a \ a^ x (a>0 且 a \neq1) & (e^ x)=e^ x \\
\\
(\sin x)'=\cos x & (\cos x)'=-\sin x \\
\\
(\tan x)'=\sec^2x & (\cot x)'=-\csc^2x \\
\\
(\sec x)'=\sec x \tan x & (\csc  x)'=-\csc x \cot x \\
\\
(\log_ax)'=\frac{1}{x\ln a} (a>0 且 a\neq 1) & (\ln x)'=\frac{1}{x} \\
\\
(\arcsin x)'=\frac{1}{\sqrt{1-x^2}} & (\arccos x)'=-\frac{1}{\sqrt{1-x^2}} \\
\\
(\arctan x)'=\frac{1}{1+x^2} & (arccot x)'=-\frac{1}{1+x^2} \\
\\
[\ln(\sqrt{x^2+a^2}+x)]'=\frac{1}{\sqrt{x^2+a^2}}
& [\ln|\sqrt{x^2-a^2}+x|]'=\frac{1}{\sqrt{x^2-a^2}}
\end{array}$$

## 常见的高阶导数公式
$$e^x,  a^x,
\sin x,\cos x,
x^a,
\frac{1}{x},\ln x$$

$$\begin{array}{ll}
(e^x)^{(n)}=e^x, & (a^x)^{(n)}=a^x\cdot \ln^n a, \\
\\
(\sin x)^{(n)}=\sin(x+\frac{n\pi}{2}), & (\cos x)^{(n)}=\cos(x+\frac{n\pi}{2}), \\
\\
(x^a)^{(n)}=a(a-1)(a-2)\cdots(a-(n-1))x^{a-n}, \\
\\
(\frac{1}{x})^{(n)}=(-1)^{n}\ n! \ x^{-(n+1)},\\
\\
(\ln x)^{n}=(-1)^{n-1}(n-1)!\ x^{-n}
\end{array}$$

## 复合函数求导

$$一阶导：\{f[g(x)]\}'=f'[g(x)]\cdot g'(x)$$
$$高阶导：\{f[g(x)]\}^{(n)}\neq f^{(n)}[g(x)]\cdot g^{(n)}(x)$$

## 幂指函数求导
$$y=u(x)^{v(x)}$$

$$指数化：y=e^{v\ln u}$$
$$对数化：\ln y=v\ln u（定义域变小，函数对应关系不变）$$

## 反函数求导
一阶导（y=f(x)可导，且f'(x)≠0）
二阶导（y=f(x)二阶可导，且f'(x)≠0）

**注意因、自变量对应**
$$一阶导：\varphi'(y)=\frac{1}{f'(x)} $$
$$二阶导：\varphi''(y)=-\frac{f''(x)}{[f'(x)]^3}$$

## 隐函数求导
（两种方法）

**特点：导函数会“耦合”自变量、因变量**
$$一阶导：隐函数存在定理（简便）\\
F(x,y)=0,\ \frac{dy}{dx}=-\frac{F'_x}{F'_y}$$
$$二阶导：方程两边同时自变量求导（不一定）\\
（某点的导数，不必整理，代入简便）$$
$$技巧：利用原方程化简\quad xe^{f(y)}=e^y，求\frac{d^2y}{dx^2}\\
$$

## 参数方程求导

$$一阶导：\frac{dy}{dx}=\frac{y'(t)}{x'(t)}$$
$$二阶导（高阶导与二阶导同理）:\\
\frac{d^2y}{dx^2}=\frac{d[\frac{y'(t)}{x'(t)}]/dt}{\frac{dx}{dt}}=\frac{y''(t)x'(t)-y'(t)x''(t)}{[x'(t)]^3}
（用第一步公式简单）$$
$$注：一阶导（x(t),y(t)均可导，且x'(t)≠0）\\
二阶导（x(t),y(t)均二阶可导，且x'(t)≠0）

$$

## 高阶求导公式（u,v,w 均n阶可导）

$$(u\pm v)^{(n)},(uv)^{(n)},(uvw)'$$

$$(u\pm v)^{(n)}=u^{(n)}\pm v^{(n)}$$
$$(uv)^{(n)}=\sum_{k=0}^nC^k_nu^{(n-k)v^{(k)}}$$
$$(uvw)'=u'vw+uv'w+uvw'$$

## 切线方程与法线方程

$$切线方程：y-f(x_0)=f'(x_0)(x-x_0)$$
$$法线方程：y-f(x_0)=-\frac{1}{f'(x_0)}(x-x_0)$$

## 已知可导反求参数（两步走）

1. 连续
2. 左导=右导

## 判断导数存在的四条常用结论

$$1. \ 若f(x)在x=x_0处连续，\\ \ \ \ \ 且\lim\limits_{x_0\to x_0}\frac{f(x)-A}{x-x_0}=B,\\ \ \ \ \ 则f(x_0)=A,f'(x_0)=B$$
$$2. \ y=f(x)在x_0处可导，y=g(x)在x_0处连续但不可导，则\\
\ \ \ F(x)=f(x)\cdot g(x)可导的充分必要条件是f(x_0)=0\\
\star\ 证明：\lim\limits_{x\to x_0}\frac{f(x)g(x)-f(x_0)g(x_0)}{x-x_0}=\lim\limits_{x\to x_0}\frac{f(x)g(x)-f(x_0)g(x)+[f(x_0)g(x)-f(x_0)g(x_0)]}{x-x_0}\\=\lim\limits_{x\to x_0}\frac{f(x)-f(x_0)}{x-x_0}g(x)+\lim\limits_{x\to x_0}\frac{g(x)-g(x_0)}{x-x_0}f(x_0)=f'(x_0)g(x_0)+\lim\limits_{x\to x_0}\frac{g(x)-g(x_0)}{x-x_0}f(x_0)$$
$$3. 若\varphi(x)在x=a处连续，\\ \ \ \ f(x)=|x-a|\varphi(x),\\
\ \ \ \varphi(a)=0\Leftrightarrow f'(a) =0（函数分段定义法证得）$$
$$4. \ f(x)=(x-x_0)^k|x-x_0|\\
\ \ \ \ f(x)在x=x_0处 k阶可导 且为0，f^{(k+1)}(x_0)不存在（函数分段定义法证得）$$

$$重难点：
可导性判断，熟练常用结论；\quad
定义求导，{\color{blue}\star 需灵活构造导数定义}$$

## 某点导函数不存在求导结论

$$\ f(x)在x=x_0的某去心邻域内可导，且f(x)在x=x_0处连续，\\若\lim\limits_{x\to x_0}f'(x)=A,则f'(x_0)=A\\（洛必达证得）$$
$$例：求f'(0)\\
f(x)=e^{x^{\frac{2}{3}}}-1-x^{\frac{2}{3}}\\
f'(x)=\frac{2}{3}e^{x^{\frac{2}{3}}}\cdot \frac{1}{\sqrt[3]{x}}-\frac{2}{3}\cdot \frac{1}{\sqrt[3]{x}}\\
$$
[Card#ID/1XxPL#变限积分函数在间断点的可导性]

## 低阶求导技巧

$$1. 导函数寻找规律\\
f(x)=(e^x-1)(e^x-2)\cdots(e^{nx}-n)\Rightarrow\\
f'(0)=(e^x-2)(e^x-3)\cdots(e^x-n)|_{x=0}=(-1)^{n-1}(n-1)!$$
$$2. 复杂乘除因式组合采用对数化求导 $$

## 高阶求导技巧

$$1. 泰勒公式（某一点导数）\\
f(x)=a_0+a_1x+a_2x^2+\cdots +a_nx^n\\
x=0处直接展开（好用）:\frac{f^{n}(0)}{n!}=a_n\\\\
x=x_0处凑t+x_0，变量代换:
f^{(n)}(x)|_{x=1}\xlongequal{x=t+1}f^{(n)}(t+1)|_{t=0}$$
$$2. 导数奇偶性\\
f^{(n)}(x)为奇函数\Rightarrow f^{(n)}(0)=0\\
奇函数\quad f^{(2k)}(0)=0\\
偶函数\quad f^{(2k+1)}(0)=0$$
$$3. 找规律归纳法\\
f(x)=(x^3-1)^n=(x-1)^n(x^2+x+1)^n\Rightarrow\\
f^{(n)}(1)=n!(x^2+x+1)^n|_{x=1}=n!\\
\ \\
f(x)=e^x\sin x\Rightarrow\\
f^{(n)}(x)=e^x\sin(x+\frac{n\pi}{4})\cdot 2^{\frac{n}{2}}$$
$$4. 莱布尼茨高阶导数公式，含多项式k项后为零\\
(uv)^{(n)}=\sum_{k=0}^nC^k_nu^{(n-k)v^{(k)}}$$

# """中值定理"""

## 考情分析

$$难点（不等式证明）：拉格朗日中值、泰勒中值\\
$$

## 介值定理

$$f(x)在[a,b]连续，\\
m\leqslant\mu \leqslant M,\ \exist\ \xi\in[a,b],\ 使f(\xi)=\mu\\
f(x_1)\leqslant\mu \leqslant f(x_2),\ \exist\ \xi\in[x_1,x_2],\ 使f(\xi)=\mu$$

## 平均值定理

$$f(x)在[a,b]连续，a<x_1<x_2<\cdots<x_n<b,\\
\exist \ \xi\in[x_1,x_n], \ 使得f(\xi)=\frac{f(x_1)+f(x_2)+\cdots+f(x_n)}{n}$$

## 零点定理及推广

$$f(x)在[a,b]连续，
f(a)\cdot f(b)<0, \\
\exist \ \xi\in (a,b), \ 使得f(\xi)=0$$
$$注意区间开闭：
\xi\in (a,b)\Rightarrow \xi\in [a,b]$$
**推广：（不可直接用）**
$$\left\{
\begin{array}{l}
\lim\limits_{x\to a^+}f(x)\cdot\lim\limits_{x\to b^-}f(x)<0,
\ \ \ \cdots \\
\\
\lim\limits_{x\to a^+}f(x)\cdot f(b)<0,
\ \ \ \cdots \\
\\
\lim\limits_{x\to a^+}f(x)\cdot\lim\limits_{x\to +\infty}f(x)<0,
\ \ \ \cdots
\end{array}
\right.$$

## 费马定理

$$f(x)在x_0处\left\{
\begin{array}{l}
可导\\
\\
取极值
\end{array}
\right.
,则f'(x_0)=0$$

## 罗尔定理及推广

$$f(x)在\left\{
\begin{array}{l}
[a,b]上连续\\
\\
(a,b)内可导\\
\\
f(a)=f(b)
\end{array}
\right.$$
$$\exists\ \xi\in(a,b),使得\ f'(\xi)=0$$
**推广：（不可直接用，需分类讨论）**
$$\left\{
\begin{array}{l}
\lim\limits_{x\to a^+}f(x)=\lim\limits_{x\to b^-}f(x),\ \ \ \cdots \\
\\
\lim\limits_{x\to a^+}f(x)=f(b),
\ \ \ \cdots \\
\\
\lim\limits_{x\to a^+}f(x)=\lim\limits_{x\to +\infty}f(x),
\ \ \ \cdots
\end{array}
\right.$$

## 拉格朗日中值定理

$$f(x)在\left\{
\begin{array}{l}
[a,b]上连续\\
\\
(a,b)内可导
\end{array}
\right.$$
$$\exists \ \xi\in(a,b),使得\\
\\
\left\{
\begin{array}{l}
f(b)-f(a)=f'(\xi)(b-a)\\
\\
f'(\xi)=\frac{f(b)-f(a)}{b-a}（斜率两点式）
\end{array}
\right.$$

## 柯西中值定理

**柯西中值定理不是两个拉格朗日相除**
$$f(x)在\left\{
\begin{array}{l}
[a,b]上连续\\
\\
(a,b)内可导\\
\\
g'(x)\neq0
\end{array}
\right.$$
$$\exists \ \xi\in(a,b),使得\ \frac{f(b)-f(a)}{g(b)-g(a)}=\frac{f'(\xi)}{g'(\xi)}$$

## 积分中值定理及推论

$$f(x)在[a,b]上连续\\
\exists \ \xi\in[a,b],使得
\int_a^bf(x)dx=f(\xi)(b-a)\\
 \ \\
介值定理证明：\\
\min[f(x)](b-a)\leqslant\int_a^bf(x)dx\leqslant\max[f(x)](b-a)$$
**推论：（不可直接使用）**
$$f(x)在[a,b]上连续，\\
\exists \ \xi\in(a,b),使得\int_a^bf(x)dx=f(\xi)(b-a)\\
\ \\
拉格朗日中值证明：\\
F(x)=\int_a^xf(t)dt\\
F(b)-F(a)=\int_a^bf(x)dx=f(\xi)(b-a)\quad \xi\in(a,b)$$

##

第一积分中值定理及推广

**不可直接使用**
$$\left\{
\begin{array}{l}
f(x)在[a,b]上连续\\
\\
g(x)可积且不变号
\end{array}
\right.\\
\exists\ \xi\in[a,b],使得\int_a^bf(x)g(x)dx=f(\xi)\int_a^bg(x)dx\\
\ \\
介值定理证明：\\
\int_a^b\min[f(x)]g(x)dx\leqslant \int_a^bf(x)g(x)dx\leqslant\int_a^b\max[f(x)]g(x)dx\\
\min[f(x)]\cdot\int_a^bg(x)dx\leqslant \int_a^bf(x)g(x)dx\leqslant\max[f(x)]\cdot\int_a^bg(x)dx$$
**推广：（不可直接使用）**
$$\left\{
\begin{array}{l}
f(x),g(x)在[a,b]上连续\\
\\
g(x)可积不变号
\end{array}
\right.\\
\exists\ \xi\in(a,b),使得\int_a^bf(x)g(x)dx=f(\xi)\int_a^bg(x)dx\\
\ \\
柯西中值定理证明：\\
H(x)=\int_a^xf(t)g(t)dt,\quad R(x)=\int_a^xg(t)dt\\
\frac{H'(\xi)}{R'(\xi)}=\frac{H(b)-H(a)}{R(b)-R(a)}\longrightarrow
\frac{f(\xi)g(\xi)}{g(\xi)}=\frac{\int_a^bf(t)g(t)dt}{\int_a^bg(t)dt}$$

## 泰勒公式

**注意泰勒公式的条件**
**带拉格朗日余项：**
$$f(x)在U(x_0)内(n+1)阶可导，对任意x\in U(x_0)\\

f(x)=f(x_0)+f'(x_0)(x-x_0)+\frac{f''(x_0)}{2!}(x-x_0)^2+\cdots +\frac{f^{(n)}(x_0)}{n!}(x-x_0)^n+R_n(x)
\\
R_n(x)=\frac{f^{(n+1)}(\xi)}{(n+1)!}(x-x_0)^{n+1} ,\ \ \xi \in(x_0,x)$$
**带佩亚诺余项：**
$$f(x)在x=x_0处n阶可导,则（默认x\to x_0）\\

f(x)=f(x_0)+f'(x_0)(x-x_0)+\frac{f''(x_0)}{2!}(x-x_0)^2+\cdots +\frac{f^{(n)}(x_0)}{n!}(x-x_0)^n+R_n(x)
\\
\\
R_n(x)=\circ((x-x_0)^n) $$
$$泰勒公式本质：利用导数将函数展开为多项式形式\\
最多可展开到某阶导数不存在为止，如f(x)=x^3\sin\frac{1}{x}=\circ(x^2)$$

## 拉格朗日余项展开，佩亚诺余项展开，幂级数展开区别

$$拉格朗日余项展开：\\
泰勒中值展开，在定义域内，中值估算误差，中值\xi受x,x_0影响，始终依赖于f(x)\\
注：\xi \neq\xi(x)，不一定满足函数映射要求（一对一、多对一）$$
$$佩亚诺余项展开前提：x\to x_0$$
$$幂级数展开：\\
在收敛域内，幂级数展开等价于函数本身$$

## 导数零点定理

**不可直接使用**
$$\left\{
\begin{array}{l}
f(x)在[a,b]上可导\\
\\
当f'_+(a)\cdot f'_-(b)<0时
\end{array}
\right.\\
\exists \ \xi\in(a,b),使得\ f'(\xi)=0\\
\ \\
费马定理证明：\\
假设\lim\limits_{x\to a^+}\frac{f(x)-f(a)}{x-a}>0\quad \lim\limits_{x\to b^-}\frac{f(x)-f(b)}{x-b} <0 \\
即\ \exists\ \xi\in(a,b)，使得f(\xi)>f(a),f(b)\\
故f(x)在(a,b)上取到最大值，f(x)可导，即极大值\\
由费马定理可知，\exists\ f'(\xi)=0$$

## 导数介值定理

**不可直接使用**
$$\left\{
\begin{array}{l}
f(x)在[a,b]上可导\\
\\
f'_+(a)\neq f'_-(b)
\end{array}
\right.
当\mu介于f_+'(a),f'_-(b)之间时，\\

\exists\ \xi\in(a,b),使得f'(\xi)=\mu\\
\ \\
费马定理证明：\\
令F(x)=f(x)-\mu x即可转化为证明导数零点定理$$

## 常用辅助函数构造形式
$$\Delta'\Box+ \Delta\Box'，\Delta'\Box - \Delta\Box'，\Delta\Delta'，\frac{\Delta'}{\Delta}，\Delta'+k\Delta，
\Delta'+\Box'\Delta，\Delta$$

$$\Delta'\Box+ \Delta\Box': \Delta\Box$$
$$\Delta'\Box - \Delta\Box': \frac{\Delta}{\Box}$$
$$\Delta\Delta':\Delta^2$$
$$\left.
\begin{array}{l}
\frac{\Delta'}{\Delta}:\ln\Delta\\
\\
\Delta'+k\Delta:e^{kx+b}\cdot\Delta\\
\\
\Delta'+\Box'\Delta:e^\Box\cdot\Delta
\end{array}
\right\}$$
$$\left.
\begin{array}{l}
\Delta:\int_a^xf(t)dt

\end{array}
\right.$$
$$注：(\Delta+b)'=\Delta'$$

## 辅助函数构造经验

1. 辅助函数不唯一（与条件不一定相通）
2. 共同成分可能被消去，注意观察
3. 阶数相差大于一，考虑相消（一般为加减）
$$f''(\xi)=f(\xi)\Rightarrow e^\xi[f''(\xi)+f'(\xi)]=e^\xi[f'(\xi)+f(\xi)]$$
4. 善用除法构造ln函数，借用不定积分构造辅助函数
$$f'(\xi)+(1-\xi) f(\xi)=0\rightarrow \frac{f'(x)}{f(x)}+(1-x)=0\\
\ln\Delta（取\ln内函数即可；仅找辅助函数而已，不加绝对值无碍）$$

## 中值证明选择框架
零点定理、介值定理、费马定理、罗尔定理、拉格朗日中值定理、柯西中值定理、泰勒中值

$$\begin{array}{lll}
f(\xi)=0:零点 & & f(\xi)=u:介值\\
\quad \quad\uparrow \ \downarrow & &  \quad \quad\uparrow\ \downarrow & （导函数、原函数灵活转换）\\
f'(\xi)=0:费马、罗尔 & \longleftarrow & f'(\xi)=u:拉格 \\
\quad\quad\vdots\\
f''(\xi)=0\cdots
\end{array}\\
\ \\
费马\longrightarrow罗尔\xrightarrow{特殊}拉格\xrightarrow{特殊}柯西（合适为佳）\\
同一函数在同一区间使用上述四定理，所得中值相同$$
$$注：定理最多迭代两层（多层证明灵活混用定理）\\
中值证明题以微分中值定理为主题，积分中值定理也有可能$$
$$泰勒中值展开（高阶中值）:相对独立特殊$$

## 泰勒公式证明框架

**主要以**不等式证明**考查泰勒中值，灵活使用常用不等式**
$$重要暗示：{\color{blue}闭区间}二阶及以上可导（首要考虑泰勒）\\
1.选点（题目会有暗示）：
\left\{\begin{array}{l}
端点、中点\\
极值点、最值点、介值点、中值点\\
一阶导信息的点x_0\\
一般点x
\end{array}\right.\\
2.展开，逐步向结果靠拢（基本不等式、放缩、介值定理等）$$
$$注：(b-a)^2:\frac{a+b}{2}（展开点、被展开点灵活）$$

## 中值定理证明重要经验

**中值证明题两大切入点：1.辅助函数  2.选点**
1. 纯用微分中值定理易，辅用函数中值定理难
2. 逆向分析，由所证推所需，正向书写

## 中值定理证明重要结论
$$\lim\limits_{x_0\to x_0}\frac{f(x)-A}{x-x_0}=B$$

$$若f(x)在x=x_0处连续，且\lim\limits_{x_0\to x_0}\frac{f(x)-A}{x-x_0}=B，则f(x_0)=A,f'(x_0)=B$$

## 根的唯一性证明

$$零点定理+单调性$$

## 双中值证明

**不同函数在同一区间：**
$$1. 拉格+拉格：
寻找拉格朗日“分式项”的关联\\
\ [e^xf(x)]'\big|_{x=\eta}=\frac{e^bf(b)-e^af(a)}{b-a}=\frac{e^b-e^a}{b-a}=(e^x)'\big|_{x=\xi}
\ \\
2.柯西+拉格朗日：\\
\frac{f'(\xi)}{f'(\eta)}=\frac{e^b-e^a}{b-a}\cdot e^{-\eta}\\
\ \\
注：\xi,\eta可能相等
$$
**同一函数在不同区间：**
$$拉格朗日分式逆向分析凑\\f'(\xi_1)f'(\xi_2)=1\\
\frac{1}{f(\xi_1)}+\frac{1}{f(\xi_2)}=a （以\ \xi分开，分别拉格朗日）\\
\ \\
注：\xi_1\neq\xi_2$$

## 中值不等式证明
拉格朗日、泰勒中值

$$拉格朗日：f''(\xi)=\frac{f'(\eta_2)-f'(\eta_1)}{\eta_2-\eta_1}>0$$
$$泰勒中值：利用基本不等式等$$

## 区分单导数中值与双导数中值

$$单导数中值：\\
\frac{f(a)-f(c)}{g(c)-g(b)}=\frac{f'(c)}{g'(c)}\rightarrow \frac{f(a)-f(x)}{g(x)-g(b)}=\frac{f'(x)}{g'(x)}\rightarrow g'[x](f(a)-f(x))-f'[x](g(x)-g(b))=0\\
\ \\
即F(x)=[g(x)-g(b)]\cdot [f(a)-f(x)]$$
$$双导数中值：柯西中值$$

## 中值定理同一函数在同一区间使用问题

**费马、罗尔、拉格、柯西**
**对同一函数在同一区间的使用不可重复**
$$f(x)各阶可导，f(0)=f(1)\\
\exist\ \xi_1\in(0,1),使f'(\xi_1)=0（费马定理）\\
\exists\ \xi_1\in(0,1),使f'(\xi_1)=0（罗尔定理）
\\
 \exists\ \xi_1\in(0,1),使f'(\xi_1)=\frac{f(1)-f(0)}{1-0}=0（拉格朗日中值定理）\\
\exists\ \xi_1\in(0,1),g(x)=x,使f'(\xi_1)=\frac{f(1)-f(0)}{g(1)-g(0)}=0（柯西中值定理）

$$

## 重要题型（反解）

$$\frac{a}{f'(\xi)}+\frac{b}{f'(\eta)}=a+b$$

$$f'(\xi)=\frac{f(c)-f(0)}{c-0}=\frac{f(c)}{c}\quad
f'(\eta)=\frac{f(1)-f(c)}{1-c}=\frac{1-f(c)}{1-c}\\
\frac{a\cdot c}{f(c)}+\frac{b(1-c)}{1-f(c)}=a+b，整理后得：\\
(c-f(c))[a(1-f(c))-bf(c)]=0\quad取定义区间上的点即可$$
$$注：反解题型两种步骤
\left\{\begin{array}{ll}
\textcircled{1}必要解法：&分子=分子，分母=分母\\
\textcircled{2}充要解法：&拆重组为因式相乘=0
\end{array}\right.$$

## 压轴题型一
$$\star \star形如\left|\int_a^bf(x)dx\right|\leqslant \frac{M}{c},M=\max\{|f'(x)|\}问题$$

**非特殊暗示，用拉格朗日，或泰勒展开**
$$1. 拉格朗日，或泰勒展开
\quad(F(x)=\int_a^xf(t)dt;\quad M=\max\{|f'(x)|\})\\
2. 分部积分法构造f'(x)\qquad\left|\int_a^bf(x)dx\right|\leqslant \frac{M}{c}\\
f(0)=f(1)=0\\
\left| \int_0^1f(x)dx \right|=\left| xf(x)\bigg|_0^1-\int_0^1xf'(x)dx \right|\leqslant \max\{|f'(x)|\}\int_0^1xdx=\frac{M}{2}
$$

## 压轴题型二

$$\star \star求解\lim\limits_{x\to 0}\theta(x)问题$$

拉格朗日中值、泰勒中值

**根据所给条件将 θ(x) “调出来”**
$$双式结合\left\{\begin{array}{l}
拉格多次展开，结合\\
泰勒不同阶展开,结合
\end{array}\right.\rightarrow 极限约分$$

## 压轴题型三
$$\star\star抽象函数不等式证明$$

**泰勒中值展开**
$$动点展开：\\
f(x)在[0,1]上二阶可导，且当0\leqslant x\leqslant 1时，|f(x)|\leqslant 1，|f''(x)|\leqslant 2. \ 证0\leqslant x\leqslant 1时，|f'(x)|\leqslant3\\
f(u)=f(x)+f'(x)(u-x)+\frac{f''(\xi)}{2!}(u-x)^2\\
$$
$$极值点展开：\\
f(x)在[0,1]上有二阶连续导数，f(0)=f(1)=0，\max\limits_{0\leqslant x\leqslant 1}f(x)=2，证\min\limits_{0\leqslant x\leqslant 1}f''(x)\leqslant -16\\
f(u)=f(x_0)+f'(x_0)(u-x_0)+\frac{f''(\xi)}{2!}(u-x_0)^2
$$

# 一元微分学的应用

## 考情分析

难点：抽象函数各阶导数与极值点，拐点，单调性的判定问题
条件多，不易分清
经常求各阶导数，繁琐

## 极值的定义

$$f(x)在U(X_0)内有定义，对于任意x\in \mathring{U}(x_0,\delta),\ \ \ f(x)<f(x_0)(或f(x)>f(x_0))，则称f(x_0)为极值$$
$$注：定义区间端点无法取到极值\\
常函数无法取到极值
$$

## 最值的定义

$$设x_0为f(x)在定义域内一点，若对于f(x)定义域内任一异于x_0的一点x，均有\\
f(x)\leqslant f(x_0)(或f(x)\geqslant f(x_0)),则称f(x_0)为f(x)最值$$
$$注：开区间端点无法取到最值\\
若为最值段，则可取到无限个最值点$$

## 拐点的定义

$$f(x)在区间{\color{blue}连续}，y=f(x)的凹凸性的分界点称为拐点$$

## 凹凸性定义

$$函数区间连续，对区间内任意x_1,x_2, 使\\f(\frac{x_1+x_2}{2})>\frac{f(x_1)+f(x_2)}{2}凸\\f(\frac{x_1+x_2}{2})<\frac{f(x_1)+f(x_2)}{2}凹$$

## 单调性与导数关系

$$f(x)一阶可导，f'(x)>0(<0)\Rightarrow f(x)单增（单减）$$
$$f(x)一阶可导，f'(x)\geqslant0(\leqslant0)（等号仅在有限点处、或无限不连续点处取到）\Leftrightarrow f(x)单增（单减）$$

$$f'(x_0)>0\not\Rightarrow \exists \ x\in U(x_0)，使f(x)\nearrow$$
$$f'(x_0)>0，且f'(x_0)连续\Rightarrow \exists \ x\in U(x_0)，使f(x)\nearrow$$

## 复合函数与反函数单调性

$$y=f[g(x)]:  同增异减$$
$$y=f(x),y=f^{-1}(x):  单调性一致$$

## 凹凸性与导数的关系

$$f(x)二阶可导，f''(x)>0(<0)\Rightarrow f(x) 是凹函数（凸函数）$$
$$f(x)二阶可导，f''(x)\geqslant0(\leqslant0)（等号仅在有限点处、或无限不连续点处取到）\ 或f'(x)\nearrow(\searrow) \\\Leftrightarrow f(x) 是凹函数（凸函数）$$

$$f''(x_0)>0\not\Rightarrow \exists \ x\in U(x_0)，使f(x)\ 为凹函数$$
$$f''(x_0)>0，且f''(x_0)连续\Rightarrow \exists \ x\in U(x_0)，使f(x)\ 为凹函数$$

## 凹凸性不等式拓展

$$凹: f(\frac{x_1+x_2+\cdots+x_n}{n})<\frac{f(x_1)+f(x_2)+\cdots+f(x_n)}{n}$$
$$凸: f(\frac{x_1+x_2+\cdots+x_n}{n})>\frac{f(x_1)+f(x_2)+\cdots+f(x_n)}{n}$$

## 极值点判断
必要条件，三个充分条件

**必要条件：**
$$若x_0为极值点，且f'(x_0)可导，则f'(x_0)=0$$
**充分条件：**
$$f(x)在x=x_0连续，在\underline{}\mathring{U}(x_0,\delta)内可导，f'(x)左右变号$$
$$f(x)在x=x_0处二阶可导，且f'(x_0)=0,f''(x_0)\neq0\\(或\mathring{U}(x_0,\delta)内，仅在x_0处，f''(x)=0)，则\\
\begin{array}{}
\left\{
\begin{array}{l}
f''(x_0)>0,极小值\\
f''(x_0)<0,极大值
\end{array}
\right.
\left\{
\begin{array}{l}
f''(x)\geqslant0,极小值\\
f''(x)\leqslant0,极大值
\end{array}
\right.
\end{array}$$
$$f(x)在x=x_0处n阶可导，且f^{(m)}(x_0)=0(m=1,2,\cdots,n-1),f^{(n)}\neq0(n\geqslant 2)\\(或\mathring{U}(x_0,\delta)内，仅在x_0处，f^{(n)}(x)=0),则\\
\begin{array}{}
n为偶数\left\{
\begin{array}{l}
f^{(n)}(x_0)>0，f(x_0)取极小值\\
f^{(n)}(x_0)<0，f(x_0)取极大值
\end{array}
\right. &
n为偶数\left\{
\begin{array}{l}
f^{(n)}(x)\geqslant0，f(x_0)取极小值\\
f^{(n)}(x)\leqslant0，f(x_0)取极大值
\end{array}
\right.
\end{array}
$$

## 拐点判断

必要条件，三个充分条件

**必要条件：**
$$若x_0为拐点，且f''(x_0)存在，则f''(x_0)=0$$
**充分条件：**
$$f(x)在x=x_0连续，在\underline{}\mathring{U}(x_0,\delta)内二阶可导，f''(x)左右变号$$
$$f(x)在x=x_0处三阶可导，且f''(x_0)=0,f'''(x_0)\neq0\\ \bigg(或\mathring{U}(x_0,\delta)内，仅在x_0处，f'''(x)=0\left\{
\begin{array}{l}
f'''(x)\geqslant0\\
f'''(x)\leqslant0
\end{array}
\right.\bigg)$$
$$f(x)在x=x_0处n阶可导，且f^{(m)}(x_0)=0(m=2,3,\cdots,n-1),f^{(n)}\neq0(n \geqslant 3)，则\\当n为奇数时，x=x_0是拐点
\\
\bigg(或\mathring{U}(x_0,\delta)内，仅在x_0处，f^{(n)}(x)=0\left\{
\begin{array}{l}
f^{(n)}(x)\geqslant0\\
f^{(n)}(x)\leqslant0
\end{array}
\right.\bigg)$$

## 一元微分重要经验

1. 善用极值点划分单调区间（函数区间可导，导函数为零的点之间必单调）
2. 借助ln函数分析幂指函数单调性
3. 求最值直接代驻点、端点，无须分析极值点

## 极值点与拐点重要结论
$$开区间唯一极值点\\
极值点、拐点同时存在点\\
f(x)=(x-a)^ng(x)判极值点与拐点\\
f(x)=(x-a_1)^{n_1}\cdot(x-a_2)^{n_2}\cdots (x-a_k)^{n_k}判极值点、拐点个数$$

$$1. 若f(x)在(a,b)连续，x=x_0\in(a,b)是唯一极值点\\则x=x_0也是(a,b)的唯一最值点（闭区间考虑端点，开区间只考虑极值点）$$
$$2. 可导点不同时为极值点与拐点，不可导点可同时为极值点与拐点\\
注：极值点处f'(x_0)=0，若也为拐点，即f(x)在x<x_0,x>x_0两侧凹凸性不一致，可反证不是拐点$$
$$3. 多项式函数f(x)=(x-a)^ng(x)\ \ (n>1),且g(a)\neq0,则\\
\left\{
\begin{array}{l}
n为偶数，x=a是极值点 \\
n为奇数，x=a是拐点
\end{array}
\right.$$
$$4. 多项式函数f(x)=(x-a_1)^{n_1}\cdot(x-a_2)^{n_2}\cdots (x-a_k)^{n_k}\\其中n_i是正整数，a_i是实数且a_i两两不等，\\
记k_1为n_i=1的个数，k_2为n_i>1且n_i为偶数的个数，k_3为n_i>1且n_i为奇数的个数，则\\
\left\{
\begin{array}{l}
极值点个数为k_1+2k_2+k_3-1\\
拐点个数为k_1+2k_2+3k_3-2
\end{array}
\right.$$
$$注：极值点可利用“穿针引线法”大致分析$$

## 穿针引线法

$$y=(x-1)(x-2)^2(x-3)^3(x-4)^4\\

奇穿偶不穿，两端取极限

$$
$$注：穿针引线法仅可分析趋势与正负，无法分析拐点$$

## 极值点、最值点、拐点的可疑点

$$极值点\subset \{一阶导为零（驻点），不可导点\}$$
$$最值点\subset\{一阶导为零（驻点），不可导点，端点\}$$
$$拐点\subset\{二阶导为零，二阶导不存在\}$$

## 极值点、驻点、极值、拐点规范写法

$$极值点（驻点同理）：x_0\ 或\ x=x_0$$
$$极值：f(x_0)$$
$$拐点：(x_0,y_0)$$

## 求渐近线顺序

$$先“铅直”，后“水平”，再“斜渐近线”\\

（在单侧无穷处，斜渐近线与水平渐近线不共存）\\

水平：y=C\\
铅直：x=a\\
斜渐近线：y=ax+b$$

## 曲率公式，曲率半径与中心

$$曲率公式：\\
k=\frac{|y''|}{[1+(y')^2]^{\frac{3}{2}}}（k>0,所以有绝对值）\\
\ \\
k=\frac{|y''(t)x'(t)-y'(t)x''(t)|}{[x'(t)^2+y'(t)^2]^\frac{3}{2}}（绝对值已考虑到）$$
$$曲率半径：R=\frac{1}{k}=\frac{[1+(y')^2]^{\frac{3}{2}}}{|y''|} (y''\neq 0)\\
曲率中心：
\begin{cases}
a=x-y'\frac{1+(y')^2}{y''}\\

b=y+\frac{1+(y')^2}{y''}
\end{cases}$$

## 曲线有公切线、公切圆

$$公切线：
\left\{
\begin{array}{l}
f(x_0)=g(x_0)\\
f'(x_0)=g'(x_0)
\end{array}
\right.$$
$$公切圆：
\left\{
\begin{array}{l}
f(x_0)=g(x_0)\\
f'(x_0)=g'(x_0)\\
|f''(x_0)|=|g''(x_0)|
\end{array}
\right.$$

## 相关变化率问题

$$\text { 若函数 } y=f(x),
\begin{cases}x=x(t)  \\
 y=y(t) \end{cases}均可导, 则\frac{\mathrm{d} y}{\mathrm{~d} t}=\frac{\mathrm{d} y}{\mathrm{~d} x} \frac{\mathrm{d} x}{\mathrm{~d} t}=f^{\prime}(x) \frac{\mathrm{d} x}{\mathrm{~d} t}$$

## 讨论“含参数”方程的根
$$2x^3-9x^2+12x+k=0$$

$$1. 方程变形，令k=F(x)=-2x^3+9x^2-12x\\
讨论极小值m、极大值M、端点值与k之间的关系\\
2. 直接分析函数性态，含参数讨论$$

## 隐函数判断极值点、拐点
$$2y^3-2y^2+2xy-x^2=1$$

$$一般用第二充分条件：\\
f'(0)=0,且f''(0)\neq0\\
f''(0)=0,且f'''(0)\neq0\\
\ \\
F'_y=0时，定义法讨论，对方程进行分析$$

## 微分方程判断极值点、拐点
$$2f''(x)+[f'(x)]^2=3x，在(0,f(0))处$$

$$分类讨论f'(0)=0,f''(0)\neq0的情况（解微分方程过于复杂）\\

f'''(x)=\frac{1}{2}[3-2f'(x)f''(x)]$$

## 恒等式证明

$$1. 最大值等于最小值\\
2. 一阶导为零

$$

# 零点问题

## 罗尔定理推论

$$f^{(n)}(x)=0至多有k(k\geqslant0)个根，则f(x)=0至多有k+n个根\\
\ \\
罗尔定理反证:\\
若f(x)=0有大于k+n个根\\
根据罗尔定理，可得出f^{(n)}存在多于k个根，与原题设不符$$

## 实系数奇次方程至少有一个根

最高项阶次为奇数

# 不等式判定

## 考情分析

收录一般微分不等式、积分不等式式的判定方法
较复杂情形与中值定理联系颇深，归于中值定理方法中

## 具体型不等式判定

**1. 函数性态分析（最多求二阶导，灵活构造）：**
$$幂指函数取\ln分析单调性$$
**2. 拉格朗日中值**
$$ 不等式（统一形式比大小）：\\
\frac{b-a}{1+b^2}\leqslant \arctan b-\arctan a\leqslant\frac{b-a}{1+a^2}$$

## 抽象型不等式判定

**1.函数性态**
$$辅助函数\\
f(x)f'(x)>0\\
\Rightarrow[f^2(x)]'>0\\
\Rightarrow F(x)=f^2(x)\nearrow$$
**2. 拉格朗日中值：**
$$构造不等式：\left\{
\begin{array}{l}
xf'(x)-f(x)=xf'(x)-[f(x)-f(0)]=xf'(x)-f'(\xi)\cdot x\ \ \ (f(0)=0)\\
\\
b-a-\frac{f(b)}{f'(b)}=\frac{f(b)-f(a)}{f'(\xi)}-\frac{f(b)}{f'(b)}=\frac{f(b)}{f'(\xi)}-\frac{f(b)}{f'(b)}\ \ \ (f(a)=0)
\end{array}
\right.$$
**3. 泰勒中值展开：**
$$f(x)二阶可导，f(0)=0，f'(0)>0，f''(x)>0，判f(0) \diamond f(\frac{1}{2})$$

## 一般不等式（李六）

**根据题目分析转化，非考研专属考点，灵活是关键**
$$x_1x_2>e^2$$
$$\int_0^xf(t)dt\geqslant\frac{1}{2}[xf(x)+x]$$
$$\int_0^1(\frac{2}{3}-x)f(x)dx\geqslant \frac{1}{6}$$

# ""不定积分""

## 考情分析

1. 只有f(x)连续时，才考原函数相关性质
2. 不定积分只考三大方法：凑微分法、换元积分法、分部积分法
不定积分计算很有限，所求均是**人为构造**出来的，三大方法掌握到位，**把握好切入点**

## 章节概述

1. 不定积分与定积分关系：
关联性极其弱，仅在牛顿-莱布尼茨公式中有关联
2. 不定积分理论薄，极考计算;
**不定积分核心在于凑基本积分公式的形式，不同解法间不甚相通**

## 不定积分书写规范

$$\int f(x)dx=F(x)+C（C为任意常数）$$

## 原函数与不定积分的定义

$$如果在{\color{blue}区间I}上，可导函数F(x)的导函数为f(x)，即对任一x\in I，都有F'(x)=f(x)\\
则称F(x)为f(x)在区间I上的原函数,
称\int f(x)dx=F(x)+C为f(x)在区间I上的不定积分$$
$$注：定义区间\neq定义域，定义区间为一个区间，仅是定义域的子集\\
求原函数的过程应以不改变f(x)定义区间为前提（原函数之间应只差常数）\\
1. 三角函数变形（非恒等变形）可能会对间断点产生影响，姑且不计\\
2. \ln|x|去绝对值号：在不改变函数定义域的情况下，直接去掉
$$

## 原函数存在定理

$$f(x)在区间I上连续，则存在可导函数F(x),使对任一\ x\in I,都有F'(x)=f(x)\\
（区间I可开可闭）$$
$$
f(x)在区间I内均有定义，则\\
\left\{
\begin{array}{ll}存在可去间断点、跳跃间断点、无穷间断点必无原函数{\color{blue}（导函数不可能出现此三种情况；假设存在反证）}\\
\\
存在振荡间断点可能有原函数
\end{array}
\right.\\
 \ \\
f(x)在区间I内存在{\color{blue}无定义点}，则区间I不存在原函数，可讨论各分段的原函数$$
$$注：\int\frac{1}{x}dx=\ln|x|+C即为原函数（定义区间上，区间一定是连续的）
$$

## 原函数的奇偶性、周期性

**前提：连续函数的原函数**

$$f(x)\quad 奇 \Longrightarrow \int f(x)dx \quad 偶\\
f(x)\quad 偶 \quad 且\quad F(0)=0 \Longrightarrow \int f(x)dx \quad奇\quad（唯一,且等于\int_0^xf(t)dt）\\
f(x)\quad T  \quad 且\quad  \int_0^Tf(x)dx=0 \Longleftrightarrow \int f(x)dx \quad T$$

## 基本积分公式
$$x^k (k\neq -1), \ \frac{1}{x}\qquad
e^x, \ a^x(a>0\ 且\ a\neq1)\qquad
\ln x,\log_ax\qquad
\sin x,\cos x\qquad
\tan x,\cot x\\

\sec x(\frac{1}{\cos x}),\csc x(\frac{1}{\sin x})\qquad
\sec^2x,\csc^2x\qquad
\sec x\tan x,\csc x\cot x\\

\frac{1}{1+x^2},\ \frac{1}{a^2+x^2},\ \frac{1}{x^{2}-a^{2}} ,\ \frac{1}{a^{2}-x^{2}}\qquad
\frac{1}{\sqrt{1-x^2}},\ \frac{1}{\sqrt{a^2-x^2}},\
\frac{1}{\sqrt{x^2+a^2}},\ \frac{1}{\sqrt{x^2-a^2}}\qquad
{\color{blue}\sqrt{x^2+a^2}},{\color{blue}\sqrt{x^2-a^2}},
{\color{blue}\sqrt{a^2-x^2}}
$$

$$\begin{array}{ll}
\int x^{k} \mathrm{~d} x=\frac{1}{k+1} x^{k+1}+C (k \neq-1); & \int \frac{1}{x} \mathrm{~d} x=\ln|x|+C \\
\\
\int \mathrm{e}^{x} \mathrm{~d} x=\mathrm{e}^{x}+C; & \int a^{x} \mathrm{~d} x=\frac{a^{x}}{\ln a}+C(a>0\ 且 \ a\neq 1) \\
\\
\int \ln x\ dx=x\ln x-x+C; & \int \log_ax\ dx=x\log_ax-\frac{x}{\ln a}+C\\
\\
\int \sin x \mathrm{~d} x=-\cos x+C;  & \int \cos x \mathrm{~d} x=\sin x+C \\
\\
\int \tan x \mathrm{~d} x=-\ln |\cos x|+C； & \int \cot x \mathrm{~d} x=\ln |\sin x|+C \\
\\
\int \frac{\mathrm{d} x}{\cos x}=\int \sec x \mathrm{~d} x=\ln |\sec x+\tan x|+C; & \int \frac{\mathrm{d} x}{\sin x}=\int \csc x \mathrm{~d} x=\ln |\csc x-\cot x|+C \\
\\
\int \sec ^{2} x \mathrm{~d} x=\tan x+C; & \int \csc ^{2} x \mathrm{~d} x=-\cot x+C \\
\\
\int \sec x \tan x \mathrm{~d} x=\sec x+C; & \int \csc x \cot x \mathrm{~d} x=-\csc x+C\\
\\
\hdashline\\
\int \frac{1}{1+x^{2}} \mathrm{~d} x=\arctan x+C; & \int \frac{1}{a^{2}+x^{2}} \mathrm{~d} x=\frac{1}{a} \arctan \frac{x}{a}+C(a>0)\\
\ \\
\int \frac{1}{x^{2}-a^{2}} \mathrm{~d} x=\frac{1}{2 a} \ln \left|\frac{x-a}{x+a}\right|+C; &\int \frac{1}{a^{2}-x^{2}} \mathrm{~d} x=\frac{1}{2 a} \ln \left|\frac{x+a}{x-a}\right|+C\\
\\
\hdashline\\
\int \frac{1}{\sqrt{1-x^{2}}} \mathrm{~d} x=\arcsin x+C; & \int \frac{1}{\sqrt{a^{2}-x^{2}}} \mathrm{~d} x=\arcsin \frac{x}{a}+C(a>0)\\
\\
\int \frac{1}{\sqrt{x^{2}+a^{2}}} \mathrm{~d} x=\ln \left(x+\sqrt{x^{2}+a^{2}}\right)+C; & \int \frac{1}{\sqrt{x^{2}-a^{2}}} \mathrm{~d} x=\ln \left|x+\sqrt{x^{2}-a^{2}}\right|+C(|x|>|a|)\\
\ \\
\hdashline\\

{\color{blue}\int \sqrt{x^2+a^2}dx=\frac{x}{2}\sqrt{x^2+a^2}+\frac{a^2}{2}\ln(x+\sqrt{x^2+a^2})+C}\\
\ \\
{\color{blue}\int \sqrt{x^2-a^2}dx=\frac{x}{2}\sqrt{x^2-a^2}+\frac{a^2}{2}\ln|x+\sqrt{x^2-a^2}|+C}\\
\ \\
{\color{blue}\int \sqrt{a^2-x^2}dx=\frac{x}{2}\sqrt{a^2-x^2}+\frac{a^2}{2}\arcsin\frac{x}{a}+C}
\end{array}$$

## 不定积分性质

$$\int [af(x)+bg(x)]dx=a\int f(x)dx+b\int g(x)dx $$
$$\bigg[\int f(x)dx\bigg]'=f(x) \quad \int f'(x)dx=f(x)+C,\quad \int d[f(x)]=f(x)+C\\
(公式已成，说明可导、存在原函数)  $$
$${\color{blue}\left(\int f(e^x)dx\right)'=f(e^x)}\quad
{\color{blue}\left(\int f'(e^x)dx\right)'=f'(e^x)}\quad
{\color{blue}\left(\int d[f(e^x)]\right)'=f(e^x)}$$

## 原函数性质

1. 原函数若存在，必为无穷个
2. 定义区间内，原函数必可导，故必连续

## 留数法(单根，重根)

$$单根：\frac{c_i}{s-p_i}$$
$$c_i=\lim\limits_{s\to p_i}[(s-p_i)F(s)] \\

$$
$$重根：\frac{c_m}{(s-p_1)^m},\frac{c_{m-1}}{(s-p_1)^{m-1}},\cdots$$
$$c_m=\lim\limits_{s\to p_1}[(s-p_1)^m F(s)] \\
c_{m-1}=\lim\limits_{s\to p_1}\frac{\mathrm{d}}{\mathrm{d}s}[(s-p_1)^{m} F(s)]\frac{1}{1!}  \\
c_{m-2}=\lim\limits_{s\to p_1}\frac{\mathrm{d^2}}{\mathrm{d}s^2}[(s-p_1)^{m} F(s)]\frac{1}{2!}  \\

$$

## 万能公式

$$\sin x,\cos x,\tan x,\ dx$$

$$u=\tan\frac{x}{2}, 即\sin x=\frac{2u}{1+u^2}, \cos x=\frac{1-u^2}{1+u^2},\tan x=\frac{2u}{1-u^2},dx=\frac{2}{1+u^2}du$$
$$\int R(\sin x,\cos x)dx =\int R(\frac{2u}{1+u^2},\frac{1-u^2}{1+u^2})\frac{2}{1+u^2}du$$

## 三角函数 n 次方的积分

$$\int \sin^nx dx与\int \cos^nx dx;\quad \int \sec^nxdx与\int \csc^nxdx;\quad \int \tan^nxdx 与\int \cot^nxdx$$

$$\int \sin^nx dx与\int \cos^nx dx\\
\left\{
\begin{array}{l}
\int \sin^{2k+1}x dx=-\int (1-\cos^2x)^k d(\cos x)......\\
\\
\int \sin^{2k}x dx=\int (\frac{1-\cos2x}{2})^k dx......\\
或I=-\int\sin^{2k-1}xd(\cos x)=-[\cos x\sin^{2k-1}-(2k-1)\int\cos^2x\sin^{2k-2}xdx]=-[\cos x\sin^{2k-1}-(2k-1)(\int\sin^{2k-2}xdx-I)]\\
\\
\int \cos^nx dx同理
\end{array}
\right.$$
$$\int \sec^nxdx与\int \csc^nxdx\\

\left\{
\begin{array}{l}
\int \sec^{2k}xdx=\int (\tan^2+1)^{k-1}d(\tan x)\ \overset{t=\tan x}{\xlongequal{\quad\quad\quad}}\int (t^2+1)^kdt\\
\\
I=\int \sec^{2k+1}xdx=\int \sec^{2k-1}xd(\tan x)=\tan x\sec^{2k-1}x-(2k-1)I +(2k-1)\int \sec^{2k-1}xdx\\
\\
\int \csc^nxdx同理
\end{array}
\right.$$
$$\int \tan^nxdx 与\int \cot^nxdx
\left\{
\begin{array}{l}
\int \tan^{n}x dx=\int \tan^{n-2}(\sec^2x-1)dx=\int \tan^{n-2}d(\tan x)-\int \tan^{n-2}dx......\\
\\
\int \cot^nx dx同理
\end{array}
\right.$$

## 无法不定积分的函数（有原函数，但无法用初等函数表达）

$$\int c\ e^{(ax+b)^{2}} d x,\int\frac{e^x}{x}dx;\ \int \frac{\sin x}{x} d x; \ \int \frac{\cos x}{x} d x\\
\ \\
\int\frac{1}{\ln x}dx,\int\frac{x^n}{\ln x}dx(n\neq1);\int\sin x^2dx,\int\cos x^2dx$$
$$注：不可积分的函数很多$$

## 凑微分法

**凑微分方法是不定积分的底层方法**
$$
形式无突破口：考虑“消去”，“整理”\\
加减凑、乘除凑、倍角公式凑，拆分凑等等

$$
$$注：\int\frac{\Delta'}{\Delta}dx:\ln|\Delta|$$

## 不定积分的第一类换元

$$\int f[x,\varphi(x)]d[\varphi(x)]\xlongequal{t=\varphi(x)}\int f[\varphi^{-1}(t),t]dt\\
若为f[x,\varphi(x)]情形，t=\varphi(x)需反解\\
若为f[\varphi(x)]情形，t=\varphi(x)无需反解$$

## 不定积分的第二类换元

$$\int f(x)dx\xlongequal{x=\varphi(t)}\int f[\varphi(t)]\varphi'(t)dt\\
x=\varphi(t)需单调，计算完谨记t=\varphi^{-1}(x)回代$$
$$注：t取值范围，值域对应，单调区间（不定积分换元法需反解）\\
\int \frac{1}{(x^2-1)^2}dx\xlongequal{x=\sec t，t\in()}\int\frac{1}{\tan^4 t}\sec t\tan tdt\qquad  \times （值域无法对应）\\
严格意义上来讲，要求值域对应，单调区间对应，但考研考查不至如此$$

## 有理分式的裂项
假分式、真分式及裂项通式

$$假分式：直接用长除法化简（简便）$$
$$真分式：\\
1.分母寻找因式:试根法（阶数不会很高）\\
若分母无法分解为一次、二次实因式，则另寻他法（偏题，极少数）\\

2.裂项求分子：一阶因式裂项用“留数法”\\
           一阶、二阶因式组合，用“待定系数法”结合“留数法”\\

\frac{P(x)}{(x-a)(x^2+bx+c)(dx^5+ex^2)}=\frac{A}{x-a}+\frac{Bx+C}{x^2+bx+c}+\frac{Dx^4+Ex^3+Fx^2+Gx+H}{dx^5+ex^2}\\
\ \\
分子通式总比分母低一阶$$
$$注：同根放同式，否则通分后分子必捆绑其式\\
\frac{1}{(x-1)(x^2-1)}\rightarrow\frac{A}{x-1}+\frac{Bx+C}{x^2-1}=\frac{(x-1)......}{(x-1)(x^2-1)} \quad \times\\
化简为最简形式，再进行后续积分$$

## 有理分式的分解原则及计算

$$一次单因式：\frac{A}{ax+b}$$
$$k重一次因式：\frac{A_1}{ax+b}+\frac{A_2}{(ax+b)^2}+\cdots+\frac{A_k}{(ax+b)^k}\\
注：留数法的标准形式$$
$$二次单因式:\frac{Ax+B}{px^2+qx+r}
\left\{\begin{array}{l}

\frac{A}{px^2+qx+r}: \frac{a}{(x+b)^2+c}\xrightarrow{t=x+b}\int\frac{a}{t^2+c}dt\\
\ \\
\frac{Ax+B}{px^2+qx+r}: \frac{\lambda(2px+q)}{px^2+qx+r}+\frac{\mu}{{px^2+qx+r}}

\end{array}\right.$$
$$k重二次因式：\frac{A_1x+B_1}{px^2+qx+r}+\frac{A_2x+B_2}{(px^2+qx+r)^2}+\cdots+\frac{A_kx+B_k}{(px^2+qx+r)^k}\\
注：考研阶数不高，试凑即可出来$$
$$\left\{\begin{array}{l}
\frac{A}{(px^2+qx+r)^k}:\frac{A}{[(x+b)^2\pm c^2]^k}\xrightarrow {t=x+b}\int\frac{A}{(t^2\pm c^2)^k}dt(c>0)
\xlongequal["-"\quad 一次因式情形]{"+"\quad t=c\tan u,u\in(-\frac{\pi}{2},\frac{\pi}{2})}

\int\frac{A}{c^{2k-1}(\sec u)^{2k-2}}du=\int \frac{A}{c^{2k-1}}\cos^{2k-2}udu\\

\frac{Ax+B}{(px^2+qx+r)^k}=\frac{\lambda(2px+q)}{(px^2+qx+r)^k}+\frac{\mu}{(px^2+qx+r)^k}
\end{array}\right.$$

## 含根式的积分
三角代换、无理代换

**三角代换（内代换，注意限定单调区间）：**
$$\sqrt{x^2\pm a^2},\ \sqrt{a^2\pm x^2},\sqrt{2x-x^2}\\
x=\varphi(t) ，且单调\\
三角函数回代需画“三角”\\
\ \\
注：\sqrt{x^2-a^2}\left\{\begin{array}{lll}
x\in[a,+\infty),& x=a\sec t, &t\in[0,\frac{\pi}{2})\\
x\in(-\infty,-a],& x=-a\sec t, &t\in(-\frac{\pi}{2},0]
\end{array}\right.$$
**无理代换（整体代换）：**
$$简单根式：整体代换(\sqrt{1+x},\sqrt{1+\frac{1}{x}})$$

## 乘、除、简单复合的积分

**使用分部积分法**
$$参考选择顺序（例）：\arcsin x,\ln x,x^k,\sin x,e^x$$
$$注：中途勿切换函数\\
无从下手时首先考虑分部积分（破解形式）$$
$$典例：I=\int \sin(\ln x)dx=x\sin(\ln x)-\int \cos(\ln x)dx=x\sin(\ln x)-[x\cos(\ln x)+\underbrace{\int \sin(\ln x)dx}_{I}]

$$

## 三角函数的不定积分

换元法、化简整理、万能公式

**换元法：利用反三角导数**
$$\int \frac{1}{\sqrt{\sin x}\cdot \cos x}dx(t=\sqrt{\sin x})$$
$$\int\frac{1}{1+2\tan x}dx(t=\tan x)$$
**化简整理：**
$$化简分母，善用倍角公式、半角公式、辅助角公式等\\

\begin{array}{ll}
\left\{
\begin{array}{l}
\sin^2x+\cos^2x=1\\
\sin2x=2\sin x\ \cos x,\\ \cos2x=2\cos^2x-1=1-2\sin^2x\\
\sin^2x=\frac{1-\cos2x}{2},
\cos^2x=\frac{\cos2x+1}{2}\\
\sin x+\cos x=\sqrt{2}\sin(x+\frac{\pi}{4})\\
\end{array}
\right.
&
\left\{
\begin{array}{}
1+\tan^2x=\sec^2x\\
1+\cot^2x=\csc^2x\\
\end{array}
\right.
\end{array}

$$
**万能公式（一般较繁琐）：**......

## 循环复现分部积分公式

**指数函数与sinx、cosx相乘**

$$\int e^{ax}\sin bx\ dx=\frac{\left|\begin{array}{cc}(e^{ax})'& (\sin bx)'\\
\\
e^{ax}&\sin bx\end{array}\right|}{a^2+b^2}+C$$

## 分部积分表格法

$$\begin{array}{c|c|c|c|c|}
\hline
u的各阶导数& u & u' & u'' & \cdots & \begin{array}{lr}u^{(n+1)}\\&(-1)^{n+1}\end{array}\\
\hline
v的各阶原函数 & v& v^{(-1)}& v^{(-2)}&\cdots&v^{(-n-1)}\\
\hline
\end{array}
$$
$$右下斜对角逐个相乘（任意位置停均可）：\\
(-1)^0\cdot uv^{(-1)}+(-1)^1\cdot u'v^{(-2)}+\cdots+(-1)^n\cdot u^{(n)}v^{(-n-1)}+ (-1)^{n+1} \int u^{(n+1)}v^{(-n-1)}dx\\
若u为n阶多项式，(-1)^{n+1} \int u^{(n+1)}v^{(-n-1)}dx=0，且之后各项均为0$$

## 不定积分重要经验

$$选择题，直接选项求导（稳定）$$

## 分段函数求原函数

1. 各区间分开求
2. 原函数在分段点处连续，解C1,C2关系

## 不定积分“变量对应”题型
复合函数、积分变量对应

**复合函数：]
$$f(\ln x)=\frac{\ln(1+x)}{x},求\int f(x)dx（令x=\ln t,参考前式变量代换即可）$$
$$其余求解类型，解f(x)即可$$
**积分变量对应：]
$$\quad\int f(x)dx=\frac{\sin x}{x}+C\\
\Rightarrow \int f(ax)dx=\int \frac{f(ax)}{a}d(ax)=\frac{\sin(ax)}{a^2x}+C$$

## 不定积分特殊计算方法（抵消型）

$$\quad\int \frac{xe^x}{(1+x)^2}dx=\int \frac{(1+x-1)e^x}{(1+x)^2}dx\\=
\int \frac{e^x}{1+x}dx-\int \frac{e^x}{(1+x)^2}dx\\=
\int\frac{1}{1+x}d(e^x)-\int \frac{e^x}{(1+x)^2}dx\\
=\frac{e^x}{1+x}+\int\frac{e^x}{(1+x)^2}dx-\int \frac{e^x}{(1+x)^2}dx\\
=\frac{e^x}{1+x}$$
$$注：此题\frac{1}{(1+x)^2}分部积分更简便$$

## $\int \frac{1}{1+x^4}dx$

$$\int \frac{1}{1+x^4}dx = \frac{1}{2}\int \frac{(1+x^2)+(1-x^2)}{1+x^4}$$
$$\begin{array}{llll}
&\int \frac{1+x^2}{1+x^4}dx  &&\int \frac{1-x^2}{1+x^4}dx \\
\\
=& \int \frac{\frac{1}{x^2}+1}{\frac{1}{x^2}+x^2}dx &=&\int \frac{\frac{1}{x^2}-1}{\frac{1}{x^2}+x^2}dx\\
\\
=& -\int \frac{1}{(\frac{1}{x}-x)^2+2}d(\frac{1}{x}-x)&=&-\int \frac{1}{(\frac{1}{x}+x)^2-2}d(\frac{1}{x}+x)\\
\\
=& ......&=&......

\end{array}$$

## 不定积分典例

**灵活理解推广**
$$\frac{\cos x}{\sin x+\cos x}
\rightarrow

\left\{\begin{array}{l}
法一：\frac{\cos x(\cos x-\sin x)}{(\cos x+\sin x)(\cos x-\sin x)}=\frac{\cos^2 x-\sin x\cos x}{\cos^2x-\sin^2x}\\
\ \\
法二：\frac{A(\cos x+\sin x)+B(\cos +\sin x)'}{\sin x+\cos x}

\end{array}\right.$$

# 定积分

## 考情分析

1. 分为两个体系：固有定积分代入（重点）、牛莱体系求原函数

已知积分，构造求积分

## 积分定义式
一般区间、(0,1)区间

$$\lim\limits_{n\to \infty}\sum_{i=1}^{n}f[a+\frac{(b-a)i}{n}]\frac{b-a}{n}=\int_a^b f(x)dx\\

$$
$$\left\{
\begin{array}{l}a+\frac{(b-a)i}{n}\rightarrow x（范围同样）\\
\\
\frac{b-a}{n}\rightarrow dx
\end{array}
\right.$$
$$\lim\limits_{n\to \infty}\sum_{i=1}^{n}f(\frac{i}{n})\cdot\frac{1}{n}=\int_0^1f(x)dx\\

$$
$$\left\{
\begin{array}{l}\frac{i}{n}\rightarrow x（范围同样）\\
\\
\frac{1}{n}\rightarrow dx
\end{array}
\right.$$

## 定积分存在的充分条件

$$f(x)在[a,b]上连续（即有界），则\int_a^bf(x)dx存在\\
f(x)在[a,b]上单调（即有界），则\int_a^bf(x)dx存在\\
f(x)在[a,b]上有界，且只有有限个间断点，则\int_a^bf(x)dx存在$$

## 定积分重要细节

$$f(x)有界，\int_{a^-}^af(x)dx=0\\
瑕点在一点的积分值难以分析
$$

## 常用积分值记忆

一个拱，半个拱

$$\int_0^{\pi}\sin x\ dx=2（一个拱），
\int_0^{\frac{\pi}{2}}\sin x\ dx=1（半个拱）\\
\ \\
\int_0^{\pi}|\sin kx|dx=2\\
\ \\
\int_0^1 \arcsin x\ dx=\frac{\pi}{2}-\int_0^{\frac{\pi}{2}}\sin x\ dx=\frac{\pi}{2}-1$$

## 定积分估值定理

$$m(b-a)\leqslant\int_a^bf(x)dx\leqslant M(b-a)$$

## 积分中值又称函数均值

## 定积分的性质

**函数、区间的线性叠加性**
$$\int_a^b[\alpha f(x)+\beta g(x)]=\alpha\int_a^bf(x)dx+\beta\int_a^bg(x)dx$$
$$\int_a^bf(x)dx=\int_a^cf(x)dx+\int_c^bf(x)dx（c为任意常数）$$

## 定积分不等式

$$\int_a^bf(x)dx\leqslant \bigg|\int_a^bf(x)dx\bigg|\leqslant\int_a^b|f(x)|dx
$$
$$注意(a<b)$$

## 华里士公式

$$\int_0^\frac{\pi}{2}\sin^nx\ dx=\int_0^\frac{\pi}{2}\cos^nx\ dx=
\left\{
\begin{array}{l}
\frac{n-1}{n}\cdot \frac{n-3}{n-2}\cdots \frac{2}{3}\cdot 1，\quad n为奇(n\geqslant3)\\
\\
\frac{n-1}{n}\cdot\frac{n-3}{n-2}\cdots \frac{1}{2}\cdot \frac{\pi}{2}，\quad n为偶(n\geqslant2)
\end{array}
\right.$$

## 对称区间定积分

**与轮换对称性本质相同**
$$\int_{-a}^af(x)dx\xlongequal{函数处理}\frac{1}{2}\int_{-a}^af(x)+f(-x)dx\xlongequal{区间处理}\int_0^af(x)+f(-x)dx$$
$$奇零偶倍：
\int_{-a}^{a}f(x)dx\xlongequal{f(x)\  奇}0\qquad \int_{-a}^{a}f(x)dx\xlongequal{f(x)\  偶}2\int_{0}^{a}f(x)dx$$

## 对称函数定积分
$$f(x)关于x=I对称\\
f(x)关于(a,0)对称$$

**与复合函数奇偶性同理，“内偶则偶，内奇同外”**
$$
\int_{c-a}^{c+a}g[f(x)]dx=
\left\{
\begin{array}{cl}
0,&g(x)关于(c,0)对称\\
\\
2\int_c^{c+a}g[f(x)]dx,&g(x)关于x=c对称

\end{array}
\right.$$
$$记:
\int_0^{\pi}f(\sin x)dx=2\int_0^{\frac{\pi}{2}}f(\sin x)dx$$

## 同“形”内函数的定积分

$$g(x)与h(x)在[a,b]上有相同的形状（形状可打乱）,有\\
\int_a^b f[g(x)]dx=\int_a^bf[h(x)]dx（相当于线性组合）
$$
$$记:\\
\quad\int_0^{2\pi}f(|\sin x|)dx=\int_0^{2\pi}f(|\cos x |)dx\\
=4\int_0^\frac{\pi}{2}f(\sin x)dx=4\int_0^\frac{\pi}{2}f(\cos x)dx\\
\ \\
\quad\int_0^\pi f(\sin x)dx=2\int_0^\frac{\pi}{2} f(\sin x)dx\\
\quad\int_0^\pi f(|\cos x|)dx=2\int_0^\frac{\pi}{2} f(\cos x)dx
$$

## 区间再现公式

$$\int_a^bf(x)dx=\int_a^bf(a+b-x)dx$$
$$记：\\
\int_0^{\pi}xf(\sin x)dx=\frac{\pi}{2}\int_0^{\pi}f(\sin x)dx=\pi\int_0^{\frac{\pi}{2}}f(\sin x)dx\\
纯(\sin x,\cos x)组成的函数,\sin x与\cos x互换：\\
\int_0^\frac{\pi}{2}\frac{\sin x}{\sin x+\cos x}dx=\int_0^\frac{\pi}{2}\frac{\cos x}{\cos x+\sin x}dx$$

## 牛顿-莱布尼茨公式

$$f(x)在[a,b]上可积且存在原函数，则\int_a^bf(x)dx=F(b)-F(a)$$
$$注：若所求“原函数”含无定义点，不可视作此区间的原函数\\
故不可用牛顿-莱布尼茨公式计算定积分$$

## 定积分的换元积分法

$$\left\{
\begin{array}{l}
f(x)在[a,b]上连续 \\
\\
\varphi(\alpha)=a, \varphi(\beta)=b \\
\\
x=\varphi(t)在[\alpha,\beta] 或 [\beta, \alpha]上连续（上下限对应即可，R_{\varphi}无须等于[a,b]）
\end{array}

\right.$$
$$\int_a^bf(x)dx=\int_{\alpha}^{\beta}f[\varphi(t)]\varphi'(t)dt$$
$$注：定积分换元无需反解，故无需单调$$

## 定积分的分部积分法

$$u'(x), v'(x)在[a,b]上连续$$
$$\int^b_au(x)v'(x)dx=u(x)v(x)\bigg|^b_a-\int_a^bv(x)u'(x)dx$$

## 不定积分、定积分、变限积分的关系

$$变限积分本质上为定积分$$
$$f(x)连续时：三者统一，\int_a^xf(t)dt\ 即为一个原函数
\\
f(x)不连续：各成体系

$$

## 牛顿-莱布尼茨公式求定积分

$$分段连续，分段求，\\\int_a^bf(x)dx=\int_{a^+}^bf(x)dx=F(x)\bigg|_{a^+}^b$$
$$注：多段极限不存在书写规范\lim\limits_{b\to +\infty}[\frac{b}{1+e^{-b}}-\ln(e^b+1)]$$

## 定积分重要经验

1. 灵活利用“图像、面积”计算定积分
2. 条件允许下，将积分区间尽量往对称区间凑

## 特殊积分函数处理技巧

$$\begin{array}{rl}

u(x,y)=&\int_0^tf(t)|xy-t|dt\\
=& \int_0^{xy}f(t)(xy-t)dt+\int_{xy}^tf(t)(t-xy)dt

\end{array}$$

## 定积分比较大小问题

$$同一区间的定积分（一般不必计算，比较被积函数即可）：\\
典例：I_1=\int_0^1\frac{x}{2(1+\cos x)}dx,\quad
I_1=\int_0^1\frac{\ln(1+x)}{(1+\cos x)dx},\quad
I_1=\int_0^1\frac{2x}{(1+\sin x)}dx\\
\frac{x}{2}<\ln(1+x)\rightarrow I_1<I_2\qquad
\frac{\ln(1+x)}{1+\cos x}<
\frac{x}{1+\cos x}
<\frac{2x}{1+\sin x}\rightarrow I_2<I_3$$

## 综合题型

$$微分方程：f(t)=e^{4\pi t^2}+2\pi \int_0^{2t}f(\frac{1}{2}r)dr（变限积分函数）\\

积分求解：f(x)=\sqrt{1-x^2}+e^x\int_a^b f(x)dx（积分为数）$$

# 变限积分函数

## 变限积分函数的连续性、可导性
$$\Phi(x)=\int_0^xf(x)dx$$

$$1. f(x)在[a,b]可积，\Phi(x)在[a,b]上连续\\
2. f(x)在[a,b]连续，\Phi(x)在[a,b]上可导\\
3. f(x)在[a,b]可导，\Phi(x)在[a,b]上k+1阶可导$$

## 变限积分函数在间断点的可导性
$$\Phi(x)=\int_a^xf(t)dt$$

$$若x_0是f(x)的可去间断点，则\Phi(x)在x_0处可导，且\\F'(x_0)=\lim\limits_{x\to x_0}f(x)$$
$$若x_0是f(x)的跳跃间断点，则\Phi(x)在x_0处连续，但不可导,且\\
F_-'(x_0)=\lim\limits_{x\to x_0^-}f(x),F_+'(x_0)=\lim\limits_{x\to x_0^+}f(x)\\
$$
$$注：可由洛必达证得$$

## 变限积分函数的奇偶性、周期性

**前提：f(x)可积**
$$f(x)\ \ \ 奇 \Longrightarrow \int_a^xf(t)dt=\int_0^xf(t)dt-\int_0^af(t)dt \quad  偶$$
$$f(x)\ \ \ 偶
\left\{
\begin{array}{l}
\Rightarrow\int_0^xf(t)dt\quad 奇\\
\\
\int_0^af(x)dx=0 \Rightarrow \int_a^xf(t)dt=\int_0^xf(t)dt\Rightarrow\int_a^xf(t)dt \quad奇\\
\end{array}
\right.$$
$$f(x)\ \ T  \quad 且 \quad \int_0^T f(x)dx=0 \Longleftrightarrow \int_0^x f(t)dt \ \ \ \ T$$

## 变限积分“被积函数含积分上限”情形
加减型、复合型

**加减型：**
$$\int_a^x(x-t)f(t)dt=x\int_a^xf(t)dt-\int_a^xtf(t)dt$$
**复合型：**
$$\int_0^xtf(x^2-t^2)dt,令u=x^2-t^2,得\frac{1}{2}\int_0^{x^2}f(u)du$$
$$\int_0^3x\sqrt{9-x^2t^2}\ dt \ \ \ 令u=xt, 得 \int_0^{3x}\sqrt{9-u^2}du\\
（注意\frac{1}{x}情形，需分类讨论）$$
$$注：F(x)=\int_a^xf(x)+g(u)du\\
F'(x)=[f(x)(x-a)]'+g(x)\neq f(x)+g(x)$$

## 积分与函数比较大小

$$\int_{\frac{1}{x}}^1f(t)dt与g(x)(1-\frac{1}{x})\\
\begin{array}{ll}
\int_{\frac{1}{x}}^1f(t)dt &\rightarrow f(\xi)(1-\frac{1}{x})\\
g(x)(1-\frac{1}{x})& \rightarrow \int_{\frac{1}{x}}^1g(x)dt
\end{array}$$

## 小技巧

$$巧用\int_a^x f(t)dt表示f(x)的原函数$$

# 反常积分

## 考情分析

反常积分审敛两大方法：比较判别法（一般用于证明题）、比较判别法的极限形式

## 定积分与反常积分区别

定积分：区间有限（闭区间），函数有界，又称黎曼积分（黎曼关于定积分的理论存在不完备的缺陷）
反常积分：区间无限，或函数无界，又称广义积分

## 反常积分的敛散性

**同一函数积分在不同区间的敛散性，函数不同另行讨论：**
$$需分开计算，但趋向速度可能不一致\\
\int_{-1}^{1}\frac{1}{x}dx=\lim\limits_{x\to 0^-}\int_{-1}^x\frac{1}{x}dx+\lim\limits_{x\to 0^+}\int_{x}^{1}\frac{1}{x}dx\\
\int_{-\infty}^{\infty}\frac{1}{x}dx=\lim\limits_{x\to -\infty}\int_{x}^af(x)dx+\lim\limits_{x\to+\infty}\int_{a}^{x}f(x)dx\\
$$
$$子区间:\\收敛+收敛=收敛\\
收敛+发散=发散\\
发散+发散= 发散\\
$$
**反常积分任意子区间积分发散，称反常积分发散**
**发散的反常积分一定存在**
$$\int_{-1}^{1}\frac{1}{x}\neq0\ 不收敛$$

## 反常积分分析思路

$$反常积分敛散与否关键在于反常积分在趋于\\
\left\{
\begin{array}{ll}
\infty\\
\\
瑕点
\end{array}
\right.
时的“表现”\\
故有，反常积分判别尺度$$

## 反常积分判别尺度

$$p \ \nearrow \quad (\frac{1}{x})^p绕(1,1)顺时针旋转\\
$$
$$\int_0^1(\frac{1}{x})^p\ dx\quad
\left\{
\begin{array}{cl}
0<p<1，& 收敛\\
&&（\infty^p阶次越低越收敛）\\
p\geqslant1，& 发散
\end{array}
\right.$$
$$\int_1^{+\infty}(\frac{1}{x})^p\ dx\quad
\left\{
\begin{array}{cl}
p>1，& 收敛\\
&&（0^p阶次越高越收敛）\\
p\leqslant1，& 发散
\end{array}
\right.$$

## 比较判别法的极限形式

**反常积分审敛的核心方法**
$$无穷处：\\
\lim\limits_{x\to +\infty}\frac{f(x)}{(\frac{1}{x})^p}=A\neq0，则\int_a^{+\infty}f(x)dx与\int_a^{+\infty}(\frac{1}{x})^p同敛散\\
\ \\
\lim\limits_{x\to +\infty}\frac{f(x)}{(\frac{1}{x})^p}=\infty,且p\leqslant1,则发散
\\
\ \\
\lim\limits_{x\to +\infty}\frac{f(x)}{(\frac{1}{x})^p}=0,且p>1,则收敛$$
$$瑕点：\\
\lim\limits_{x\to x_0}\frac{f(x)}{(\frac{1}{x-x_0})^p}=A\neq0，则\int_a^{+\infty}f(x)dx与\int_a^{+\infty}(\frac{1}{x})^p同敛散\\
\ \\
\lim\limits_{x\to x_0}\frac{f(x)}{(\frac{1}{x-x_0})^p}=\infty,且p\geqslant1,则发散\\
 \ \\
\lim\limits_{x\to x_0}\frac{f(x)}{(\frac{1}{x-x_0})^p}=0,且p<1,则收敛$$
$$注：
均与(\frac{1}{x})^p作比$$

## 常用反常积分
$$\int_a^{+\infty}\frac{1}{x\ln^px}dx,\ \int_a^{+\infty}x^ke^{-\lambda x}dx$$

$$\int_a^{+\infty}\frac{1}{x\ln^px}dx=\int_a^{+\infty}\frac{1}{\ln^px}d(\ln x)
\left\{
\begin{array}{lll}
收敛，&p>1\\
&&a>1\\
发散，&p\leqslant1
\end{array}
\right.
$$
$$注：\\
\lim\limits_{x\to +\infty}\frac{1}{x}\frac{1}{\ln^px}\to 0无具体阶次，且与1的关系无法判断\\
\ \\
\lim\limits_{x\to +\infty}\frac{1}{x^k}\frac{1}{\ln^px}(k\neq1)\to 0无具体阶次，但与1的关系可判断$$
$$\\ \int_a^{+\infty}x^ke^{-\lambda x}dx
\left\{
\begin{array}{lll}
收敛，&\lambda>0\\
&&k\geqslant0\\
发散, &\lambda<0
\end{array}
\right.$$

## 判别尺度使用规范过程

$$无穷区间(x\to \infty)\\
利用判别尺度分析\lim\limits_{x\to \infty}f(x)\to 0的阶次p，再用同阶(\frac{1}{x})^p作比,\lim\limits_{x\to \infty}\frac{f(x)}{(\frac{1}{x})^p}=a（同敛散）$$
$$瑕积分(x\to x_0)\\
利用判别尺度分析\lim\limits_{x\to x_0}f(x)\to \infty的阶次p，再用同阶(\frac{1}{x})^p作比, \lim\limits_{x\to x_0}\frac{f(x)}{(\frac{1}{x})^p}=a（同敛散）$$
$$无具体阶次,找“大阶”或“小阶”作比$$

## 特殊函数阶次

$$\lim\limits_{x\to +\infty},\lim\limits_{x\to -\infty}\left\{
\begin{array}{ll}
e^x, &阶数为“正无穷”\\
\frac{1}{e^x},&阶数为“正无穷”
\end{array}
\right.\quad
\left\{\begin{array}{l}
\lim\limits_{x\to +\infty}\frac{x^k}{e^x}=0\quad \lim\limits_{x\to -\infty}\frac{(\frac{1}{x})^k}{e^x}=\infty\\

\lim\limits_{x\to +\infty}\frac{(\frac{1}{x})^k}{\frac{1}{e^x}}=\infty\quad \lim\limits_{x\to -\infty}\frac{x^k}{\frac{1}{e^x}}=0
\end{array}\right.$$
$$\lim\limits_{x\to 0},\lim\limits_{x\to +\infty}
\left\{
\begin{array}{ll}
\ln x^k,\ln^kx, &阶数为“无穷小”\\
\frac{1}{\ln x^k},\frac{1}{\ln^kx},&阶数为“无穷小”
\end{array}
\right.\quad \cdots$$

## $\Gamma$函数\\
\Gamma(\alpha)=\int_0^{+\infty}x^{\alpha-1}e^{-x}dx(\alpha>0)$$

$$\Gamma(\alpha+1)=\alpha\Gamma(\alpha)\\
\Gamma(n+1)=n!\quad
\Gamma(\frac{1}{2})=\sqrt{\pi}\quad
\Gamma(1)=1$$
$$例：\\
\int_0^{+\infty}x^3e^{-x}dx=\int_0^{+\infty}x^{4-1}e^{-x}dx=\Gamma(4)=3!$$

## $I=\int_0^{+\infty}e^{-x^2}dx$

$$I=\int_0^{+\infty}e^{-x^2}dx\\
I^2=\int_0^{+\infty}e^{-x^2}dx\int_0^{+\infty}e^{-y^2}dy\\
=\iint\limits_{D} e^{-r^2}rdrd\theta\\
=\frac{1}{2}\int_0^{\frac{\pi}{2}}d\theta\int_0^{+\infty}e^{-r^2}d(r^2)=\frac{\pi}{4}
$$
$$故I=\frac{\sqrt{\pi}}{2}$$

# 一元积分学的应用

## 考情分析

旋转体只考沿坐标轴旋转

## 旋转体几何计算公式

**两类旋转体体积：**
$$饼状微元：V=\int_a^b\pi[f(x)]^2dx\\
桶状微元：
V=\int_a^b2\pi |x|\cdot |f(x)|dx$$
**旋转体侧面积：**
$$饼状微元：S=\int_a^b 2\pi |f(x)|\cdot\sqrt{1+f'^2(x)}dx$$

## 物理量计算公式

$$压力微元：\rho gxdS（x为水深）\\
抽水做功微元：\rho gxdV（x为提升高度）$$
$$注：旋转体灵活转换坐标系简化计算\\
灵活运用物理意义（x 深度、高度等）

$$

# 多元微分

## 考情分析

1. 多元微分过于复杂，故考查内容很浅
2. 主考察二元，三元及以上难以理解
3. 隐函数存在定理理解即可

## 二元极限的定义

$$若二元函数f(x,y)在(x_0,y_0)的去心邻域内有定义，\\
且(x,y)以\ \textbf{任意方式}\ 趋向于(x_0,y_0)时，\\
f(x,y)均趋向于A，则\lim\limits_{(x,y)\to (0,0)}f(x,y)=A$$

## 多元函数的连续性

$$多元初等函数在其自然定义域上是连续的$$

## 二元极值定义
极大值，极小值

$$f(x,y)在U(x_0,y_0)内有定义，对于任意(x,y)\in \mathring{U}(x_0,y_0),\ \ \ f(x,y)<f(x_0,y_0)(或f(x,y)>f(x_0,y_0))，则\\称f(x_0,y_0)为极值
$$

## 二元可微的定义

$$设函数z=f(x,y)在点(x,y)的某邻域内有定义，如果函数在点(x,y)的全增量\\
\quad\quad\quad\quad\Delta z=f(x+\Delta x,y+\Delta y)-f(x,y)\\
可表示为\\
\quad\quad\quad\quad\quad\Delta z=A\Delta x+B\Delta y+\circ(\rho)（各增量均趋于0）\\
其中A和B不依赖于\Delta x和\Delta y，而仅与x和y有关，\rho=\sqrt{(\Delta x)^2+(\Delta y)^2},\\
则称z=f(x,y)在点(x,y)可微分
$$
$$A\Delta x+B\Delta y称为z=f(x,y)在点(x,y)的全微分,记作dz\\
即dz=Adx+Bdy\\
$$

## 多元微分的本质或几何理解

$$多元微分由一元微分定义，以一元导数的组合理解多元导数\\
可微\Leftrightarrow dz可由\frac{\partial z}{\partial x}dx+\frac{\partial z}{\partial y}dy表示$$

## 二元可微的必要条件

$$若函数z=(x,y)可微，则该函数在点(x,y)的偏导数\frac{\partial z}{\partial x},\frac{\partial z}{\partial y}必存在，\\
且dz=\frac{\partial z}{\partial x}dx+\frac{\partial z}{\partial y}dy（偏导虽是坐标轴方向，但(d x,d y)表示任意方式）$$

## 二元可微的判定

$$定义判定式（充要条件）：\lim\limits_{(x,y)\to (x_0,y_0)}\frac{\Delta z-A\Delta x-B\Delta y}{\sqrt{(x-x_0)^2+(y-y_0)^2}}=0\\
\lim\limits_{(x,y)\rightarrow(x_0,y_0)}\frac{f(x,y)-f(x_0,y_0)-f_x'(0,0)(x-x_0)-f_y'(0,0)(y-y_0)}{\sqrt{(x-x_0)^2+(y-y_0)^2}}=0$$
$$一阶偏导连续（充分条件）\\
一阶偏导存在（必要条件）$$
$$小结论（充分非必要）：\\
\lim\limits_{(x,y)\to (x_0,y_0)}\frac{\Delta z}{\rho}=0\Rightarrow\Delta z=\circ(\rho),即\underbrace{\Delta z=0\Delta x+0\Delta y+\circ(\rho)}_{定义式}\\

\lim\limits_{(x,y)\to (x_0,y_0)}\frac{f(x,y)-Ax-By+C}{\rho}=0 \Rightarrow\underbrace{\Delta z=A\Delta x+B\Delta y+\circ(\rho)}_{定义式}$$

## 二元微分注意点

$$“偏积分”+C(x)/C(y)$$
$$二阶偏导连续（则二阶混合偏导均连续），或\frac{\partial^2z}{\partial x\partial y}与\frac{\partial ^2z}{\partial y\partial x}连续，则\frac{\partial^2z}{\partial x\partial y}=\frac{\partial ^2z}{\partial y\partial x}$$

## 极值点、驻点、极值规范写法

$$极值点（驻点同理）：(x_0,y_0)$$
$$极值：f(x_0,y_0)$$

## 微分因变量可为0，微分自变量不可为0

$$函数z=z(x,y)\\
dz=0,dz\neq0\\
dx,dy\neq0$$

## 连续、可偏导及可微之间的关系图

**可微即曲面的光滑，但曲面的光滑相较曲线更为复杂，大致理解即可**

![](pic-advance-math\Markji_1751354341254.png)
$${\color{blue}在定义域内，可微\Rightarrow 连续}\\
一阶偏导连续（两个均连续）：一阶偏导仍是二元函数，其在某圆域内连续，即圆域内其一阶偏导相等$$

## $f'_x(x_0,y_0)$存在,$f'_y(x_0,y_0)$连续，则$f(x_0,y_0)$可微

$$向定义式靠近：\Delta z=A\Delta x+B\Delta y+\circ(\rho)\\
\Delta z= f(x_0+\Delta x,y_0+\Delta y)- f(x_0,y_0)\\
\quad \ \ \ =[f(x_0+\Delta x,y_0+\Delta y)-f(x_0+\Delta x,y_0)]+[f(x_0+\Delta x,y_0)-f(x_0,y_0)]\\
$$
$$\quad\quad f(x_0+\Delta x,y_0+\Delta y)-f(x_0+\Delta x,y_0)\\
\xRightarrow{拉格}f'(x_0+\Delta x,\xi)\Delta y\ \ (\xi\in(y_0+\Delta y,y_0))\\
\xlongequal{连续}f'(x_0,y_0)\Delta  y$$
$$\quad \ f'_x(x_0,y_0)=\lim\limits_{(x,y)\to (x_0,y_0)}\frac{f(x_0+\Delta x,y_0)-f(x_0,y_0)}{\Delta x}=A\\
\Rightarrow f(x_0+\Delta x,y_0)-f(x_0,y_0)=A\Delta x+\circ(\Delta x)$$
$$一阶偏导连续\Rightarrow 可微\quad （同理可证）$$

## 隐函数存在定理

$$设函数F(x,y)在P(x_0,y_0)的某一邻域内具有连续偏导数，F(x_0,y_0)=0,F'_y(x_0,y_0)\neq0,\\则方程F(x,y)=0在(x_0,y_0)的某一邻域内能唯一确定一个连续且具有连续导数的函数y=f(x),\\它满足条件y_0=f(x_0),并有\frac{dy}{dx}=-\frac{F'_x}{F'_y}$$

## 隐函数求导公式
二元，多元

$$二元：
\frac{dy}{dx}=-\frac{F'_x}{F'_y}（x,y为F的自变量，相互独立）$$
$$多元：
\frac{\partial z}{\partial x}=-\frac{F'_x}{F'_z},\ \ \frac{\partial z}{\partial y}=-\frac{F'_y}{F'_z}（x,y,z为F的自变量，相互独立）$$

## 求极值处理技巧

$$d=\sqrt{x^2+y^2},|x+y|\rightarrow 计算d^2\\
$$

## 无条件极值

**开区域求极值问题**
$$极值可疑点：\\
1. \left\{
\begin{array}{l}
f'_x(x,y)=0\\
f'_y(x,y)=0
\end{array}
\right.的点(x_0,y_0)\\
2. 偏导数不存在的点（极值的定义去判别）$$
$$\left\{
\begin{array}{}
f_x'(x_0,y_0)=0\\
\\
f_y'(x_0,y_0)=0
\end{array}
\right.\\

判断驻点是否极值：\left\{
\begin{array}{}
f_{xx}''(x_0,y_0)=A\\
\\
f_{xy}''(x_0,y_0)=B\\
\\
f_{yy}''(x_0,y_0)=C
\end{array}
\right.\quad\quad\Delta=AC-B^2
\left\{
\begin{array}{l}
>0 \Rightarrow 极值\left\{   \begin{array}{}
A<0 \Rightarrow 极大值 \\
A>0 \Rightarrow 极小值
\end{array}
\right. \\
\\
<0 \Rightarrow 非极值 \\
\\
=0  \Rightarrow失效

\end{array}

\right.$$

## 条件极值失效情形

$$取特殊路径，证明不存在\\
典例：f(x,y)=(y-x^2)(y-x^3)\\
驻点(0,0)\quad 取y_1=2x^2,y_2=2x^3\\
(x,y)\to (0,0)时
\left\{\begin{array}{l}
f(x,2x^2)=(2x^2-x^2)(2x^2-x^3)>0\\
f(x,2x^3)=(2x^3-x^2)(2x^3-x^3)<0
\end{array}\right.$$
$$
利用定义证明极值存在
$$

## 条件最值与拉格朗日乘数法
$$求u=f(x,y,z)在条件
\left\{
\begin{array}{l}
\varphi(x,y,z)=0\\
\\
\psi(x,y,z)=0
\end{array}
\right.
下的最值$$

**边界上求最值问题**
$$构造辅助函数F(x,y,z,\lambda,\mu)=f(x,y,z)+\lambda\varphi(x,y,z)+\mu\psi(x,y,z)$$
$$\left\{
\begin{array}{l}
F'_x=f'_x+\lambda\varphi'_x+\mu\psi'_x=0\\
\\
F'_y=f'_y+\lambda\varphi'_y+\mu\psi'_y=0\\
\\
F'_z=f'_z+\lambda\varphi'_z+\mu\psi'_z=0\\
\\
F'_\lambda=\varphi(x,y,z)=0\\
\\
f'_\mu=\psi(x,y,z)=0
\end{array}
\right.$$
$$解出可疑点P_i，取f(P_i)最值即可$$

## 二元极限存在判定

1. 直接计算
2. 找特殊路径证不存在
$$y=kx,y=kx^2$$

## 二元极限计算

**二元极限的可计算性是有限的**
**通常考无定义点、分段点处极限（初等多元函数在有定义点必连续）**
1. 利用一元求极限
（除洛必达与单调有界准则外，非零因子常数化、等价无穷小、泰勒展开等均可用）
$$\lim\limits_{(x,y)\to (0,0)}\frac{y\sin(xy)}{\ln(1+xy)}=\lim\limits_{(x,y)\to (0,0)}\frac{y\cdot xy}{xy}=0\\
$$
（二元函数单变量求极限，可用洛必达，另一变量视作常数）
$$\lim\limits_{x\to 0}\frac{2e^{x^2y}-e^x-e^{-x}}{x^2}\xlongequal{洛必达}\lim\limits_{x\to 0}\frac{4xye^{x^2y}-e^x+e^{-x}}{2x}=\cdots$$
2. 利用夹逼准则（放缩）
$$\lim\limits_{(x,y)\to (\infty,\infty)}\frac{x^2}{x^4+y^4}(0\leqslant\frac{x^2}{x^4+y^4}\leqslant\frac{1}{x^2})=0$$
3. 极坐标法（转换坐标系，新坐标系下或许能计算）
$$\lim\limits_{(x,y)\to(0,0)}f(x,y)=\lim\limits_{\rho\to0}f(\rho\cos\theta,\rho\sin\theta)（\rho,\theta均为自变量）$$

## 多元微分“单函数”求导

**显函数：**
$$寻找函数中以f(x,y)表达的部分\\
不含f(x,y)部分：\\
直接按求导习惯求导即可......\\
含f(x,y)部分：\\
1. 画出变量关系图\\
2. 链式求导法则计算
$$
**隐函数：**
$$隐函数求导法则（适用于一阶）
$$
$$注：若二阶混合偏导连续，注意合并二阶混合偏导$$

## 多元微分“多函数”求导

**导函数可能会“耦合”自变量、因变量**
**方程组型求导（通用方法）：**
$$1. 根据变量与方程组个数分析是“ \_\_”个“\_\_”元函数”\\
2. 画出变量关系图\\
3. 对方程组两边求导\\
4. 解方程......
$$
**显函数+隐函数：**
$$u=f(x,y,z),而\varphi(x^2,e^y,z)=0,y=\sin x,求\frac{du}{dx}\\
 \ \\
y=g(x,z),函数z=z(x,y)由方程f(x-z,xy)=0确定,求\frac{dy}{dx}\\
 视为y=g[x,z(x,y)]\\
\ \\
注意区别：
\left\{
\begin{array}{ll}
\frac{dz}{dx}=-\frac{F'_x}{F'_z},\quad z=z(x)\\
\ \\
\frac{dz}{dx}=\frac{\partial z}{\partial x}+\frac{\partial z}{\partial y}\frac{dy}{dx},\quad z=z(x,y)
\end{array}\right.$$

## 克拉默法则解方程组

**齐次，非齐次均适用**
ax + by = {\color{red}e}\\
cx + dy = {\color{red}f}$$
$$\begin{bmatrix} a & b \\ c & d \end{bmatrix}\begin{bmatrix} x \\ y \end{bmatrix}=\begin{bmatrix} {\color{red}e} \\ {\color{red}f} \end{bmatrix}$$
$$x = \frac { \begin{vmatrix} \color{red}{e} & b \\ \color{red}{f} & d \end{vmatrix} } { \begin{vmatrix} a & b \\ c & d \end{vmatrix} } = { {\color{red}e}d - b{\color{red}f} \over ad - bc}$$
$$y = \frac { \begin{vmatrix} a & \color{red}{e} \\ c & \color{red}{f} \end{vmatrix} } { \begin{vmatrix} a & b \\ c & d \end{vmatrix} } = { a{\color{red}f} - {\color{red}e}c \over ad - bc}$$

## 多元求“极值”与“最值”问题
开区域极值、边界最值、闭区域最值

$$开区域极值=无条件极值\\
边界最值=条件最值\\
闭区域最值=无条件极值+条件最值（无需判断极值点，直接比大小）$$

## 多元隐函数无条件极值问题

$$直接对方程求一阶偏导、二阶偏导\\
"令F_x'=F'_y=0"\\
\quad一阶导方程，解驻点\\
\quad二阶导方程，代入驻点解A,B,C
（二阶求偏导四选三即可）
\\
 \ \\
F'_z=0为不可导点，定义法讨论，对方程进行分析$$

## 条件最值问题
拉格朗日乘数法、反解消元法

$$拉格朗日乘数法：若函数、条件均有轮换对称性，则对应变量相等（结论好用，虽有误）

$$
$$反解消元法（“条件最值”向“无条件最值”的转化）：一般反解条件方程组不易，灵活使用\\
“约束条件”反解代入函数消元，原约束条件得新函数定义域（闭区间），转化为“无条件最值”$$
$$注：
\left\{\begin{array}{l}
无条件极值问题，即开区域求极值\\
条件最值问题，即约束条件下（边界）求最值
\end{array}\right.

$$

## 多元微分关系形成微分方程

$$z=xf(\frac{y}{x})+yf(\frac{y}{x})满足\frac{\partial z}{\partial x}=\frac{y}{x}\\
$$
$$\frac{\partial z}{\partial x}=f(\frac{y}{x})-\frac{y}{x}f'(\frac{y}{x})-\frac{y^2}{x^2}f'(\frac{y}{x})=\frac{y}{x}，
解微分方程$$

## 分段函数探讨连续，偏导连续，可微相关问题

$$坐标轴分段函数\\
\left\{\begin{array}{cl}
(x^2+y^2)\sin\frac{1}{xy},&xy\neq0\\
0,&xy=0
\end{array}
\right.\\
\ \\
f_x'(0,0)=\lim\limits_{x\to 0}\frac{f(x,0)-f(0,0)}{x}\\
f_x'(x,0)=0\\
f_x'(0,y)=\lim\limits_{x\to 0}\frac{f(x,y)-f(0,y)}{x}=\lim\limits_{x\to 0}\frac{(x^2+y^2)\sin\frac{1}{xy}}{x}\\
f_x'(x,y)=2x\sin\frac{1}{xy}-\frac{1}{x^2y}(x^2+y^2)\cos\frac{1}{xy}$$

## 二元函数二阶导

$$f_{xy}''(x_0,y_0)=\lim\limits_{y\to y_0}\frac{f_x'(x_0,y)-f_x'(x_0,y_0)}{y-y_0}（f_x'(x_0,y)为导函数，f_x'(x_0,y_0)为导数）$$
$$注：导函数可能用定义求得$$

# 微分方程

## 考情分析

**难点在于微分方程类型的识别**
考试大纲要求：仅要求求通解，不要求求出全部解

微分方程可结合性极强，可结合多种知识考查：
多元微分关系形成微分方程、幂级数微分关系形成微分方程
应用题型微分关系形成微分方程.......

 优先级：一阶线性 > 分离变量型 > 齐次型
 微分方程只考求解，按习惯计算即可，勿多想

## 微分方程可解性

$$只有少数简单的微分方程可以求得解析解\\
微分方程可解性较弱，故复杂题型也均属特殊构造，难点在于整理识别

$$

## 变量分离型

**分离变量、约分会改变定义域，但不要求求全部解**
**除线性微分方程外，分离变量方法贯穿微分方程求解始终**
$$\frac{dy}{dx}=f(x)g(y)$$

## 齐次型微分方程

$$\frac{dy}{dx}=\varphi(\frac{y}{x})$$

**齐次：整理为标准形式，分子分母阶次相同**
$$\frac{dy}{dx}=\varphi(\frac{y}{x}):\\
令u=\frac{y}{x},得y=ux,\frac{dy}{dx}=x\frac{du}{dx}+u\\
x\frac{du}{dx}+u=\varphi(u)$$
$$或\frac{dx}{dy}=\psi(\frac{x}{y}):
......$$
$$注：(\frac{y}{x})为0次\\
类型不明显，向标准形式(dy/dx)化
$$

## 一阶线性微分方程

$$y'+p(x)y=q(x)\\
y'+p(x)y=0$$

$$y=e^{-\int p(x)dx}[\int e^{\int p(x)dx}\cdot q(x)dx+C]（C为任意常数）$$
$$y=Ce^{-\int p(x)dx}$$
$$此处\int p(x)dx不加C，仅表示一个原函数\\
凡遇\int p(x)dx为\ln|\varphi(x)|均可直接去掉绝对值（分类讨论，后验解释）
$$

## 伯努利方程

$$y'+p(x)y=q(x)y^n(n\neq0,1)$$

**伯努利方程不易察觉**
$$变形为：y^{-n}\cdot y'+p(x)y^{1-n}=q(x)$$
$$令z=y^{1-n},得\frac{dz}{dx}=(1-n)y^{-n}\frac{dy}{dx}，则$$
$$\\
原式=\frac{1}{1-n}\cdot \frac{dz}{dx}+p(x)z=q(x)（一阶线性微分方程）$$
$$......（注意代回）$$

## 全微分方程
$$P(x,y)dx+Q(x,y)dy=0$$

$$当\frac{\partial Q}{\partial x}=\frac{\partial P}{\partial y}时，P(x,y)dx+Q(x,y)dy=0称为全微分方程\\
即du=P(x,y)dx+Q(x,y)dy=0（可知u(x,y)=C）$$
**解微分方程问题=由偏导反求原函数问题**
$$(y-x^2)dx+(x-1)dy=0$$
**公式法（易混）：**
$$u(x,y)=\int_{x_0}^{x}P(x,y_0)dx+\int_{y_0}^yQ(x,y)dy=C_1$$
**积分法（两步走）：**
$$\frac{\partial u}{\partial x}=y-x^2,\frac{\partial u}{\partial y}=x-1\\
u=\int (y-x^2)dx+C_1(y)=xy-\frac{x^3}{3}+C_1(y)\\
\frac{\partial u}{\partial y}=x+C_1'(y)=x-1,即C_1'(y)=-1,C_1(y)=-y+C_1\\
故u(x,y)=xy-\frac{x^3}{3}-y=C$$
**微分元法（勿用，难以对应）：**
$$\begin{array}{rl}du&=(2x+y)dx+(2y)dy\\
&=d(x^2+xy)+d(y^2)\\
&=d(x^2+y^2+xy)\quad \times
\end{array}$$

## 欧拉方程（固定解法）
$$x^2y''+pxy'+qy=f(x)$$

$$x>0时，令x=e^t，t=\ln x,\frac{dt}{dx}=\frac{1}{x}（固定处理，用以消去x相关项）\\
\left\{
\begin{array}{l}
\frac{dy}{dx}=\frac{dy}{dt}\cdot \frac{dt}{dx}=\frac{1}{x}\frac{dy}{dt}\\
\\
\frac{d^2y}{dx^2}=\frac{d}{dx}(\frac{1}{x}\frac{dy}{dt})=-\frac{1}{x^2}\frac{dy}{dt}+\frac{1}{x}\frac{d}{dx}(\frac{dy}{dt})=-\frac{1}{x^2}\frac{dy}{dt}+\frac{1}{x}\frac{d(\frac{dy}{dt})}{dt}\cdot \frac{dt}{dx}=-\frac{1}{x^2}\frac{dy}{dt}+\frac{1}{x^2}\frac{d^2y}{dt^2}
\end{array}
\right.\\
\ \\
注：高阶同理，k阶求导后均对应\frac{1}{x^k}$$
$$\frac{d^2y}{dt^2}+(p-1)\frac{dy}{dt}+qy=f(e^t)（常系数非齐次线性微分方程）$$
$$x<0时，令x=-e^t,同理即可$$
$$注：解完方程，注意回代变量t=\ln x$$

## 二阶可降阶微分方程
$$y''=f(x,y')型\\
y''=f(y,y')型$$

**关键：降阶，处理为一阶微分方程**
$$y''=f(x,y')型：\\
令p=y',p'=y'',原方程:\frac{dp}{dx}=f(x,p)\\
y=\int p(x,C_1)dx+C_2$$
$$y''=f(y,y')型：\\
令y'=p,y''=\frac{dp}{dx}=\frac{dp}{dy}\cdot \frac{dy}{dx}=\frac{dp}{dy}\cdot p\\
原方程：p\frac{dp}{dy}=f(y,p)\\
p=\frac{dy}{dx}=\varphi(y,C_1)$$
$$注：二阶方程应有两个初始条件，任意一步均可代入$$

## 微分方程通解、特解的定义

$$通解：若微分方程中含有独立的任意常数的个数等于微分方程的阶数，则称此解为微分方程的通解$$
$$特解：不含任意常数的解称为微分方程的特解$$

## 线性微分方程解的性质
一般线性、常系数线性

$$全部解的构成：齐次通解+非齐次特解\\
（除去“齐次通解因子”，“非齐次特解因子”唯一）$$
$$齐次解叠加性：y_1,y_2,y_3,\cdots,y_n为齐次解\\
k_1y_1+k_2y_2+\cdots+k_ny_n仍为齐次解$$
$$非齐次解叠加性：y_1,y_2,y_3,\cdots,y_n为非齐次解\\
k_1y_1+k_2y_2+\cdots+k_ny_n\left\{
\begin{array}{ll}
\sum k_i=0,齐次解\\
\sum k_i=1,非齐次解
\end{array}
\right.$$
$$注：
常系数线性微分方程与线性方程组性质相似，但不相同\\
常系数线性微分方程的非齐次解可以“模态”分解，线性方程组不可$$

## 常系数线性微分方程线性无关解个数

$$n阶常系数线性微分有n维“模态”或“基向量”\xRightarrow{} n阶常系数线性齐次微分方程必有n个线性无关的解$$
$$非齐次特解必然无法被齐次通解线性表示\xRightarrow{}n阶常系数线性非齐次微分方程必有n+1个线性无关的解$$

## 高阶常系数齐次线性微分方程的通解
$$y^{(n)}+a_1y^{(n-1)}+\cdots+a_{n-1}y'+a_ny=0$$

$$令r^n+a_1r^{n-1}+\cdots+a_{n-1}+a_n=0,解特征根r_i，得通解:$$
$$r_i\left\{
\begin{array}{l}
实根（个数）\quad [C_0+C_1x+C_2x^2+\cdots+C_{n-1}x^{n-1}]e^{r_i}\\
\\
复根 \alpha\pm\beta i（对数）\quad e^\alpha[(C_0+C_1x+\cdots+C_{n-1}x^{n-1})\sin\beta x+(D_0+D_1x+\cdots+D_{n-1}x^{n-1})\cos\beta x]
\end{array}
\right.$$

## 高阶常系数非齐次线性微分方程的特解
$$y^{(n)}+a_1y^{(n-1)}+\cdots+a_{n-1}y'+a_ny=f(x)$$
$$f(x)=P_n(x)e^{\alpha x}\\
f(x)=e^{\alpha x}[P_m(x)\cos\beta x+P_n(x)\sin\beta x]$$

$$f(x)=P_n(x)e^{\alpha x}时，y^*=e^{\alpha x}Q_n(x)x^k\\
k=(\alpha等于特征根r_i)的个数$$
$$f(x)=e^{\alpha x}[P_m(x)\cos\beta x+P_n(x)\sin\beta x]时，y^*=e^{\alpha x}[Q_l(x)\cos\beta x+R_l(x)\sin\beta x]x^k\\
l=\max\{m,n\}\qquad
k=(\alpha\pm\beta i等于特征根)的对数$$
可能考查[Card#ID/1Yzk6#积化和差、和差化积]

## 解特征根注意
$$(x-1)^3=0,\  x^3-1=0$$

$$(x-1)^3=0\Rightarrow x_{1,2,3}=1\\
  x^3-1=0\Rightarrow (x-1)(x^2+x+1)=0\Rightarrow x_1=1,x_{2,3}=\frac{-1\pm\sqrt{3}\ i}{2}$$

## 微分方程的“任意常数C”问题

**不要求求全部解，但通解形式要求简介美观**
$$\frac{dy}{dx}=2\sqrt{y}\\
\int \frac{dy}{2\sqrt{y}}=\int dx
\\
\sqrt{y}=(x+C)\\
y=(x+C)^2
（y=0为奇解，不包含在通解内，不用补）
$$
$$\sin(y+C_1)=\pm e^{C_0}e^x\\
\sin(y+C_1)=0为微分方程的解\\
\sin(y+C_1)=C_2e^x(C_1,C_2为任意常数)$$
$$(1+y^2)^3=e^{2C_0}(1+x^2)\\
(1+y^2)^3=C(1+x^2)(C为任意常数，且C>0)\\
$$

## 变量替换解微分方程

常规型，特殊型

**常规型：**
$$\ \  1.  \ \frac{dy}{dx}=f(ax+by+c)\Rightarrow
u=ax+by+c\\
\left.\begin{array}{l}
2.\ y'=\frac{y^2-x}{2y(x+1)}\Rightarrow (y^2)'=\frac{y^2-x}{x+1}\\
3.\ y\cdot y''+(y')^2=0\Rightarrow
(y\cdot y')'=0\Rightarrow y\cdot y'=C
\end{array}\right\}灵活利用辅助函数思想$$
**特殊型：**
$$利用变换t=\tan x求解，\cos^4x\frac{d^2y}{dx^2}+2\cos^2x(1-\sin x\cos x)\frac{dy}{dx}+y=\tan x（与欧拉方程同理）\\
\left\{\begin{array}{l}
\frac{dy}{dx}=\frac{dy}{dt}\cdot\frac{dt}{dx}=\frac{1}{\cos^2x}\cdot\frac{dy}{dt}\\
\ \\
\frac{d^2y}{dx^2}=\frac{2\sin x}{\cos^3x}\cdot\frac{dy}{dt}+\frac{1}{\cos^4x}\frac{d^2y}{dt^2}
\end{array}\right.$$
$$反函数替换，参数方程替换等（仅在于形式转换，无关难易）$$

## 微分方程反解函数问题

$$反三角函数直接反解，三角函数勿反解$$

## 应用题求函数

$$典例：
切点为(x,f(x)),直线表示Y-f(x)=f'(x)(X-x)，直线所过点(x_0,y_0)代入X,Y\\
（仅此题较绕，其余按题目列写表达式，构造微分方程即可）$$
$$注：首要考虑微分方程求解，并求特解，根据题干找初始条件f(a),f'(a)$$

## 注意事项

$$微分方程满足条件y(0)=2,y'(0)=0的解\\
注意是齐次方程的解还是非齐次方程的解满足条件$$

## 知一般线性微分方程线性无关解，求非齐次通解、特解

$$y_1,y_2,y_3为二阶线性非齐次微分方程的三个线性无关解，则\\
(y_1-y_2),(y_2-y_3)也线性无关\\
\ \\
将y_1,y_2,y_3视作向量，用线性代数处理\\
A=(y_1,y_2,y_3)
\left(
\begin{array}{}
1 & 0\\
-1& 1\\
0& -1
\end{array}
\right),r(A)=2\\
非齐次通解=C_1(y_1-y_2)+C_2(y_2-y_3)+y_i$$

## 知常系数线性微分方程的具体解，反求微分方程

**思路：分析讨论（解均是特别给的）**
$$便捷技巧

\left\{\begin{array}{l}
齐次解：找特征根即可\\
非齐次解：先分析非齐次特解因子，再找特征根
\end{array}\right.

$$
$$注：分析法优先，代入法备用（待定系数的思路）$$

## 微分方程导数定义构造典例1

$$典例一：\\
f(x+y)=e^yf(x)+e^xf(y),f'(0)=1,求f(x)\\
\Rightarrow f(0)=0\\

f'(x)=\lim\limits_{\Delta x \to 0}\frac{f(x+\Delta x)-f(x)}{\Delta x}=\lim\limits_{\Delta x \to 0}\frac{e^{\Delta x}f(x)+e^xf(\Delta x)-f(x)}{\Delta x}=\lim\limits_{\Delta x \to 0}\frac{(e^{\Delta x}-1)f(x)+e^xf(\Delta x)}{\Delta x}=f(x)+e^xf'(0)$$
$$典例二：\\
f(xy)=yf(x)+xf(y),f'(1)=2,求f(x)\\
\Rightarrow f(1)=0\\

f'(x)=\lim\limits_{\Delta x\to 0}\frac{f(x+\Delta x)-f(x)}{\Delta x}=\lim\limits_{\Delta x\to 0}\frac{f[x(1+\frac{\Delta x}{x})]-f(x)}{\Delta x}=\lim\limits_{\Delta x\to 0}\frac{\frac{\Delta x}{x}f(x)}{\Delta x}+\lim\limits_{\Delta x\to 0}\frac{f(1+\frac{\Delta x}{x})}{\frac{\Delta x}{x}}=\frac{f(x)}{x}+f'(1)$$

## 微分方程导数定义构造典例2

$$正值可导函数f(x)满足\lim\limits_{t\to \infty}\left[\frac{f(x+\tan\frac{1}{t})}{f(x+\sin\frac{1}{t})}\right]^{t^3}=e^x,且f(0)=1,求f(x)$$
![](pic-advance-math\Markji_1751354385159.jpg)
$$注：
导函数不一定连续，拉格朗日中值行不通$$

# ""数项级数""

## 考情分析

**数项级数考查敛散性**
1. 正（负）项级数审敛几大方法：
比较审敛法（一般用于证明）、比较审敛法的极限形式、比值审敛法、根值审敛法、积分审敛法
2. 数列的敛散性容易分析，数项级数的敛散性较复杂
3. 重难点：数项级数的证明题

## 数列收敛与子列的关系

**关键在“致密性”，跟函数与数列的关系同理**
$$\{x_n\}收敛\ \substack{\Rightarrow\\ \not\Leftarrow}\{x_{2n}\}收敛\\
$$
$$\{x_{2n}\}发散\ \substack{\Rightarrow\\ \not\Leftarrow}\{x_n\}发散$$

## 数列与级数的关系

$$级数可完全视作数列\\
数列也可完全视作级数\\
\ \\
子数列（连续求和）\neq 子级数（跳跃求和）\sum_{i=1}^{\infty} u_{2i}$$

## 级数收敛的必要条件

$$\sum_{n=0}^{\infty}u_n收敛\Rightarrow\lim\limits_{n\to \infty}u_n=0\\
\lim\limits_{n\to \infty}u_n\neq0\Rightarrow\sum_{n=0}^{\infty}u_n发散$$

## 数项级数的性质

$$在\sum u_n中任意加括号会提高级数的收敛性\\
\ \\
在\sum u_n中任意加绝对值会提高级数的发散性\\
\ \\
若级数\sum u_n绝对收敛，不论将其各项如何重新排列，所得新级数也绝对收敛，且其和不变
$$

## 正项级数收敛与有界的关系

$$\sum u_n收敛\Leftrightarrow\{S_n\}收敛\Leftrightarrow \{S_n\}有界$$

## 数项级数敛散性常用结论1

$$\sum_{n=1}^{\infty}u_n收敛，\sum_{n=1}^{\infty}v_n收敛\Rightarrow \sum_{n=1}^{\infty}(u_n\pm v_n)收敛\not\Rightarrow
\sum_{n=1}^{\infty}u_n v_n收敛\\（u_n,v_n\to 0的速度互相加快了，但交错级数可能正负号相消了）\\
\ \\
\sum_{n=1}^{\infty}u_n收敛，\sum_{n=1}^{\infty}v_n发散
\Rightarrow \sum_{n=1}^{\infty}(u_n\pm v_n)发散\\
\ \\
\sum_{n=1}^{\infty}u_n发散，\sum_{n=1}^{\infty}v_n发散
\not\Rightarrow \sum_{n=1}^{\infty}(u_n\pm v_n)发散\quad（问题在于正负相消）\\
\ \\
\sum_{n=1}^{\infty}u_n发散(u_n\geqslant0)，\sum_{n=1}^{\infty}v_n发散(v_n\geqslant0)
\Rightarrow \sum_{n=1}^{\infty}(u_n+ v_n)发散$$

## 数项级数敛散性常用结论2

$$\sum_{n=1}^{\infty}u_n收敛\ \substack{\Rightarrow\\
\not\Leftarrow}\sum_{n=1}^{\infty}(u_{2n-1}+u_{2n})收敛\quad (反例：u_n=(-1)^n)\\
\ \\
\sum_{n=1}^{\infty}(-1)^{n-1}u_n(u_n>0)收敛\Rightarrow \sum_{n=1}^{\infty}(u_{2n-1}-u_{2n})收敛\\
\ \\
\sum_{n=1}^{\infty}(u_{2n-1}+u_{2n})收敛且\lim\limits_{n\to \infty}u_{n}=0\Rightarrow \sum_{n=1}^{\infty}u_n收敛\quad （S_{2n},S_{2n+1}均收敛于A\Leftrightarrow S_n收敛于A）\\
$$
$$\left\{
\begin{array}{l}
\sum_{n=1}^{\infty}u_n收敛\Leftarrow \sum_{n=1}^{\infty}u_{2n-1}与\sum_{n=1}^{\infty}u_{2n}均收敛\quad（注意：非子数列，结论3证得）\\
\\
正项级数：\sum_{n=1}^{\infty}u_n收敛\Leftrightarrow \sum_{n=1}^{\infty}u_{2n-1}与\sum_{n=1}^{\infty}u_{2n}均收敛\quad（充分性可用比较法理解，勿深究）
\end{array}
\right.$$
$$\sum_{n=1}^{\infty}u_{2n-1}与\sum_{n=1}^{\infty}u_{2n}中一个发散，一个收敛\Rightarrow\sum_{n=1}^{\infty}u_n发散\quad（\sum_{n=1}^{\infty}(u_{2n-1}+u_{2n})发散，故\sum_{n=1}^{\infty}u_n发散）$$

## 数项级数敛散性常用结论3

$$\sum_{n=1}^{\infty}u_n收敛\Rightarrow \sum_{n=1}^{\infty}(\alpha u_n+ \beta u_{n-1})收敛\quad（收敛的叠加性证得）\\
\ \\
\lim\limits_{n\to \infty}u_n存在\Leftrightarrow\sum_{n=1}^{\infty}(u_{n+1}-u_n)收敛\quad（级数展开，所见即所得）$$

## 数项级数敛散性常用结论4

$$\sum_{n=1}^{\infty}u_n收敛，\sum_{n=1}^{\infty}|v_n|收敛\Rightarrow\sum_{n=1}^{\infty}|u_n v_n|收敛，\sum_{n=1}^{\infty}u_n\cdot|v_n|收敛\quad（\lim\limits_{n\to \infty}|v_n|,加快了|u_n|,u_n\to 0的速度）\\
\ \\
\sum_{n=1}^{\infty}u_n与\sum_{n=1}^{\infty}v_n至少有一个发散\Rightarrow\sum_{n=1}^{\infty}(|u_n|+|v_n|)发散\quad （均为正项级数，无法正负相消）\\
\ \\
\sum_{n=1}^{\infty}u_n^2与\sum_{n=1}^{\infty}v_n^2都收敛\Rightarrow \sum_{n=1}^{\infty}|u_n v_n|与\sum_{n=1}^{\infty}(u_n+v_n)^2均收敛\quad(|u_n v_n|\leqslant\frac{1}{2}(u_n^2+v_n^2),\quad(u_n+v_n)^2\leqslant2(u_n^2+v_n^2))$$

## 数项级数敛散性常用结论5

$$\sum_{n=1}^{\infty}u_n(u_n\geqslant0)收敛\Rightarrow\sum_{n=1}^{\infty}u_n^2,\sum_{n=1}^{\infty}\sqrt{u_n u_{n+1}},\sum_{n=1}^{\infty}\frac{\sqrt{u_n}}{n}均收敛\\(u_n^2\leqslant u_n(n充分大),\quad\sqrt{u_n u_{n+1}}\leqslant\frac{1}{2}(u_n+u_{n+1}),\quad\frac{\sqrt{u_n}}{n}\leqslant\frac{1}{2}(u_n+\frac{1}{n^2}))$$
$$\sum_{n=1}^{\infty}u_n收敛\not\Rightarrow \sum_{n=1}^{\infty}|u_n|,\sum_{n=1}^{\infty}u_n^2,\sum_{n=1}^{\infty}(-1)^n u_n,\sum_{n=1}^{\infty}u_n u_{n+1}收敛\quad(反例：\sum_{n=1}^{\infty}\frac{(-1)^n}{\sqrt{n}})$$
$$\sum_{n=1}^{\infty}u_n^2收敛\Rightarrow \sum_{n=1}^{\infty}\frac{u_n}{n}绝对收敛\qquad (|u_n\cdot \frac{1}{n}|\leqslant \frac{1}{2}(u_n^2+\frac{1}{n^2}))$$

## 正项级数敛散性分析思路

$$正项级数敛散一般看通项在趋于
\infty
时的“表现”，
即正项级数判别尺度$$
$$比值判别法，根值判别法，积分审敛法\ 为补充方法（覆盖不同情形）$$

## 正项级数敛散判别尺度

$$\sum_{n=1}^{\infty}\frac{1}{n^p}\left\{
\begin{array}{ll}
发散，& p\leqslant1\\
&&（0^p阶次越高越收敛）\\
收敛，& p>1
\end{array}
\right.$$

## 比较判别法的极限形式

**级数判敛的核心方法**
$$正项级数\sum_{n=0}^{\infty}u_n$$
$$\lim\limits_{n\to \infty}\frac{u_n}{(\frac{1}{n})^p}=A\neq0，则\sum_{n=1}^{\infty} u_n与\sum_{n=1}^{\infty} (\frac{1}{n})^p同敛散$$
$$\lim\limits_{n\to \infty}\frac{u_n}{(\frac{1}{n})^p}=\infty,且p\leqslant1,则发散$$
$$\lim\limits_{n\to \infty}\frac{u_n}{(\frac{1}{n})^p}=0,且p>1,则收敛$$

## 比值判别法与根值判别法

$$小结论：比值法极限存在\substack{\Rightarrow \\ \not\Leftarrow}根植法极限存在$$
**比值判别法：**
$$正项级数\sum_{n=1}^{\infty}u_n,\ 若\lim\limits_{x\to \infty}\frac{u_{n+1}}{u_n}=\rho,则\\
\left\{
\begin{array}{ll}
\rho<1,& 级数收敛\\
\\
\rho>1,& 级数发散
\end{array}
\right.$$
**根值判别法：**
$$正项级数\sum_{n=1}^{\infty}u_n,\ 若\lim\limits_{x\to \infty}\sqrt[n]{u_n}=\rho,则\\
\left\{
\begin{array}{ll}
\rho<1,& 级数收敛\\
\\
\rho>1,& 级数发散
\end{array}
\right.$$

## 积分审敛法

$$级数通项u_n非负单减，则\sum f(n)与\int_a^{+\infty}f(x)dx同敛散$$
$$简证：\\
\sum_{n=1}^{k} f(n+1) \leqslant
\sum_{n=1}^{k} \int_n^{n+1} f(x)\, dx \leqslant
\sum_{n=1}^{k} f(n)\\

\sum_{n=1}^{k} \int_n^{n+1} f(x)\, dx= \int_1^{k+1} f(x)\, dx\\

\sum_{n=1}^{\infty}f(n+1)\leqslant\int_1^{+\infty}f(x)dx\leqslant\sum_{n=1}^{\infty}f(n)（k\to +\infty时，f(x)\to 0）$$

## 莱布尼茨判别法（交错级数）

**交错级数的收敛比较特别**
$$\sum_{n=1}^{\infty}(-1)^{n-1}u_n（与首项正负无关）, \ u_n>0, n=1,2,\cdots\\若\{u_n\}单调不增且\lim\limits_{n\to \infty}u_n=0,则该级数收敛\\
（单调有界准则证明，加括号证有界、单调）$$
$$交错级数判单减方法：导函数正负、比值法等$$

## 泰勒展开判敛方法

**重要判别方法，与极限判别法地位等同**
$$思路：\\
泰勒展开为各阶无穷小的子级数求和\\判别n\to \infty时，各子级数u_n趋于0的阶次$$
$$例：\\ \sum_{n=1}^{\infty}(-1)^nu_n=\sum_{n=1}^{\infty}\frac{(-1)^n}{\sqrt{n+(-1)^n}}\\
u_n=\frac{1}{\sqrt{n}}[1+\frac{(-1)^n}{n}]^{-\frac{1}{2}}=\frac{1}{\sqrt{n}}[1-\frac{1}{2}\frac{(-1)^n}{n}+\circ(\frac{1}{n})]\\

（由判别尺度可知，p>1即收敛，\circ(\frac{1}{n})<\frac{A}{n^2}+\frac{B}{n^3}+n\frac{C}{n^4}收敛\\
故高阶无穷小对应子级数之和必收敛）$$

## 数项级数证明题

$$主要使用比较审敛法，
灵活使用极限等价、泰勒展开、数列极限等相关技巧$$

# 幂级数

## 阿贝尔定理

$$\sum_{n=0}^{\infty}a_nx^n在x=x_1处收敛，对于满足|x|<|x_1|的一切x,幂级数\ \textbf{绝对收敛}$$
$$\sum_{n=0}^{\infty}a_nx^n在x=x_2处发散，对于满足|x|>|x_1|的一切x,幂级数\ \textbf{发散}$$

## 阿贝尔定理证明

$$设x_0是\sum_{n=0}^{\infty}a_nx^n的收敛点，根据级数收敛的必要条件，有\\
\quad\ \lim\limits_{n\to \infty}a_nx^n_0=0\\
\Rightarrow|a_nx_0^n|\leqslant M\\
\Rightarrow|a_n x^n|=|a_nx_0^n|\cdot\left|\frac{x^n}{x_0^n}\right|\leqslant M\left|\frac{x}{x_0}\right|^n\\
故\  |x|<|x_0|时，\sum_{n=0}^{\infty}M\left|\frac{x}{x_0}\right|^n收敛，此时\sum_{n=0}^{\infty}|a_nx^n|收敛

$$
$$发散性质由反证法证得......$$

## 收敛半径的求法

$$\lim\limits_{n\to \infty}\left|\frac{a_{n+1}}{a_n}\right|=\rho,\ 则\sum_{n=0}^{\infty}a_nx^n的收敛半径为\\
R=
\left\{
\begin{array}{ll}
\frac{1}{\rho},& \rho\neq0\\
\\
+\infty,& \rho=0\\
\\
0,& \rho=+\infty
\end{array}
\right.\qquad{\color{blue}本质： \lim\limits_{n\to \infty}\left|\frac{a_{n+1}}{a_n}\right|\left|\frac{x_{n+1}}{x_n}\right|<1时绝对收敛，故\left|\frac{x_{n+1}}{x_n}\right|<\frac{1}{\rho}时绝对收敛}$$
$$注：
\sum_{n=0}^{\infty}a_{n}x^{n}与\sum_{n=0}^{\infty}a_{2n}x^{2n}收敛半径相同\\
收敛区间为开区间，收敛域需讨论区间端点$$

## 幂级数线性叠加的收敛半径

$$\sum_{n=0}^{\infty}a_n x^n与\sum_{n=0}^{\infty}b_n x^n的收敛半径分别为R_1,R_2(R_1\neq R_2)\\
\sum_{n=0}^{\infty}\alpha a_n \pm \beta b_n x^n的收敛半径为\min\{R_1,R_2\}$$
$$注：\\
若R_1\neq R_2
\left\{
\begin{array}{l}
公共收敛区间叠加后必收敛\\
\\
非公共收敛区间叠加必发散\\
（由阿贝尔定理，以外区间也发散）
\end{array}
\right.\\
若R_1= R_2，则R\geqslant\min\{R_1,R_2\}$$

## 幂级数绝对收敛、发散、条件收敛的关系

$$\sum_{n=0}^{\infty}a_nx^n
\left\{
\begin{array}{ll}
绝对收敛，& |x|<R\\
\\
&|x|=R\Leftarrow (\substack{x=x_1条件收敛\\
\\
或x=x_1收敛，x=-x_1发散})\\
\\
发散，& |x|>R
\end{array}
\right.$$

## 和函数性质

$$S(x)在收敛域上连续$$

## 幂级数展开式
$$e^x,\ln(1+x),\quad \frac{1}{1+x},\frac{1}{1-x},\quad \sin x,\cos x,\quad \arctan x$$

**有阶乘域无穷，无阶乘域为“1”**
$$\mathrm{e}^x=\sum_{n=0}^{\infty} \frac{x^n}{n !} =1+x+\frac{x^2}{2!}+\cdots+\frac{x^n}{n!}+\cdots\quad(-\infty<x<+\infty)\\
\ln (1+x)=\sum_{n=1}^{\infty} \frac{(-1)^{n-1} x^n}{n} =x-\frac{x^2}{2}+\frac{x^3}{3}-\frac{x^4}{4}+\cdots+(-1)^{n-1}\frac{x^n}{n}+\cdots\quad(-1<x \leqslant 1) $$
$$\frac{1}{1+x}=\sum_{n=0}^{\infty}(-1)^n x^n=1-x+x^2-x^3+\cdots+(-1)^nx^n+\cdots\quad(-1<x<1)\\
\frac{1}{1-x}=\sum_{n=0}^{\infty}x^n=1+x+x^2+\cdots+x^n+\cdots\quad(-1<x<1)$$
$$\sin x=\sum_{n=0}^{\infty} \frac{(-1)^n x^{2 n+1}}{(2 n+1) !}=x-\frac{x^3}{3!}+\frac{x^5}{5!} -\frac{x^7}{7!}+\cdots+(-1)^n\frac{x^{2n+1}}{(2n+1)!}+\cdots\quad(-\infty<x<+\infty)\\
\cos x=\sum_{n=0}^{\infty} \frac{(-1)^n x^{2 n}}{(2 n) !}=1-\frac{x^2}{2!}+\frac{x^4}{4!} -\frac{x^6}{6!}+\cdots+(-1)^n\frac{x^{2n}}{(2n)!}+\cdots\quad(-\infty<x<+\infty)$$
$$\arctan x =\sum_{n=0}^{\infty}(-1)^n\frac{x^{2n+1}}{2n+1}=x-\frac{x^3}{3} + \frac{x^5}{5}-\cdots +\frac{(-1)^n}{2n+1} x^{2n+1}+\cdots\quad (-1\leqslant x\leqslant 1)
$$

## 幂级数展开式（补）

$$\frac{e^x+e^{-x}}{2},\frac{e^x-e^{-x}}{2}\quad e^{-x},-\ln(1-x)$$

$$\frac{e^x+e^{-x}}{2}=\sum_{n=0}^{\infty}\frac{x^{2n}}{(2n)!}=1+\frac{x^2}{2!}+\frac{x^4}{4!}+\cdots+\frac{x^{2n}}{(2n)!}+\cdots\quad(-\infty<x< +\infty)\\

\frac{e^x-e^{-x}}{2}=\sum_{n=0}^{\infty}\frac{x^{2n+1}}{(2n+1)!}=x+\frac{x^3}{3!}+\frac{x^5}{5!}+\cdots+\frac{x^{2n+1}}{(2n+1)!}+\cdots\quad(-\infty<x< +\infty)$$
$$e^{-x}=\sum_{n=0}^{\infty} \frac{(-x)^n}{n !}=\sum_{n=0}^{\infty} \frac{(-1)^nx^n}{n !} =1-x+\frac{x^2}{2!}-\frac{x^3}{3!}+\cdots+(-1)^n\frac{x^n}{n!}+\cdots\quad(-\infty<x<+\infty)\\
-\ln (1-x)=\sum_{n=1}^{\infty} \frac{(-1)(-1)^{n-1} (-x)^n}{n} =\sum_{n=1}^{\infty} \frac{(-1)^{2n} x^n}{n}=x+\frac{x^2}{2}+\frac{x^3}{3}+\cdots+\frac{x^n}{n}+\cdots\quad(-1\leqslant x <1) $$

## 狄利克雷收敛定理

$$设f(x)是以[-l,l]为周期的可积函数，如果在[-l,l]上f(x)满足：\\
1. f(x)连续或只有有限个第一类间断点\\
2. f(x)只有有限个极值\\
则f(x)的傅里叶级数\frac{a_0}{2}+\sum_{n=1}^{\infty}(a_n\cos nx+b_n\sin nx)的和函数为\\
S(x)=
\left\{
\begin{array}{ll}
f(x),&x为连续点\\
\frac{f(x+0)+f(x-0)}{2},&x为间断点\\
\frac{f(-l+0)+f(l-0)}{2},&x=\pm l
\end{array}
\right.$$

## 傅里叶级数

$$f(x)\sim\frac{a_0}{2}+\sum^\infty_{n=1}(a_n\cos\frac{n\pi x}{l}+b_n\sin\frac{n\pi}{l}x)\\

\left.\begin{array}{l}
a_0=\frac{1}{l}\int_{-l}^lf(x)dx= a_n|_{n=0}\\
\ \\
a_n=\frac{1}{l}\int_{-l}^lf(x)\cos\frac{n\pi x}{l}dx,n=1,2,\cdots\\
\ \\
b_n=\frac{1}{l}\int_{-l}^lf(x)\sin\frac{n\pi x}{l}dx,n=1,2,\cdots
\end{array}\right\}积分区间不固定，2l即可$$
$$f(x)偶函数\rightarrow余弦级数，f(x)=\frac{a_0}{2}+\sum_{n=1}^{\infty}a_n\cos \frac{n\pi x}{l}\\
f(x)奇函数\rightarrow正弦级数，f(x)=\sum_{n=1}^{\infty}b_n\sin \frac{n\pi x}{l}$$
$$注：2l须为f(x)的最小正周期；
否则，会丢失部分谐波\\
借"m"求"n"次的系数，\int_{-\mu}^{\mu}\cos\frac{m\pi x}{\mu}\cos\frac{n\pi x}{l}dx(\mu=kl,k>1)$$

## 傅里叶级数奇延拓，偶延拓

$$\left\{
\begin{array}{l}S(x)=\sum_{n=1}^{\infty}b_n\sin n\pi x\\
\ \\
 b_n=2\int_0^lf(x)\sin n\pi xdx
\end{array}
\right.\rightarrow 奇延拓[0,l]上的f(x)$$
$$\left\{
\begin{array}{l}S(x)=\frac{a_0}{2}+\sum_{n=1}^{\infty}a_n\cos n\pi x\\
\ \\
 a_n=2\int_0^lf(x)\cos n\pi xdx
\end{array}
\right.\rightarrow 偶延拓[0,l]上的f(x)$$
$$注：仅考查周期奇延拓与偶延拓\\
对[-a,b]的函数作奇、偶延拓得到的不是函数
$$

## 傅里叶级数小结论

$$\int_{-l}^l\cos\frac{n\pi x}{l}dx=\int_{-l}^l\sin\frac{n\pi x}{l}dx=0$$
$$\int_{0}^l\sin\frac{n\pi x}{l}dx=\frac{-1}{n\pi}(\cos n\pi-1)=\frac{-1}{n\pi}((-1)^n-1)\\
\int_{0}^l\cos\frac{n\pi x}{l}dx=0
$$

## 和函数的逐项求导、逐项积分原则

$$若在收敛区间(-R,R)上有和函数S(x)=\sum_{n=0}^{\infty}a_nx^n,则\\
在(-R,R)内有S'(x)=\sum_{n=1}^{\infty}na_nx^{n-1}$$
$$若在收敛区间(-R,R)上有和函数S(x)=\sum_{n=0}^{\infty}a_nx^n,则\\
在(-R,R)内有\int_0^xS(x)dx=\sum_{n=0}^{\infty}\frac{a_n}{n+1}x^{n+1}$$
$$收敛半径：逐项求导、逐项积分后不变\\
收敛域：逐项求导可能“去端点”、逐项积分可能“加端点”（数项级数收敛判断）$$

## 数项级数与幂级数的转化

$$收敛关系转化：\sum_{n=0}^{\infty}a_n条件收敛\Leftrightarrow \sum_{n=0}^{\infty}a_n(x-2)^n在x=3处条件收敛$$
$$数项级数求和：\sum_{n=0}^{\infty}a_n = \sum_{n=0}^{\infty}a_nx^n\left|_{x=1}\right.$$

## 缺项型幂级数求收敛域
$$\sum_{n=0}^{\infty}a_nx^{2n},
\sum_{n=0}^{\infty}a_nx^{2n+1}$$

$$令t=x^2\\
\sum_{n=0}^{\infty}a_nx^{2n}=\sum_{n=0}^{\infty}a_nt^n, x^2\in(-R,R)\Rightarrow x\in(-\sqrt{R},\sqrt{R})\\

\sum_{n=0}^{\infty}a_nx^{2n+1}=x\sum_{n=0}^{\infty}a_nt^n,x^2\in(-R,R)\Rightarrow x\in(-\sqrt{R},\sqrt{R})$$

## 和函数相关运算注意

**加和号“∑”的下标注意:**
$$通项“+1”，下标“-1”\\
通项“-1”，下标“+1”\\
拆项后约分：
注意无效项，改下标勿多勿漏

$$
$$求导后未出现无效项，无需改变下标\\
无效项：阶乘(-b)!\quad x^k(k< 0)$$
**首先计算幂级数收敛域并标注**
**使用级数公式时，注意标注收敛域**
$$配\frac{1}{x^k}时，注意讨论\left\{\substack{x=0\\x\neq0}\right.$$

## 求和函数技巧

**展开式侧凑**
**前提，先求收敛域**
$$形式处理：裂项、拆分、凑已知展开式等\quad{\color{blue}关键：配凑单次因式（仅单次因式可被“积”“导”处理）}\\
例：\sum_{n=0}^{\infty}\frac{4n^2+4n+3}{2n+1}x^{2n},\quad\sum_{n=0}^{\infty}(-1)^{n-1}[1+\frac{1}{n(2n-1)}]x^{2n},\quad \sum_{n=0}^{\infty}\frac{1+n^2}{n!\cdot2^n}x^n,\quad \sum_{n=0}^{\infty}(-1)^n\frac{n+1}{(2n+1)!}x^{2n+1}$$
$$先积后导：\sum_{n=1}^{\infty} nx^{n-1}=\sum_{n=1}^{\infty}(x^n)'=(\sum_{n=1}^{\infty}x^n)'=S(x)\\
先导后积：\sum_{n=1}^{\infty}\int_0^x(\frac{1}{n}x^n)'dx=\int_0^x\sum_{n=1}^{\infty}x^{n-1}dx=S(x)-S(0)\\
\ \\
注：
\begin{array}{l}
若整体求导、积分，求导、积分符号可直接放至\sum内外，否则不可\\
“高次”型中间增设S_1(x)，提取\frac{1}{x}或x等后的展开式，设为S_1(x)
\end{array}$$
$$微分方程：\\
1. 已知数列递推式，勿解通项，幂级数求导、积分可构造微分方程\\
(n+1)a_{n+1}=na_n+a_{n-1}（统一累加下限即可），根据a_n关系构造对应幂级数，可得S(x)的关系方程\\
2. 难以寻找规律，可求导，寻找导数间关系，借助微分方程解函数

$$

## 幂级数展开技巧

**函数侧凑**
$$凑形式展开：\\
\ln(4x-5)展开成(x-2)的幂级数（即可便捷求出x=2处的高阶导）\\
\ln(4(x-2)+3)=\ln3(1+\frac{4(x-2)}{3})=\ln3+\ln(1+\frac{4(x-2)}{3})\\
注：(x-1)\frac{1}{4-x}在x=1处展开，(x-1)无须处理
$$
$$逐项求导+逐项积分: \\
例：\arctan\frac{1-x}{1+x}展开为幂级数\qquad(\arctan\frac{1-x}{1+x})'=-\frac{1}{1+x^2}\\

\int_0^x-\frac{1}{1+x^2}dx=-\sum_{n=0}^{\infty}\int_0^x(-x^2)^n dx=\sum_{n=0}^{\infty}(-1)^n\frac{1}{2n+1}x^{2n+1}=\arctan\frac{1-x}{1+x}-\arctan1$$
$$凑已知和函数（求导、求积等）：\\
f(x)=\frac{1}{1+x},g(x)=\frac{x^2}{(1+x)^2}\\
g(x)=-x^2f'(x)=\cdots$$
$$拆函数展开等：\\
f(x)=\frac{1+x^2}{x}\arctan x=\frac{1}{x}\arctan x+x\arctan x$$
$$注：展开成x的幂级数，即在x=0处展开\\
注意补充收敛区间，取交集$$

# 空间解析几何

## 数量积、向量积、混合积

$$数量积：\textbf{a}\cdot\textbf{b}=|\textbf{a}|\cdot|\textbf{b}|\cos\theta$$
$$向量积：\textbf{a}\times \textbf{b}=
\left|
\begin{array}{ccc}
\textbf{i}&\textbf{j}&\textbf{k}\\
\\
a_1&a_2&a_3\\
\\
b_1&b_2&b_3
\end{array}
\right|\\
\ \\
|\textbf{a}\times\textbf{b}|=|\textbf{a}|\cdot|\textbf{b}|\cdot\sin(\widehat{\textbf{a},\textbf{b}})\quad （平行四边形面积）$$
$$混合积：[abc]=(a\times b)\cdot c=
\left|
\begin{array}{ccc}
a_x&a_y&a_z\\
\\
b_x&b_y&b_z\\
\\
c_x&c_y&c_z
\end{array}
\right|\quad（六面体体积）$$

## 垂直、平行的向量表示
$$\mathbf{s_1}=(m_1,n_1,p_1),\mathbf{s_2}=(m_2,n_2,p_2)$$

$$\mathbf{s_1}\parallel\mathbf{s_2}\Leftrightarrow \mathbf{s_1}\times\mathbf{s_2}=\mathbf{0}\Leftrightarrow \frac{m_1}{m_2}=\frac{n_1}{n_2}=\frac{p_1}{p_2}\\
$$
$$\mathbf{s_1}\perp\mathbf{s_2}\Leftrightarrow \mathbf{s_1}\cdot\mathbf{s_2}=m_1m_2+n_1n_2+p_1p_2=0$$

## 点到直线、平面距离

$$平面：d_{线}=\frac{|Ax_0+By_0+C|}{\sqrt{A^2+B^2}}\\
空间：d_{线}=\frac{|\textbf{s}\times \overrightarrow{MM_1}|}{|\textbf{s}|}\qquad点M_1(x_1,y_1,z_1)到直线L:\frac{x-x_0}{m}=\frac{y-y_0}{n}=\frac{z-z_0}{p}的距离$$
$$d_{面}=\frac{|Ax_0+By_0+Cz_0+D|}{\sqrt{A^2+B^2+C^2}}$$

## 直线方程的三种形式

$$点向式：\frac{x-x_0}{l}=\frac{y-y_0}{m}=\frac{z-z_0}{n}\\
参数式：\left\{
\begin{array}{l}
x=x_0+lt\\
y=y_0+mt\\
z=z_0+nt
\end{array}
\right.\\
两点式：\frac{x-x_1}{x_2-x_1}=\frac{y-y_1}{y_2-y_1}=\frac{z-z_1}{z_2-z_1}$$

## 平面方程的三种形式

$$一般式：Ax+By+Cz+D=0$$
$$点法式：A(x-x_0)+B(y-y_0)+C(z-z_0)=0$$
$$截距式：\frac{x}{a}+\frac{y}{b}+\frac{z}{c}=1$$

## 空间曲线的切线与法平面
参数方程、一般式方程

$$参数方程\left\{
\begin{array}{l}
x=\varphi(t)\\
y=\psi(t)\\
z=\omega(t)
\end{array}
\right.\\切向量:
\boldsymbol{\tau}=(\varphi'(t),\psi'(t),\omega'(t))\\
切平面:
\varphi'(t)(x-x_0)+\psi'(t)(y-y_0)+\omega'(t)(z-z_0)=0
$$

$$交面式方程\left\{
\begin{array}{l}
F(x,y,z)=0\\
G(x,y,z)=0
\end{array}
\right.\\
切向量：\boldsymbol{\tau}=\left|
\begin{array}{ccc}
\textbf{i}&\textbf{j}&\textbf{k}\\
F'_x& F'_y&F'_z\\
G'_x & G'_y&G'_z
\end{array}
\right|_{(x_0,y_0,z_0)}\quad （与空间直线方向向量同理）\\
切平面：......$$

## 空间曲面的法线与切平面

$$法向量：\textbf{n}=(F'_x,F'_y,F'_z)\big|_{(x_0,y_0.z_0)},\textbf{n}=(z'_x,z'_y,-1)或(-z'_x,-z'_y,1)\big|_{(x_0,y_0.z_0)}$$
$$法线：\frac{x-x_0}{F'_x(x_0,y_0,z_0)}=\frac{y-y_0}{F'_y(x_0,y_0,z_0)}=\frac{z-z_0}{F'_z(x_0,y_0,z_0)}$$
$$法平面：F'_x(x_0,y_0,z_0)(x-x_0)+F'_y(x_0,y_0,z_0)(y-y_0)+F'_z(x_0,y_0,z_0)(z-z_0)=0$$

## 梯度与方向导数

$$三元函数u=u(x,y,z)$$
$$梯度：\textbf{grad}\ u\bigg|_{P_0}=(u'_x,u'_y,u'_z)\big|_{P_0}$$
$$方向导数：\\
\frac{\partial u}{\partial \boldsymbol{l}}\bigg|_{P_0}=u'_x\cos\alpha+u'_y\cos\beta+u'_z\cos\gamma\big|_{P_0}=\boldsymbol{l^0}\cdot \textbf{grad}\ u\\
(\cos\alpha,\cos\beta,\cos\gamma)为方向\boldsymbol{l^0}的方向余弦\\
即梯度向量在单位方向向量\boldsymbol{l^0}上的投影$$
$$注：方向导数在与梯度同向时取得最大值$$

## 方向导数取最大值题型

**在某方向向量上取得最大方向导数，即梯度与方向向量同向**
$$f(x,y,z)=axy^2+byz+cx^3z^2在点P(1,2,-1)处沿z轴正向\boldsymbol{l}取得最大值$$
$$\textbf{grab}\ f=(f'_x,f'_y,f'_z)\big|_P=\lambda \boldsymbol{l}=\lambda(0,0,1)$$
**在某曲线（曲面）取得最大方向导数，即梯度取得最大值**
$$||\textbf{grab}\ f||的条件最值问题$$

## 梯度与等值线（面）的关系

$$z=x^2+y^2在(1,0)处的梯度方向（z数值由低到高）：\\
沿曲线x^2+y^2=1在(1,0)处的外法线方向（z越大，等值线越大）$$
$$u=4x^2+y^2+z^2-6在点M(1,1,1)的梯度方向：\\
沿曲面S：4x^2+y^2+z^2-6=0的外法线方向（u越大，等值面越大）$$
$$关键：函数u=F(x,y,z)的梯度是等值面F(x,y,z)=c的法向量（u增大方向）$$

## 场论公式
$$散度\text{div} A、旋度\textbf{rot\ A}$$

$$向量场(P(x,y,z),Q(x,y,z),R(x,y,z))$$
$$
\text{div}\ \textbf{A}=\frac{\partial P}{\partial x}+\frac{\partial Q}{\partial y}+\frac{\partial R}{\partial z}$$
$$\textbf{rot A}=
\left|
\begin{array}{}
\textbf{i}&\textbf{j}&\textbf{k}\\
\\
\frac{\partial}{\partial x}&\frac{\partial}{\partial y}&\frac{\partial}{\partial z}\\
\\
P&Q&R
\end{array}
\right|$$

## 平面束方程

$$直线L：
\left\{
\begin{array}{l}
x+y+2z+1=0\\
2x+4y+z-3=0
\end{array}
\right.\\
过直线L的所有平面可表示为（构成原直线的两平面不平行）：\\
x+y+2z+1+\lambda(2x+4y+z-3)=0\\
法向式原理：
(1+2\lambda,1+4\lambda,2+\lambda)与直线L垂直且任意，并作为平面法向量$$

## 空间直线方程的转化
$$一般方程\rightleftharpoons点向式方程、参数方程$$

**一般式转化：**
$$一般式方程\left\{
\begin{array}{l}
A_1x+B_1y+C_1z+D_1=0\\
A_2x+B_2y+C_2z+D_2=0
\end{array}
\right.\\
1. 叉乘确定向量\boldsymbol{\tau}=(A_1,B_1,C_1)\times(A_2,B_2,C_2)\\
2. 确定一个直线上的点(0,y_0,z_0)$$
**点向式、参数方程转化：**
$$点向式方程、参数方程\\
已知点P(x_0,y_0,z_0)，向量\boldsymbol{\tau}=(l,m,n)\\
任意两组等式
\left\{
\begin{array}{l}
\frac{x-x_0}{l}=\frac{y-y_0}{m}\\
\frac{y-y_0}{m}=\frac{z-z_0}{n}
\end{array}
\right.\Rightarrow
\left\{
\begin{array}{l}
m(x-x_0)-l(y-y_0)=0\\
n(y-y_0)-m(z-z_0)=0
\end{array}
\right.$$

## 平面曲线绕坐标轴旋转所得曲面（一般式）

**灵活利用此性质分析曲面形状**
$$坐标平面yOz中有曲线f(y,z)=0\\
绕z轴旋转:|y|=\sqrt{x^2+y^2}\rightarrow y=\pm\sqrt{x^2+y^2}\\
故f(\pm\sqrt{x^2+y^2},z)=0\\
z=y^2绕z轴旋转\rightarrow z=(\pm \sqrt{x^2+y^2})^2=x^2+y^2$$
$$注：
z=2-\sqrt{x^2+y^2}由z=2-y或z=2+y绕z轴转成\\
（针对z而言，y为正取\sqrt{x^2+y^2}，y为负取-\sqrt{x^2+y^2}）\\
$$

## 曲线绕坐标轴旋转所得曲面（参数方程）

**参数方程法**
$$例：
直线L的参数方程
\left\{
\begin{array}{l}
x=1\\
y=t\\
z=1+2t
\end{array}
\right.其上一点P(x_0,y_0,z_0)转至P(x, y, z)时，有\\
\left\{
\begin{array}{l}
x_0^2+y_0^2=x^2+y^2=1+t^2\\
z_0=z=2t+1（t反解代入）
\end{array}
\right.$$
$$注：空间中曲线的参数方程同理\\
坐标平面中直线的参数方程同理\quad xOy面y=x\quad
\left\{\begin{array}{l}
x=t\\
y=t\\
z=0
\end{array}\right.$$

# 多元函数积分学

## 考情分析

一元定积分、二重积分、三重积分求原函数的难度逐渐递减
两类曲线积分间、两类曲面积分间的转化灵活使用

## 方向余弦
$$\cos\alpha,\cos\beta,\cos\gamma$$

$$三元方程F(x,y,z)=0$$
$$
\textbf{n}=\frac{(F'_x,F'_y,F'_z)}{\sqrt{(F'_x)^2+(F'_y)^2+(F'_z)^2}}=\ \cos\alpha\ \textbf{i}+\cos\beta\ \textbf{j}+\cos\gamma\ \textbf{k}$$
$$\cos\alpha=\frac{F'_x}{\sqrt{(F'_x)^2+(F'_y)^2+(F'_z)^2}}\\
\cos\beta=\frac{F'_y}{\sqrt{(F'_x)^2+(F'_y)^2+(F'_z)^2}}\\
\cos\gamma=\frac{F'_z}{\sqrt{(F'_x)^2+(F'_y)^2+(F'_z)^2}}$$

## 二重积分定义式

**最多考区间 x,y∈(0,a)**
$$\lim\limits_{n\to \infty}\sum_{i=1}^{n}\sum_{j=1}^{n}f(\frac{ia}{n},\frac{jb}{n})\cdot\frac{ab}{n^2}=\int_0^a dx\int_0^b f(x,y)dy$$
$$\quad\lim\limits_{n\to \infty}\sum_{i=1}^{n}\sum_{j=1}^{n}\frac{2}{(\frac{ia}{n})^2+4(\frac{jb}{n})^2+2(\frac{ia}{n}+2\frac{jb}{n})+2}\cdot\frac{ab}{n^2}\\
=\int_0^adx\int_0^b\frac{2}{x^2+4y^2+2x+4y+2}dy\\
\ \\
\left\{
\begin{array}{ll}
\frac{ab}{n^2}\rightarrow dxdy\\
\\
\frac{ia}{n}\rightarrow x,
\frac{jb}{n}\rightarrow y
\end{array}
\right.$$
**变限积分：**
$$\lim\limits_{n\to \infty}\sum_{i=1}^{n}\sum_{j=1}^{i}f(\frac{i}{n},\frac{j}{n})\cdot\frac{1}{n^2}=\int_0^1 dx\int_0^x f(x,y)dy$$

## 极坐标转换

$$\left\{
\begin{array}{l}
x=r\cos\theta\\
y=r\sin\theta\\
d\sigma=rd\theta dr
\end{array}
\right.\qquad   \iint\limits_{D}
 f(x, y) \mathrm{d} \sigma= \iint\limits_{D}f(r \cos \theta, r \sin \theta) r d\theta dr$$
$$积分区域\left\{\begin{array}{rl}
(x-a)^2+y^2=a^2 &\leftrightarrow \rho=2a\cos \theta\\
(x-a)^2+(y-b)^2=a^2+b^2&\leftrightarrow \rho=2a\cos \theta+2b\sin\theta
\end{array}
\right.$$

## 球面坐标转换

$$\left\{
\begin{array}{l}
x=r\sin \varphi\cos\theta\\
y=r\sin \varphi\sin \theta\\
z=r\cos\varphi\\
dv=r^2\sin\varphi d\theta d\varphi dr
\end{array}
\right.\qquad \iiint\limits_{\Omega}f(x,y,z)dv=\iiint\limits_{\Omega}f(r\sin\varphi \cos\theta,r\sin\varphi \sin\theta, r\cos\varphi)r^2\sin\varphi d\theta d\varphi dr\\
\varphi\in(0,\pi)\quad \theta\in (0,2\pi)$$
$$\left\{
\begin{array}{l}
x=r\sin \varphi\cos\theta\\
y=r\sin \varphi\sin \theta\\
z=r\cos\varphi\\
dS=r^2\sin\varphi d\theta d\varphi
\end{array}\right.\qquad
\iint\limits_{\Sigma}f(x,y,z)dS=\iint f(r\sin\varphi \cos\theta,r\sin\varphi \sin\theta, r\cos\varphi)r^2\sin\varphi d\varphi d\theta$$
![](pic-advance-math\Markji_1751354432597.png)
$$积分区域\left\{\begin{array}{ll}
球面：x^2+y^2+z^2=4z&\leftrightarrow \rho=4\cos\varphi\\
锥面：
z=\sqrt{\frac{x^2+y^2}{3}}&\leftrightarrow \varphi=\frac{\pi}{3}
\end{array}
\right.$$

## 第二型曲面微元的正负问题

$$曲面微元
\left\{\begin{array}{l}
方向与坐标轴方向相同时，处理为dxdy\\
\ \\
方向与坐标轴方向不同，处理为-dxdy
\end{array}\right.
$$

## 两类曲面积分的关系

$$\textbf{n}=(\cos\alpha,\cos\beta,\cos\gamma)为有向曲面\textbf{S}在指定侧的单位法向量\\
\alpha,\beta,\gamma为\textbf{n}与x,y,z正向的夹角$$
$$\iint \limits_{\textbf{S}}Pdydz+Qdzdx+Rdxdy=\iint\limits_{S}(P\cos\alpha+Q\cos\beta+R\cos\gamma)dS\\
左式中曲面“方向”内含于有向曲面微元的“正负”中\\
右式中曲面“方向”内含于“方向余弦”中\\
$$

## 曲线微元转换公式

$$\frac{dx}{\cos\alpha}=\frac{dy}{\cos\beta}=ds\quad(\cos\alpha,\cos\beta)为曲线的单位切向量$$

## 曲面微元转换公式

$$dxdy、dydz、dzdx$$

$$\frac{dydz}{\cos\ \alpha}=\frac{dzdx}{\cos\ \beta}=\frac{dxdy}{\cos\ \gamma}=dS$$
$$有向曲面微元有正有负\\
“方向余弦”内含了“有向曲面微元的正负”
$$

## 格林公式

$$平面有界闭区域D由分段光滑曲线L围成，P(x,y),Q(x,y)在D上具有一阶连续偏导数，则$$
$$
\oint_{L}P(x,y)dx+Q(x,y)dy=\iint\limits_D(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y})d\sigma$$
$$L 取正向，即左手始终在 L 所围成区域 D 内；\quad
单连通、多连通（复连通）区域均成立$$
$$注：{\color{blue}边界奇点也应挖去}\\
挖奇点处理后，封闭曲线方向处理为外逆内顺（均在左手）\\
\oint\limits_{L+L_1}-\oint\limits_{L_1}\qquad或\qquad-\left[\oint\limits_{L^-+L_1}-\oint\limits_{L_1}\right]$$

## 高斯公式

$$空间有界闭区域\Omega由有向分片光滑封闭曲面\textbf{S}围成，P(x,y,z),Q(x,y,z),R(x,y,z)在\Omega上具有一阶连续偏导数，则$$
$$\oiint\limits_{\textbf{S}}Pdydz+Qdzdx+Rdxdy=\iiint\limits_{\Omega}(\frac{\partial P}{\partial x}+\frac{\partial Q}{\partial y}+\frac{\partial R}{\partial z})dv$$
$$\textbf{S}是\Omega的整个边界{\color{blue}曲面外围}；\quad 单连通、多连通（复连通）区域均成立$$
$$注：{\color{blue}边界奇点也应挖去}\\
挖奇点处理后，封闭曲面方向侧处理为外外内内\\
\oiint\limits_{\mathbf{S}+\mathbf{S_1}}-\oiint\limits_{\mathbf{S_1}}\qquad或\qquad-\left[\oiint\limits_{\mathbf{S^-}+\mathbf{S_1}}-\oiint\limits_{\mathbf{S_1}}\right]$$

## 斯托克斯公式

$$\Gamma为分段光滑的空间有向闭曲线，\textbf{S}为以\Gamma为边界的分片光滑有向曲面\\
P(x,y,z),Q(x,y,z),R(x,y,z)在包含曲面\textbf{S}的空间区域内有一阶连续偏导数，则$$
$$\begin{array}{r l}\oint_\Gamma P dx+Q dy +R dz=&
\iint\limits_{S}
\left|
\begin{array}{ccc}
\cos\alpha & \cos\beta & \cos\gamma\\
\\
\frac{\partial}{\partial x} & \frac{\partial}{\partial y} &
\frac{\partial}{\partial z} \\
\\
P & Q & R
\end{array}
\right|dS（第一型曲面积分）\\
\\
{\color{grey}=} & {\color{grey}\iint \limits_{\textbf{S}}
\left|
\begin{array}{ccc}
dydz & dzdx & dxdy\\
\\
\frac{\partial}{\partial x} & \frac{\partial}{\partial y} &
\frac{\partial}{\partial z} \\
\\
P & Q & R
\end{array}
\right|（第二型曲面积分）

}

\end{array}$$
$$\Gamma 方向与\Sigma法向量 成右手系$$
$$注：{\color{blue}边界奇点应挖去}\\
\oint_\Gamma P dx+Q dy +R dz=\iint\limits_{\textbf{S}}\text{rot}\ Fd\textbf{S}\\
斯托克斯公式为格林公式在空间中的推广$$

## 第一型线面积分、重积分的奇偶性

$$两要素判断
\left\{\begin{array}{l}积分区域对称\\
积分函数对称
\end{array}\right.$$
$$关于坐标轴\\
区域对称：1. 关于坐标轴对称
\ \ 2. 某变量变号，区域函数不变\\
函数对称：f(x,y,z)=\pm f(-x,y,z)\\
\ \\
关于原点\\
区域对称：1. 关于原点对称
\ \ 2. 两变量变号，区域函数不变\\
函数对称：f(x,y,z)=\pm f(-x,-y,z)$$
$$关于y=x\\
区域对称：1.关于y=x对称\ \ 2.\ x,y对换，区域函数不变\\
函数对称：f(x,y)=\pm f(y,x)$$
$$注：奇偶性勿固化于坐标轴的奇偶性，关于某点、某条直线也可以谈论奇偶性$$

## 第一型线面积分、重积分轮换对称性

**轮换对称性仅与积分区域有关**
$$判断方法：1. 关于直线或平面“y=x”对称\ \ 2.交换某两变量，积分区域不变$$
**若满足轮换对称性，对应积分变量间可任意对换（地位等同）**
$$\star f(x)\rightarrow f(y)\\
\star f(x,y,z)\rightarrow f(y,z,x)$$
$$函数处理：\iint\limits_{D_{xy}}f(x,y)dxdy=\iint\limits_{D_{xy}}f(y,x)dxdy=\frac{1}{2}\iint\limits_{D_{xy}} f(x,y)+f(y,x)dxdy\\
区间处理：\iint\limits_{D_{xy}}f(x,y)dxdy=\iint\limits_{D_1}f(x,y)+f(y,x)dxdy\qquad
D_{xy}=D_1+D_2（关于y=x对称）
$$
$$\begin{array}{ll}
\begin{array}{l}D为y=2-x与坐标轴围成区域\\
\iint\limits_{D}(x+3y)d\sigma=\iint\limits_{D}4yd\sigma
\end{array}
&
\begin{array}{l}
D为x+y+z=1与坐标轴围成区域\\
\iiint\limits_{\Omega}(x+2y+3z)dv=\iiint\limits_{\Omega}6zdv
\end{array}
\end{array}$$

## 第二型线面积分的奇偶性

$$三要素判断
\left\{\begin{array}{l}曲线、曲面对称性\\
曲线、曲面方向\\
奇偶性
\end{array}\right.$$
$$L=L_1+L_2关于x轴对称\\
L_1,L_2同向，有\int_LP(x,y)dx=
\left\{
\begin{array}{cl}
2\int_{L_1}P(x,y)dx,&P(x,y)关于y是偶函数\\
0,& P(x,y)关于y是奇函数\\
\end{array}
\right.\\
\ \\
L_1,L_2异向，有\int_LP(x,y)dx=
\left\{
\begin{array}{cl}
0,&P(x,y)关于y是偶函数\\
2\int_{L_1}P(x,y)dx,&P(x,y)关于y是奇函数\\
\end{array}
\right.$$
$$S=S_1+S_2关于xOy面对称\\
S_1取上侧，S_2取上侧，有\iint\limits_{\textbf{S}}R(x,y,z)dxdy=
\left\{
\begin{array}{cl}
0,&R(x,y,z)关于z为奇函数\\
2\iint\limits_{\mathbf{S_1}}R(x,y,z)dxdy,&R(x,y,z)关于z为偶函数
\end{array}
\right.\\
\ \\
S_1取上侧，S_2取下侧，有\iint\limits_{\textbf{S}}R(x,y,z)dxdy=
\left\{
\begin{array}{cl}
2\iint\limits_{\mathbf{S_1}}R(x,y,z)dxdy,&R(x,y,z)关于z为奇函数\\
0,&R(x,y,z)关于z为偶函数
\end{array}
\right.$$

## 第二型曲面积分重要结论

$$微元为零\left\{
\begin{array}{ll}曲线L为x=1,&\int_LP(x,y)dx=0\\
\ \\
曲面S为x^2+y^2=R^2,&\iint\limits_{\textbf{S}}P(x,y,z)dxdy=0（曲面在xOy面的投影为曲线）
\end{array}
\right.$$

## 极坐标交换积分次序

$$直接将r,\theta当作直角系变量，对应交换即可$$

## 常见曲面方程

![](pic-advance-math\Markji_1751354474017.png)
$$注：\frac{x^2}{a^2}-\frac{y^2}{b^2}=1为左右开口，\frac{y^2}{a^2}-\frac{x^2}{b^2}=1为上下开口\quad y=\pm \frac{b}{a}x为渐近线$$

## 曲面方程的坐标平移

$$整理为齐次的形式，坐标平移原则均为：负向加正向减\\
例：y^2+z^2=\frac{1}{4}(4-x)^2为-\frac{1}{4}(x-4)^2+y^2+z^2=0\\
xOy平面的直线y=2-\frac{1}{2}x，即y=\frac{1}{2}(4-x)绕x轴旋转形成的二次锥面\\

$$

## 二重积分交换积分次序问题

1. 交换积分次序，函数可积性不同

$$\int_0^{+\infty} dx\int_x^{2x} e^{-y^2}dy=\int_0^{+\infty} e^{-y^2}dy\int_\frac{y}{2}^ydx\\
\int_{-\infty}^{+\infty}dy\int_{-\infty}^{+\infty}e^{-2x^2+2xy-y^2}dx=\int_{-\infty}^{+\infty}e^{-x^2}dx\int_{-\infty}^{+\infty}e^{-(y-x)^2}d(y-x)$$
2. 交换积分次序，二重变限积分函数可导性不同
$$\int_0^tdx\int_x^t\sin\frac{x}{y}dy=\int_0^tdy\int_0^y\sin\frac{x}{y}dx$$
3. 交换积分次序，可简化二重积分计算（积分分段情形）

## 多元积分应用公式

$$质心、形心：\overline{x}=\frac{\iiint\limits_{\Omega}x\cdot\rho(x,y,z)dv}{\iiint\limits_{\Omega}\rho(x,y,z)dv}
;\qquad
\overline{x}=\frac{\iiint\limits_{\Omega}xdv}{\iiint\limits_{\Omega}dv}（形心的灵活反用是考察点）$$
$$转动惯量：I_x=\iiint\limits_{\Omega}(y^2+z^2)\rho(x,y,z)dv（绕x轴）
;\qquad
I_O=\iiint\limits_{\Omega}(x^2+y^2+z^2)\rho(x,y,z)dv（绕原点O）
$$
$$引力：
F_x=Gm\iiint\limits_{\Omega}\frac{\rho(x,y,z)(x-x_0)}{[(x-x_0)^2+(y-y_0)^2+(z-z_0)^2]^{\frac{3}{2}}}dv;\quad F_y;\quad F_z;\qquad (Gm\cdot \frac{M}{r^2}\cdot \frac{\Delta x}{r})
$$
$$注：\int_Lds,\quad\iint\limits_{D}d\sigma,\quad\iint\limits_{\Sigma}dS的质心、形心、转动惯量、引力对应换{\color{blue}积分形式}即可$$

## 三重积分计算

$$\left.\begin{array}{l}
切片法：\int dz\iint\limits_{D_z} d\sigma\\
竖线法：\iint\limits_{D_{xy}} d\sigma\int dz
\end{array}\right\}
柱坐标，即极坐标在三重积分中的灵活使用$$
$$球坐标法：特征较明显
\left\{\begin{array}{l}
积分区域为球、锥区域（便于确定积分限）\\
被积函数含x^2+y^2+z^2,\sqrt{x^2+y^2+z^2}等
\end{array}\right.$$
$$注：缺“\ ”先积“\ ”（缺两个，考虑先二后一）$$

## 第一型曲线积分计算
$$\int_Lf(x,y)ds$$
直角坐标、参数方程、极坐标

**第一型曲线积分由一元定积分推广而来**
**平面曲线（各坐标系下有各自的弧微分，并非由换元得到）：**
$$弧微分：\sqrt{(dx)^2+(dy)^2}\ ,\sqrt{[x'(t)]^2(dt)^2+[y'(t)]^2(dt)^2},\sqrt{[x'(\theta)]^2(d\theta)^2+[y'(\theta)]^2(d\theta)^2}\\
\sqrt{(dx)^2+(dy)^2}\not\xrightarrow {换元}\sqrt{[x'(t)]^2+[y'(t)]^2}\ dt\\
\ \\
\alpha,\beta上下限问题：曲线积分有特定的几何意义，保证弧长微元为正$$
$$直角坐标\ y=y(x)(a\leqslant x\leqslant b)\quad {\color{blue}（直角坐标形式x\to y\ 一对多，注意分段计算）}\\
\int_Lf(x,y)ds=\int_a^bf[x,y(x)]\sqrt{1+[y'(x)]^2}\ dx$$
$$参数方程\
\left\{
\begin{array}{l}
x=x(t)\\
y=y(t)
\end{array}
\right.
(\alpha\leqslant t \leqslant\beta)
\\
\int_Lf(x,y)ds=\int_\alpha^\beta f[x(t),y(t)]\sqrt{[x'(t)]^2+[y'(t)]^2}\ dt
$$
$$极坐标\ r=r(\theta)(\alpha\leqslant\theta\leqslant\beta)\\
\int_Lf(x,y)ds=\int_\alpha^\beta f[r(\theta)\cos\theta,r(\theta)\sin\theta]\sqrt{[r(\theta)]^2+[r'(\theta)]^2}\ d\theta$$
**空间曲线（遇见空间曲线，找参数方程，往一元转化）：**
$$参数方程\
\left\{
\begin{array}{l}
x=x(t)\\
y=y(t)\\
z=z(t)
\end{array}
\right.
(\alpha\leqslant t \leqslant\beta)
\\
\int_Lf(x,y,z)ds=\int_\alpha^\beta f[x(t),y(t),z(t)]\sqrt{[x'(t)]^2+[y'(t)]^2+[z'(t)]^2}dt$$
$$注：
善用参数方程简化曲线积分计算（曲面积分不可）\\
计算弧长，令f(x,y)或f(x,y,z)=1即可

$$

## 第一型曲面积分计算

$$\iint\limits_{S}f(x,y,z)dS$$

**第一型曲面积分由二重积分推广而来**
**（根据曲面表达式对应投影，若曲面投影重叠转换坐标系、或分片）**
$$z=z(x,y),(x,y)\in D_{xy}$$
$$\iint\limits_{S}f(x,y,z)dS=\iint\limits_{D_{xy}}f[x,y,z(x,y)]\sqrt{1+(z'_x)^2+(z'_y)^2}dxdy\\
\bigg(=\iint\limits_{S}f(x,y,z(x,y))\frac{dxdy}{\cos\gamma}=\iint\limits_{S}f(x,y,z(x,y))\frac{dxdy}{\frac{1}{\sqrt{1+(z'_x)^2+(z'_y)^2}}}=\iint\limits_{D_{xy}}f[x,y,z(x,y)]\sqrt{1+(z'_x)^2+(z'_y)^2}dxdy\bigg)$$
$$第一型曲面积分的曲面微元方向与z轴正向一致$$

## 平面曲线积分与路径无关定理

$$D是平面上的{\color{blue}单连通}区域，P(x,y),Q(x,y)在D上有{\color{blue}一阶连续偏导数}，则\\
\ \\
\quad\ \int_LPdx+Qdy的值在D内与路径无关\\
\Leftrightarrow 对任何D内的光滑闭曲线，有\oint_LPdx+Qdy=0\\
\Leftrightarrow 存在u(x,y)，使得du(x,y)=Pdx+Qdy\\
{\color{blue}\Leftrightarrow}\ 在D内，\frac{\partial Q}{\partial x}=\frac{\partial P}{\partial y}（复连通区域无法证明与路径无关,格林公式\oint_{L}=\oint_{L+l^-}+\oint_{l}）\\
（若不满足一阶连续偏导，\frac{\partial Q}{\partial x}=\frac{\partial P}{\partial y}无法证明与路径无关）$$
$$注：\\
1. du(x,y)=Pdx+Qdy证积分与路径无关\quad u(a,b)-u(0,0)\\
f(u)连续，f(x^2+y^2)(xdx+ydy)=\frac{1}{2}f(x^2+y^2)d(x^2+y^2)=d[\frac{1}{2}F(x^2+y^2)]\\
2. 一阶连续偏导，复连通区域，将积分曲线统一到“洞”的一侧即与轨迹无关，即单连通$$

## 空间曲线积分与路径无关

$$\Omega 是空间中的{\color{blue}单连通}区域，P(x,y,z),Q(x,y,z),R(x,y,z)在\Omega上有{\color{blue}一阶连续偏导数}，则\\
\ \\
\quad\int_{L}Pdx+Qdy+Rdz的值在\Omega中与路径无关\\
\Leftrightarrow 对任何\Omega内的光滑闭曲线，有\oint_LPdx+Qdy+Rdz=0\\
\Leftrightarrow 存在u(x,y,z)，使得du(x,y,z)=Pdx+Qdy+Qdz\\
{\color{blue}\Leftrightarrow}\  \text{rot} F=0（无旋场），即在\Omega内\frac{\partial Q}{\partial x}=\frac{\partial P}{\partial y},\frac{\partial Q}{\partial z}=\frac{\partial R}{\partial y},\frac{\partial R}{\partial x}=\frac{\partial P}{\partial z}$$

## 第二型曲线积分计算方法
$$\int_L P(x,y)dx+Q(x,y)dy$$
变量消元法、格林公式法、积分与路径无关

**变量消元法（与投影法本质相同）：**
$$ 直角坐标y=y(x)（a\rightarrow b）{\color{blue}（直角坐标x\to y\  一对多，注意分段）}\\
\int_L P(x,y)dx+Q(x,y)dy=\int_a^b \{P[x,y(x)]+Q[x,y(x)]y'(x)\}dx\\
参数方程
\left\{
\begin{array}{l}
x=x(t)\\
y=y(t)
\end{array}
\right.（\alpha\rightarrow\beta）\\
\int_LP(x,y)dx+Q(x,y)dy=\int_\alpha^\beta \{P[x(t),y(t)]x'(t)+Q[x(t),y(t)]y'(t)\}dt
$$
**格林公式法：**
$$补边情形：非封闭曲线\\
挖点情形：积分区域内包含被积函数的无定义点，\\
取L为有向封闭曲线x^2+\frac{y^2}{4}=\delta^2，{\color{blue}消去无定义点}，即\left\{\begin{array}{l}x=\delta\cos\theta\\
y=2\delta\sin\theta \end{array} \right.$$
**积分与路径无关：**
$$简单路径计算（直线、折线等）\\
复杂函数考虑拆函数，构造积分与路径无关\\
\int_L[f(y)e^x-3y]dx+[f'(y)e^x-3]dy=\int_{\hat{L}}f(y)e^xdx+f'(y)e^xdy-3\int_Lydx+dy$$
$$注：善用参数方程简化曲线积分计算（曲面积分不可）$$

## 第二型曲面积分计算方法
$$\iint\limits_{\textbf{S}}P(x,y,z)dydz+Q(x,y,z)dzdx+R(x,y,z)dxdy$$
投影代换法、高斯公式法

**向第一型曲面积分转换时，切记“方向侧”对应，注意曲面的投影重叠**
**投影代换法：**
$$原始消元：变量消元法，对应代入，积分区域投影即可\\
\iint\limits_{\textbf{S}}P(x,y,z)dydz=\pm\iint\limits_{D_{yz}}P[x(y,z),y,z]dydz\\
\quad \textbf{S}指定侧与x轴正向同向取“+”，异向取“-”\\
\quad ......\\
\ \\
统一微元：利用曲面微分转换投影公式，将积分统一于同一微元下\\
\iint\limits_{\textbf{S}}P(x,y,z(x,y))\frac{\cos\alpha}{\cos\gamma}dxdy+Q(x,y,z(x,y))\frac{\cos\beta}{\cos\gamma}dxdy+R(x,y,z(x,y))dxdy$$
**高斯公式法：**
$$补面情形：非封闭曲面\\
挖点情形：积分区域包含被积函数的无定义点,\\
取\textbf{S}为有向封闭曲面x^2+y^2+z^2=\delta^2，{\color{blue}消去无定义点}$$

## 第二型空间曲线积分计算方法
变量消元法、斯托克斯公式法

**变量消元法（与投影法本质相同）：**变量消元法，对应代入，积分区域投影即可
$$参数方程
\left\{
\begin{array}{l}
x=x(t)\\
y=y(t)\\
z=z(t)
\end{array}
\right.（\alpha\rightarrow\beta）\\
\quad\ \int_LP(x,y,z)dx+Q(x,y,z)dy+R(x,y,z)dz\\
=\int_\alpha^\beta \{P[x(t),y(t),z(t)]x'(t)+Q[x(t),y(t),z(t)]y'(t)+R[x(t),y(t),z(t)]z'(t)\}dt$$
$$一般方程
\left\{
\begin{array}{l}
x^2+y^2=1\\
z=x+y+1 \quad\textcircled{1}
\end{array}
\right.\\
式\textcircled{1}代入，化为第二型平面曲线积分(dz=dx+dy)
$$
**斯托克斯公式法（封闭曲线）：**
$$补边情形：非封闭曲线\\
挖点情形：灵活选择斯托克斯公式转化后的积分曲面$$
**积分与路径无关：**
$$更换积分路径（折线、直线）$$

## 线面积分的奇点讨论

$$考研从未出现过怪异奇点，主要为原点，即\frac{1}{x^2+y^2},\frac{1}{x^2+y^2+z^2}\\
无需担心奇点不可消去问题，遇到奇点情形，首先考虑曲线、曲面方程消去奇点，再择简便方法$$

## 多元函数积分重要经验

1. 重积分、第一类曲线曲面积分需灵活使用奇偶性、轮换对称性
第二型线面积分灵活使用奇偶性
2. 线、面积分的线、面方程均可代入被积函数化简，但重积分不可
3. 考虑交换积分次序问题
4. 注意积分方向问题，容易掉进陷阱
5. 坐标系转换**谨记**微元对应

## 二重积分换元法

**换元仅可换一维**
$$\qquad\quad\int_{-1}^0dx\int_{-1-x}^{1+x}f(x+y)dy+\int_0^1dx\int_{x-1}^{1-x}f(x+y)dy\\
\xlongequal{x+y=u}\int_{-1}^0dx\int_{-1}^{1+2x}f(u)du+\int_0^1dx\int_{2x-1}^1f(u)du\\
\xlongequal{交换积分次序}\int_{-1}^1du\int_{\frac{u-1}{2}}^{\frac{u+1}{2}}f(u)dx=\int_{-1}^1f(u)du
$$

## 二重积分参数方程代入方法

**先处理为定积分，再作换元（重积分无法直接代入）**
$$D为摆线\left\{
\begin{array}{l}
x=a(t-\sin t)\\
y=a(1-\cos t)\\
(0\leqslant t\leqslant 2\pi)
\end{array}
\right.与x轴围成，计算I=\iint\limits_{D_{xy}}y^2dxdy\\
x'(t)=a(1-\cos t)>0，故存在反函数t=t(x)\\
D=\{(x,y)|0\leqslant x\leqslant 2\pi a,0\leqslant y\leqslant y[t(x)]\}\\
I=\int_0^{2\pi a}dx\int_0^{y[t(x)]}y^2dy=\int_0^{2\pi a}\frac{1}{3}y^3[t(x)]dx\\
\xlongequal{x=a(t-\sin t)}\int_0^{2\pi }\frac{1}{3}y^3(t)a(1-\cos t)dt=\cdots$$

## 二重积分分部积分消“偏导数”

$$f(x,1)=a,f(1,y)=b,\iint\limits_{D}xyf_{xy}''(x,y)dxdy\\
\rightarrow 累次积分\\
\rightarrow 对x分部积分\\
\rightarrow 交换积分次序\\
\rightarrow 对y分部积分$$

## 重积分“特殊被积函数”处理技巧

$$\iint\limits_{D}|x^2+y^2-2y|d\sigma\\
x^2+y^2-2y=0为分界线
$$
$$\iint\limits_{D}\max\{2x-y,1\}d\sigma\\
2x-y=1为分界线$$

## 曲线的参数方程转化

**圆、椭圆的参数方程转化（空间曲线无法参数化）：**
$$\begin{array}{ccccc}
(\frac{x}{2})^2&+&(\frac{y}{3})^2&=2\\
\downarrow&&\downarrow\\
\sqrt{2}\sin t&&\sqrt{2}\cos t
\end{array}$$
**直线的参数方程转化：**
$$\frac{x-x_1}{x_2-x_1}=\frac{y-y_1}{y_2-y_1}=\frac{z-z_1}{z_2-z_1}=t$$

## 直角坐标与极坐标灵活转换情形

$$\iint\limits_{D}r^2\sin\theta\sqrt{1-r^2\cos2\theta}drd\theta,\quad D=\{(r,\theta)|0\leqslant r\leqslant \sec\theta, 0\leqslant \theta\leqslant \frac{\pi}{4}\}\\

\Rightarrow \iint\limits_{D}y\sqrt{1-x^2+y^2}dxdy, \qquad D=\{(x,y)|0<y<x,0<x<1\}\\
=\frac{1}{2}\int_0^1dx\int_0^x\sqrt{1-x^2+y^2}\ d\mathbf{(1-x^2+y^2)}$$

## 特殊圆锥体

$$x^2+(y-z)^2=(1-z)^2\quad 代入不同z，方程表示不同z处的圆\\
任意锥体体积V_{锥}=\frac{1}{3}Sh$$

# 横向知识点对比

极限、级数、反常积分收敛对比

**子极限自变量趋向速度不一致**
$$\begin{array}{lll}\lim\limits_{x\to \infty}f(x)+\lim\limits_{x\to \infty}g(x)&& \lim\limits_{x\to \infty}[f(x)+g(x)]&（收+收=收，收+发=发，发+发=不一定）\\
\\
\sum_{n=1}^\infty a_n+\sum_{n=1}^\infty b_n&&\sum_{n=1}^\infty (a_n+b_n)&（收+收=收，收+发=发，发+发=不一定）\\
\\
\lim\limits_{x\to 0^-}\int_{-1}^x\frac{1}{x}dx+\lim\limits_{x\to 0^+}\int_{x}^{1}\frac{1}{x}dx&& \int_{-1}^1\frac{1}{x}dx（规定趋向方式不统一）&（收+收=收，收+发=发，发+发=发）
\end{array}$$

# 备用知识点

## 特殊题型（反证）
$$\int_0^1 xf(x)dx=\int_0^1f(x)dx,证\int_0^\xi f(t)dt=0$$

$$对\int_0^xf(t)dt用零点定理：$$
$$设\int_0^xf(t)dt恒正或恒负\\
\int _0^1(x-1)f(x)dx=\int_0^1(x-1)d(\int_0^xf(t)dx)=\\(x-1)\int_0^xf(t)dt\bigg|_0^1-\int_0^1(\int_0^xf(t)dt)dx<0\\
与题不符，故\int_0^xf(t)dt不可能恒正或恒负$$

## 变限积分函数周期性证明
$$\int_0^x f(t)dt \ \ \ \ T\Longrightarrow f(x)\ \ \  T  \quad 且 \quad \int_0^T f(x)dx=0 $$

$$\begin{array}{ll}
\begin{array}{rl}
&\int_0^x f(t)dt \ \ \ \ T\\
\\
\Rightarrow & \int_0^x f(t)dt =\int_0^{x+T} f(t)dt \\
\\
\Rightarrow & \int_x^{x+T} f(t)dt=0\\
\\
即&\ \int_0^Tf(x)dx=0
 \end{array}

&

\begin{array}{rl}
&\int_0^xf(t)dt\\
\\
\xlongequal{t+T=u}&\int_{T}^{T+x}f(u-T)du\\
\\
=& \int_0^{x}f(u-T)du+\int_x^{x+T}f(u-T)du-\int_0^Tf(u-T)du\\
\\
=& \int_0^xf(u-T)du\\
\\即&\ \int_0^xf(t)-f(t-T)dt\equiv 0\\
故&\ f(t)\equiv f(t-T)
\end{array}
\end{array}$$

## 特殊反常积分

狄利克雷积分：
$$\int _0^{+\infty}\frac{\sin x}{x}dx=\frac{\pi}{2}$$

## 变量分离的两边积分法解释

$$已知有微分方程：g(y)dy=f(x)dx\quad(1)\\
假设g(y),f(x)连续，设y=\varphi(x)为方程的解\\
代入(1)式得：\\
\quad \quad \quad g[\varphi(x)]\varphi'(x)dx=f(x)dx\\
可知：\quad g[\varphi(x)]\varphi'(x)=f(x)\\
同时对等式两边积分：\\
\quad \quad \quad \int g(y)dy=\int f(x)dx\\
\quad \quad 即\ G(y)=F(x)+C\quad (2)\\
\quad \quad \quad y=\varphi(x)满足(2)式\\

(G(y))'=(F(x)+C)'\Rightarrow g(y)\frac{dy}{dx}=f(x)\\
\quad\quad\quad故(2)式满足(1)式\\
\quad即(2)式为隐式解且为所有解
$$

# 备用方法

## 高阶非常系数线性齐次微分方程求解题型

**此类方法极其特殊，针对性极强**
$$y_1=\frac{\sin x}{x}为微分方程xy''+2y'+xy=0的一个解，求通解\\
令\frac{y_2}{y_1}=u(x),即y_2=u(x)\cdot\frac{\sin x}{x}是原方程的解，带入求解即可$$

# 待整理问题

无条件极值的失效情形

## 多元积分的考查尺度

考查尺度有限，不如体系铺展得复杂，梳理轻重点

## 数学整体的考情复核
