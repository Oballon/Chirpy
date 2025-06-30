高等数学

高数知识量很大，理解相较容易，但灵活性较高       总结必要的概念、结论、方法、经验、典例等，仅为知识体系，不覆盖做题分析能力（灵活使用，掌握足够的技巧方法，面对题目“非无之无”）考试面前，适当理解以对抗风险，但应用为先！

### 默认章节

考情分析
---
选择题：4道
填空题：4道
大题：4道

考查轻重点讨论
---
1. 数列极限证明题：中上上难度
2. 中值定理证明题：中上上难度
3. 微分方程：中等难度
4. 不定积分：中上难度
5. 数项级数：中上难度



重要技巧（解题技巧 > 计算方法）
---
1. 指数化与对数化（解函数，极限，求导）（应用空间不尽相同）
$$\Delta=e^{\ln\Delta}\quad （可能影响定义域）\\
\Delta=\ln e^\Delta$$
2. 特值法
选择题善用



### 重要概念补充

系数对应问题注意
---
$$\quad \ ax+by=x+y（即\forall x,y）\\
\Leftrightarrow a,b=1$$
$$\quad \ \xi a+\mu b=a+b（对特定的a,b,有特定的\xi,\mu）\\
\not\Leftrightarrow \xi,\mu=1$$



去绝对值问题
---
$$因变量去绝对值，要加“\pm”$$
$$自变量去绝对值，
应分类讨论$$



易失误问题
---
**约分问题：**
$$\Delta=\alpha\Delta（须分类讨论\Delta=0）\\
\Delta\neq0,则\alpha=1\\
\Delta=0,则\alpha未知$$



变量代换求函数问题
---
**注意代换回原变量**
$$f[\varphi(t)]\neq f(t)\\
f[\varphi(t)]\xlongequal{t=\varphi^{-1}(x)}f[\varphi(\varphi^{-1}(x))]=f(x)$$



### 预备知识

泰勒展开
$$ e^x, a^x,\ln(1+x) $$

$$\frac{1}{1+x} , \frac{1}{1-x}$$

$$\sin x,  \cos x,  \arctan x$$

$$(1+x)^\alpha$$

$$\tan x,  \arcsin x $$

---

$$\begin{array}{l}
x_0=0,x\to0时\\
\\
\mathrm{e}^x=1+x+\frac{x^2}{2!}+ \cdots+ \frac{x^n}{n !}+\circ(x^n)\\
\\
\mathrm{a}^x=e^{x\ln a}=1+x\ln a+\frac{(x\ln a)^2}{2!}+ \cdots+ \frac{(x\ln a)^n}{n !}+\circ(x^n)\\
\ln (1+x)=x-\frac{x^2}{2}+\frac{x^3}{3}-\cdots+\frac{(-1)^{n-1} x^n}{n}+\circ(x^n) \\
\\
\frac{1}{1+x}=1-x+x^2-\cdots+(-1)^n x^n+\circ(x^n)\\
\\
\frac{1}{1-x}=1+x+x^2+\cdots+ x^n+\circ(x^n)\\
\\
\sin x = x - \frac{x^3}{3!} + \frac{x^5}{5!} - \cdots +\frac{(-1)^n}{(2n+1)!} x^{2n+1} +\circ(x^{2n+1})\\
\\
\cos x =1 - \frac{x^2}{2!} + \frac{x^4}{4!} - \cdots +  \frac{(-1)^n}{(2n)!} x^{2n}+\circ(x^{2n})\\
\\
\arctan x =x-\frac{x^3}{3} + \frac{x^5}{5}-\cdots +\frac{(-1)^n}{2n+1} x^{2n+1}+\circ(x^{2n+1})\\
\\
(1+x)^\alpha=1+\alpha x+ \frac{\alpha(\alpha-1)}{2!}x^2+\cdots+\circ(x^{n})\quad {\color{blue}（\alpha为任意常数，此式可无限展开）}
\end{array}$$
**记前两项**
$$\begin{array}{l}
\tan x=x+\frac{x^3}{3}+\frac{2 x^5}{15}+\cdots+\frac{B_{2n}(-4)^n\left(1-4^n\right)}{(2n)!}x^{2n-1}+\circ(x^{2n-1}) 
\\
\arcsin x=x+\frac{x^3}{6}+\frac{3x^5}{40}+\cdots\frac{(2n)!}{4^n(n!)^2(2n+1)}x^{2n+1}+\circ(x^{2n+1})
\end{array}$$

数列重要公式
等差、等比求和
$$1^2+2^2+3^3+\cdots+n^2$$
---
$$S_n=\frac{n(a_1+a_n)}{2}$$
$$S_n=\frac{a_1(1-q^n)}{1-q}$$
$$1^2+2^2+3^3+\cdots+n^2=\frac{n(n+1)(2n+1)}{6}$$



三角函数常用公式
$$(\sin^2x,\cos^2x),(\tan^2x, \sec^2x), (\cot^2x, \csc^2x) $$
$$\sin2\alpha, \cos2\alpha$$
$$\sin(\alpha\pm \beta), \cos(\alpha\pm \beta), \tan(\alpha\pm \beta)$$
---
$$\begin{array}{lll}
\sin^2x+\cos^2x=1 & 1+\tan^2x=\sec^2x & 1+\cot^2x=\csc^2x \\
\\
\sin2\alpha=2\sin\alpha \cos\alpha
&\cos2\alpha=\cos^2\alpha-\sin^2\alpha=2\cos^2\alpha-1=1-2\sin^2\alpha \\
\\
\sin(\alpha\pm \beta)=\sin\alpha \cos\beta\pm \cos\alpha \sin\beta &
\cos(\alpha\pm \beta)=\cos\alpha  \cos\beta \mp \sin\alpha \sin\beta & \tan(\alpha\pm \beta)=\frac{\tan\alpha\pm \tan\beta}{1\mp \tan\alpha \tan\beta}
\end{array}$$