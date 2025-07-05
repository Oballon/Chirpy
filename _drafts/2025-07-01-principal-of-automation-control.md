自动控制原理知识点很多，但出题相对固定；控制理论的诸多不完整、不严谨的使用与方法姑且用着，以后有需要再作考量；801控制原理的考察范围不完全明晰，视为风险的一部分；     总结必要的概念、结论、方法、经验、典例等，仅为知识体系，不覆盖做题分析能力（灵活使用，掌握足够的技巧方法，面对题目“非无之无”）考试面前，适当理解以对抗风险，但应用为先！

# 默认章节

## 考情分析

考察点主要在控制理论，电路，电机，模电等知识点涉及不深

## 常见函数拉氏变换

$$\delta(t),\delta(t-\tau_0), 1(t), t, \frac{t^n}{n!}, e^{\pm at}, \sin\omega t, \cos\omega t$$

$$\begin{array}{}
f(t)& F(s)\\
\delta(t) & 1 \\
\delta(t-\tau_0) & e^{-\tau_0s} \\
\ \\
1(t) & \frac{1}{s} \\
\ \\
t & \frac{1}{s^2} \\
\ \\
\frac{t^n}{n!} &\frac{1}{s^{n+1}}\\
\ \\
e^{\pm at} & \frac{1}{s\mp a}\\
\ \\
\sin{\omega t} & \frac{\omega}{s^2+\omega^2}\\
\ \\
\cos{\omega t} & \frac{s}{s^2+\omega^2}

\end{array}$$

## 留数法(单根，重根)

$$单根：\frac{c_i}{s-p_i}\\
c_i=\lim\limits_{s\to p_i}[(s-p_i)F(s)]
$$
$$重根：\frac{c_m}{(s-p_1)^m},\frac{c_{m-1}}{(s-p_1)^{m-1}},\cdots\\
c_m=\lim\limits_{s\to p_1}[(s-p_1)^m F(s)] \\
c_{m-1}=\frac{1}{1!}\cdot\lim\limits_{s\to p_1}\frac{\mathrm{d}}{\mathrm{d}s}[(s-p_1)^{m} F(s)]  \\
c_{m-2}=\frac{1}{2!} \cdot\lim\limits_{s\to p_1}\frac{\mathrm{d^2}}{\mathrm{d}s^2}[(s-p_1)^{m} F(s)] \\
\cdots
$$

## 拉氏变换基本定理

线性性质、微分定理、积分定理、实位移定理、复位移定理、初值定理、终值定理

$$\mathscr{L}[af_1(t) \pm bf_2(t)]=aF_1(s) \pm bF_2(s)$$
$$\left\{
\begin{array}{l}
 \mathscr{L}[f^{(n)}(t)]=s^nF(s)（零初始条件）\qquad \mathscr{L}[f^{\prime}(t)]=sF(s)-f(0) \\

\mathscr{L}[f^{(n)}(t)]=s^nF(s)-s^{n-1}f(0)-s^{n-2}f^{\prime}(0)-\cdots -sf^{(n-2)}(0)-f^{(n-1)}(0)

\end{array}
\right.$$
$${\color{grey}

\left\{
\begin{array}{l}
\mathscr{L}[{\underbrace{\int \cdots \int}_n} f(t)(dt)^n]=\frac{1}{s^n}F(s)（零初始条件）\qquad \mathscr{L}[\int f(t)dt]=\frac{1}{s}F(s)+\frac{1}{s}f^{(-1)}(0)\\

\mathscr{L}[{\underbrace{\int \cdots \int}_n} f(t)(dt)^n]=\frac{1}{s^n}F(s)+\frac{1}{s^n}f^{(-1)}(0)+\frac{1}{s^{n-1}}f^{(-2)}(0)+\cdots +\frac{1}{s}f^{(-n)}(0)
\end{array}
\right.\qquad （不考）

}$$
$$\mathscr{L}[f(t \pm \tau_0)]=e^{\pm \tau_0s}F(s)\qquad注： \mathscr{L}[f'(t\pm \tau_0)]\xlongequal[g(t)=f(t\pm \tau_0)]{g(t)=f'(t)}e^{\pm \tau_0s}sF(s)\\

\mathscr{L}[e^{\mp At}f(t)]=F(s\pm A)\qquad 注：\mathscr{L}[e^{\mp At}f'(t)]\xlongequal{g(t)=f'(t)}G(s\pm A)=(s\pm A)F(s\pm A)$$
$$\lim\limits_{t\to0}f(t)=\lim\limits_{s\to \infty}s\cdot F(s)\\

\lim\limits_{t\to \infty}f(t)=\lim\limits_{s\to 0}s\cdot F(s)$$

# 数学建模

## 考情分析

简单电路网络，简单力学系统，机电系统（会预给公式）的建模
计算传递函数：微分方程整理，框图化简

## 电气网络

$$\begin{array}{}电阻：u_R=R\ i_R&
电容：i_C=C\frac{du_C}{dt}&
电感：u_L=L\frac{di_L}{dt}\\
&I(s)=CsU(s)&U(s)=LsI(s)\\
Z_R=R & Z_C=\frac{1}{Cs} & Z_L=Ls

\end{array}$$
$$\begin{array}{l}串联分压：U_1=\frac{Z_1}{Z_1+Z_2}U & U_2=\frac{Z_2}{Z_1+Z_2}U & I=\frac{1}{Z_1+Z_2}U\\
 \ \\
并联分流：I_1=\frac{Z_2}{Z_1+Z_2}I & I_2=\frac{Z_1}{Z_1+Z_2}I & U=\frac{Z_1Z_2}{Z_1+Z_2}I

\end{array}$$
$$运算放大器（正负极口）：u_+=u_-\quad i_+=i_-=0$$
$$并联阻抗Z=\frac{Z_1Z_2}{Z_1+Z_2}\quad容阻并联Z=\frac{R}{sRC+1}$$

## 力学系统公式及技巧

$$\begin{array}{cl}
牛顿第二定律：&f=ma\\
阻尼器：&f=Bv=B\frac{dy(t)}{dt}\\
弹簧：&f=ky(t)\\
转矩：&T=J\frac{d\omega}{dt}=J\frac{d\Omega}{dt}=J\frac{d^2\theta}{dt^2}\quad(\omega,\Omega均为角速度)\\
&T=rF\sin\theta（0<\theta<\frac{\pi}{2}）\\
粘性摩擦力矩：&T_B=k\omega=k\frac{d\theta}{dt}
\end{array}$$
$$技巧：\\
注意区分“力的传递”\ \ “力的分担”\ \ “力的余额”\\
传递：一端施力，中间各段受力相等\\
分担：中间施力，施点两侧为分担；\quad 或并联结构\\
余额（非阻力）：物块加速度的力$$

## 机电系统

**初步认定，电机系统不考查原理（题目会提供）**

## 微分方程列写技巧及注意

$$须将体现所有部件的微分方程列写完整$$

## 方框图绘制注意

$$前馈上面画，反馈下面画$$

## 梅森增益公式

$$G(s)=\frac{\sum_{k=1}^np_k\Delta_k}{\Delta}\\
\Delta=1-\sum L_a+\sum L_bL_c-\sum L_dL_eL_f+\cdots\quad （互不接触的回路增益乘积之和）\\
p_k：第k条前向通路总增益\\
\Delta_k：\Delta中与第k条前向通路接触的回路增益置0（或在方框图中去掉）$$
$$注：（考查不会太复杂）\\
\left\{\begin{array}{l}
前向通路、回路均不可包含{\color{blue}重复点，重复段}（点接触视为接触）\\
前向通路不可包含回路\\
输入前馈无法形成回路，单独两回路也无法形成回路
\end{array}\right.\\
\ \\
\left\{\begin{array}{l}
信号流图中比较点、引出点合并默认易有歧义\\
若同质的两点间增益为1，应视作一个点；非同质的两点间增益为1，不宜合并（易有歧义）
\end{array}\right.\\

\ \\
注意变量定义位置，勿固化（R(s),E(s),C(s)）\\
{\color{blue}多输入多输出系统同理，特征式一致，分子对应输入、输出间列写即可}\\
$$

## 梅森增益公式难点与技巧

$$难点：前向通路与回路结合\\
交叉型\left\{
\begin{array}{l}
一回路“包含”两前向交叉区域，且不“大于”前向联合区域\Rightarrow 三者可结合形成前向通路\\
一前向“包含”两回路交叉区域，且不“大于”回路联合区域\Rightarrow 三者可结合形成回路
\end{array}
\right.\\
小结论：\\
回路“包含”前向通路\Leftrightarrow两者可结合形成回路$$
$$技巧：规范列写各回路(L_1,L_2,\cdots,L_1L_2\cdots)\\
方框图求传函，基本只用梅森增益公式\\
\left\{\begin{array}{l}

使用框图化简出现分式时，计算量偏大\\
灵活使用框图预处理，简化计算
\end{array}\right.
$$

## 传递函数的性质

$$\Phi(s)=\frac{G_1(s)}{1+G_1(s)H(s)}\quad（反馈相加点取“-”）\\
开环传函:G_1(s)H(s)\quad （与反馈口“正负”无关）\\
传递函数：{\color{blue}零初始条件下的\frac{C(s)}{R(s)}}$$
$$\Phi(s)=1-\Phi_e(z)前提：无输入前馈，输入无传函，且整体为单位负反馈$$
$$同一框图下\Phi(s)、\Phi_e(s)、多输入多输出等的特征式\Delta相同，但特征多项式D(s)不一定相同\\
注：若无零极点对消，则D(s)相同；\Phi(s)输出稳定\neq \Phi_e(s)误差稳定\neq\cdots$$
$$注：G(s)=\frac{M(s)}{N(s)}\quad 对实际物理系统来说，M(s)阶次\leqslant N(s)阶次$$

## 方框图化简“8字型”（重难点）

$$\left\{
\begin{array}{}
C_1=H_1(E-C_2)\quad\textcircled{1}\\
C_2=H_2(E-C_1)\quad\textcircled{2}
\end{array}
\right.\rightarrow\left\{
\begin{array}{}
H_2C_1=H_1H_2(E-C_2)\quad\textcircled{3}\\
H_1C_2=H_1H_2(E-C_1)\quad \textcircled{4}
\end{array}
\right.\\
\textcircled{3}+\textcircled{4}:\\
H_1C_2+H_2C_1=2EH_1H_2-H_1H_2(C_1+C_2)\\
\textcircled{1},\textcircled{2}代入上式:\\
H_1E-C_1+H_2E-C_2=2EH_1H_2-H_1H_2(C_1+C_2)\\
(H_1+H_2)E-(C_1+C_2)=2EH_1H_2-H_1H_2(C_1+C_2)\\
\frac{C_1+C_2}{E}=\frac{H_1+H_2-2H_1H_2}{1-H_1H_2}$$

## 变量间传递函数问题

$$根据变量关系消元整理（微分方程、拉氏方程）\\
若只求传递函数，直接列写拉氏方程
$$
$$注：方框图起不到辅助作用$$

## 电路网络典例

<img src=pic-principal-of-automation-control\Markji_1751374229141.png width="39%"><img src=pic-principal-of-automation-control\Markji_1751374241740.png width="60%">
$$灵活使用多路并联分流公式\\
注意：并联支路，负载效应$$

## 力学系统典例

![](pic-principal-of-automation-control\Markji_1751374277110.png)
$$小结论（化简时直接写）：本质与分压、分流相反\\
Y_0=\frac{F}{K_2}\quad
Y_x=\frac{F}{K_2}+\frac{F}{Bs}\quad
Y_1=\frac{F}{K_2}+\frac{F}{Bs}+\frac{F}{K_1}$$

## 复杂力学典例1

**复杂系统难以分析，分块列写动力学方程**
![](pic-principal-of-automation-control\Markji_1751374296311.jpg)
$$注：以初始状态为静止平衡状态分析，即弹簧弹力抵消重力$$

## 复杂力学典例2

**灵活设中间变量，辅助分析**
![](pic-principal-of-automation-control\Markji_1751374321708.jpg)

# 时域分析

## 时域尾“1”标准型

$$尾一型：G(s)=\frac{K(2s+1)(-3s+1)}{s^v(s+1)(-2s+1)(5s+1)}（便于计算稳态误差e_{ss}）\\
\ \\
开环增益、开环放大倍数K：
即尾“1”标准型下的比例系数，不一定是稳态增益(s^v\to0)$$

## 一阶系统单位阶跃响应

**图像重点记忆**
![](pic-principal-of-automation-control\Markji_1751374341709.jpg)
$$\Phi(s)=\frac{1}{Ts+1}（时间常数T）\quad
c(t)=1-e^{-\frac{t}{T}}\\
t=T\quad c(t)=63.2\%\\
t=2T\quad c(t)=86.5\%\\
t=3T\quad c(t)=95\%\\
t=4T\quad c(t)=98.2\%\\
可能以响应暗示T$$
$$注：脉冲响应c(t)=\frac{1}{T}e^{-\frac{1}{T}t}$$

## 典型二阶系统

$$主前向通路分子为系数\omega_n^2,a\omega_n^2；且闭环系统为单位负反馈系统\\
G(s)=\frac{\omega_n^2}{s(s+2\xi\omega_n)}\qquad
\Phi(s)=\frac{\omega_n^2}{s^2+2\xi\omega_ns+\omega_n^2}\\
\ \\
s_{1,2}=-\xi\omega_n\pm \sqrt{\xi^2-1}\ \omega_n
\left\{\begin{array}{ll}
\xi:&阻尼比\\
\omega_n:&无阻尼自然频率\\
\omega_d:& 有阻尼振荡频率(\omega_n\sqrt{1-\xi^2})（欠阻尼）
\end{array}\right.\\
\ \\
极点位置及阶跃响应曲线:\\
\xi=0（无阻尼）：两个虚根\quad s_{1,2}=\pm j\omega_n\\
0<\xi<1（欠阻尼）：两个不同的负复极点\quad s_{1,2}=-\xi\omega_n\pm j\sqrt{1-\xi^2}\omega_n\\
{\color{blue}注：\omega_n代表长度，\xi代表角度（以实部\xi\omega_n把握\beta大小）}\\
\xi=1（临界阻尼）：两个相同的负实极点\quad s_{1,2}=-\omega_n\\
\xi>1（过阻尼）：两个不同的负实极点\quad s_{1,2}=-\xi\omega_n\pm \sqrt{\xi^2-1}\omega_n\\
\xi<0（负阻尼）：两个正极点（略）$$
$$注：典型二阶系统传递函数，极点只可能同正、同负或同为零$$

## 二阶欠阻尼系统单位阶跃响应函数

$$h(t)=1-\frac{e^{-\xi \omega_n t}}{\sqrt{1-\xi^2}}\sin(\sqrt{1-\xi^2}\ \omega_nt+\beta)\quad
(\tan\beta=\frac{\sqrt{1-\xi^2}}{\xi})\quad 周期震荡曲线$$

## 不同输入下的系统响应间的关系

$$\begin{array}{ll}
&输入&输出\\
单位脉冲& r_{\delta}(t)=\delta(t) & c_{\delta}(t)=c'_p(t) \\
单位阶跃& r_p(t)=1(t) & c_p(t)=c'_v(t)\\
单位斜坡& r_v(t)=t & c_v(t)=c'_a(t)\\
单位加速度&r_a(t)=\frac{t^2}{2}&\cdots \\
\end{array}\\
针对同一系统，输入满足导数关系，输出间同样满足导数关系$$

## 动态性能指标
$$t_p, \ \sigma\%,\  t_s,\ t_r$$

$$二阶欠阻尼系统极点：-\xi\omega_n\pm j\sqrt{1-\xi^2}\ \omega_n\quad (0<\xi<1)\\
实部:\xi\omega_n\quad 虚部：\sqrt{1-\xi^2}\ \omega_n\quad（
\xi影响角度，\omega_n影响长度）$$
$$t_p=\frac{\pi}{\sqrt{1-\xi^{2}}\omega_n} \qquad （峰值时间）$$
$$\sigma\%=e^{-\frac{\pi}{\tan\beta}} \times100\%=e^{-\frac{\xi}{\sqrt{1-\xi^2}}\pi}\times100\%\\
注：c_{\max}(t)=e_{ss}\cdot(1+\sigma\%)
$$
$$t_s=\frac{3}{\xi\omega_n} (\Delta=0.05) , \ t_s=\frac{4}{\xi\omega_n} (\Delta=0.02)  （如未说明两者都求）
$$
$$t_r=\frac{\pi-\beta}{\sqrt{1-\xi^2}\omega_n}\qquad （上升时间）$$

## 动态性能指标计算器方法

$$使用\textbf{{\color{red}=}}列方程，利用\text{solve}方法解一元方程$$

## 二阶系统动态性能与极点位置的关系

$$借助实部\xi \omega_n,虚部\sqrt{1-\xi^2}\omega_n,\beta(\beta=\arctan\frac{\sqrt{1-\xi^2}}{\xi})判断\\
t_p,t_s,\sigma\%由以上构成$$
$$工程最佳参数：\xi=\frac{\sqrt{2}}{2}=0.707\qquad \sigma\%=e^{-\pi}=4.3\%$$

## 稳定性定义

$$理论分析中：\\
\begin{array}{}
稳定 & 临界稳定 & 不稳定\\
“渐进稳定” & “随遇稳定” & “越偏越远”
\end{array}\\
\ \\
工程实践中：\\
闭环极点全部位于S平面的左半平面，系统稳定\\
只要右半平面，或虚轴上存在闭环极点，系统不稳定（临界稳定、不稳定）
$$
$$注：存在虚根\Leftrightarrow 临界稳定$$
$$齐次连续线性时不变系统为临界稳定的充分必要条件是：\\
系统传递函数中每个极点的实部都为非正值，\\
且其中有一个或多个极点实部为零，\\
且均为相异的单根，\\
而其他的极点实部为负值$$

## 稳定判定方法

**简单情形，解因式，判极点位置**
$$三阶以下首先考虑因式分解$$
**劳斯稳定判据**
$$闭环特征方程D(s)=a_ns^n+a_{n-1}s^{n-1}+\cdots+a_0\\
稳定要求（临界稳定视作不稳定）：\\
1. 各项系数 a_i>0或a_i<0 (i=0,1,2,\cdots)\\
2. 劳斯表第一列大于零且无虚根（虚根为临界稳定）\\
注：\ a_i\ne 0 （i=1,2,\cdots,n-1\quad n阶系统不缺中间项\quad a_0=0为临界稳定）\\
{\color{blue}特殊}：二阶系统各项系数均大于零，即稳定
$$
$$劳斯表列法（行元素“隔阶”列写）：\\
\begin{array}{}
s^4 & 1 & 7 & 10 \\
s^3 & 5 & 2  \\
s^2 & \frac{5\times7-1\times2}{5} & \frac{5\times10-0}{5} \\
s^1 & \cdots \\
s^0 & \cdots
\end{array}\\
根的位置：\\
1.不稳定极点个数a=变号次数\\
2.特征方程纯虚根个数b=辅助方程纯虚根个数\\
3.稳定极点个数=方程阶数-a-b$$
$$注：{\color{blue}劳斯判别法姑且用即可，勿深究各类情况}\\
局限性：无法判断含延迟环节e^{-\tau s}的系统稳定性\\
\ \\
特殊情况：\\
1. \ 0 (\varepsilon\rightarrow 0^+)继续计算，取极限判正负\\
 2. 全零行 \rightarrow 由上一行系数列写辅助函数P(s)，求导作为本行数值\\
辅助方程P(s)的解是原特征方程D(s)解的一部分

$$

## 连续域静态误差系数及稳态误差

$$k_p,\  k_v, \  k_a \qquad
e_{ssp}, \ e_{ssv},  \ e_{ssa}$$

**稳态误差计算前提：先判断稳定性**
**静态误差系数法前提：无输入前馈**
$$G(s)=G_1(s)H(s)=\frac{K}{s^v}\frac{(\tau_1s+1)\cdots(\tau_m+1)}{(T_1s+1)\cdots(T_ns+1)}\\
\left\{\begin{array}{l}K为开环放大倍数\\ v为系统型别，即无静差度
\end{array}\right.$$
$$一般情形：\Phi_e(s)=\frac{s^v(T_1s+1)\cdots(T_n s+1)}{(T_1s+1)\cdots(T_ns+1)+K(\tau_1s+1)\cdots(\tau_2s+1)}\qquad 分子为s^v即代表系统型别$$
**直接用“静态误差系数”计算稳态误差即可**
$$通法：e_{ss}=\lim\limits_{s\to 0}s\cdot E(s)=\lim\limits_{s\to0}s\cdot R(s)\Phi_e(s)\\
\ \\
\begin{array}{ll}
静态误差系数：&稳态误差：\\
k_p=\lim\limits_{s\to0}G_1(s)H(s) &e_{ssp}=\frac{A}{1+k_p}&\lim\limits_{s\to0}\frac{A}{1+G_1(s)H(s)} \\

k_v=\lim\limits_{s\to0}sG_1(s)H(s) &e_{ssv} =\frac{A}{k_v}&\lim\limits_{s\to0}\frac{A}{sG_1(s)H(s)}\\

k_a=\lim\limits_{s\to0}s^2G_1(s)H(s)
&e_{ssa}=\frac{A}{k_a}&\lim\limits_{s\to0}\frac{A}{s^2G_1(s)H(s)}
\end{array}（A为相对于单位输入的系数）$$
$$注：{\color{blue}建议用定义法求稳态误差}，此法作补充（灵活运用）$$

## 连续域稳态误差

**稳态误差计算前提：先判断稳定性**
**直接用梅森增益公式求传函**
$$e_{ss}=e(\infty)=\lim\limits_{s\to 0}sE(s)=\lim\limits_{s\to 0}s\Phi_e(s)R(s)\\

e_{ss}=e(\infty)=\lim\limits_{s\to 0}sE(s)=\lim\limits_{s\to 0}s[R(s)-B(s)]\\

e_{ss}=e(\infty)=\lim\limits_{s\to 0}sE(s)=\lim\limits_{s\to 0}s[E_R(s)-E_N(s)]（输入加干扰）$$
$$注：
\Phi_e(s)=1-\Phi(s)（
典型框图下满足：单位负反馈，无前馈，输入无预置传函）$$

## 动态误差系数法

$$\Phi_e(s)=\frac{E(s)}{R(s)}=c_0+c_1s+c_2s^2+\cdots（s的升阶长除法：除数、被除数均升阶书写）\\
e(t)=c_0r(t)+c_1r'(t)+c_2r''(t)+\cdots$$
$$注：\Phi(s)在s=0邻域内展开，t\to \infty\\
稳态误差随时间的变换规律，即误差的稳态分量$$

## 有理因式的时域反变换

$$一次因式：\\
单根：留数法\\
重根：\mathscr{L^{-1}}\left[\frac{1}{(s+a)^{n+1}}\right]=e^{-at}\frac{t^n}{n!}$$
$$二次因式：\\
单复根：\\
\mathscr{L^{-1}}\left[\frac{s+a}{(s+a)^2+\omega^2}\right]=e^{-at}\cos\omega t\qquad
\mathscr{L^{-1}}\left[\frac{\omega}{(s+a)^2+\omega^2}\right]=e^{-at}\sin\omega t\\
\ \\
注：重复根不考查$$
[Card#ID/1Qe8M#拉氏变换基本定理]

## 非零初始条件下的系统响应

$$例：G(s)=\frac{2(s+2)}{(s+1)(s+4)}\quad c(0)=-1,\dot{c}(0)=0,r(t)=1\\
输入输出微分方程：\ddot{c}+5\dot{c}+4c=2\dot{r}+4r\\
非零初始条件下的拉氏变换：\\
\ [s^2C(s)-sc(0)-c'(0)]+5[sC(s)-c(0)]+4C(s)=\underbrace{2[sR(s)-r(0)]}_{r(0)=0}+4R(s)\\
s^2C(s)+5sC(s)+4C(s)=\underbrace{\frac{1}{s}(2s+4)}_{输入作用}\underbrace{-(s+5)}_{初始条件}\\
C(s)=\underbrace{\frac{-s-5}{s^2+5s+4}}_{C_0}+\underbrace{\frac{2s+4}{s(s^2+5s+4)}}_{C_r}\qquad（拉氏反变换）$$
$$注：输入在零时刻给到系统，故输入为零初始条件，c(0)=0,c'(0)=0;\quad r(0)=0\\
{\color{blue}（传递函数G(s)分母阶次决定输出零初始条件阶次，分子阶次决定输入初始条件阶次）}$$

## 由系统响应求传递函数

$$例1：系统单位阶跃响应为y(t)=1+e^{-t}+e^{-2t}，求系统传递函数\\
\ \\
判断响应为非零初始条件\quad y(0)=3,y'(0)=-3\\

设零初始条件下的y(t)=1+ae^{-t}+be^{-2t}（零初始与非零初始有相同的模态）\\
令\left\{\begin{array}{l}
y(0)=0\\
y'(0)=0
\end{array}\right.
解得
\left\{\begin{array}{l}
a=-2\\
b=1
\end{array}\right.\\
故Y(s)=\frac{1}{s}-\frac{2}{s+1}+\frac{1}{s+2}=\frac{2}{s(s+1)(s+2)}，即G(s)=\frac{2}{(s+1)(s+2)}$$
$$例2：单位阶跃响应为：c(t)=1-1.25e^{-3t}\sin(5t+53.1\degree)
=1-0.75e^{-3t}\sin5t-e^{-3t}\cos5t$$
$$注：单位脉冲响应等也应判断是否零初始条件$$

## 减小或消除稳态误差的方法

$$G(s)增大开环增益K：\\
列写\Phi_e(s)，判断稳态误差变化$$
$$G(s)增加串联积分环节（即提升系统型别v）：\\
列写\Phi_e(s)，判断稳态误差变化（提高系统型别，但会影响系统稳定性）$$
$$\star输入前馈控制（提高系统型别，不影响系统稳定性）：\\
\left\{\begin{array}{}
减小或消除输入信号下的稳态误差\\
减小或消除干扰输入下的稳态误差
\end{array}\right.\\
两种方法：\\1.配系数，使得\Phi_e(s)分子为零（一般G_b(s)实现可能有困难）\\
2.配系数，使得\Phi_e(s)分子阶次满足要求，即提升系统型别$$

## 劳斯判据的参数范围

$$系统稳定：满足劳斯稳定条件，解参数范围、关系$$
$$极点位于s=-a左侧：\\
令s=s^*-a，拆开后对s^*使用劳斯判据，求参数范围\\
注：g(s^*)=0缺项、存在负系数，则参数不存在
$$

## 高阶系统主导极点性能分析

$$瞬态性能指一、二阶系统，若所给系统为高阶，利用主导极点分析\\
\Phi(s)=\frac{10}{(s+5)(s+4.56)(s+0.44)}=\frac{\frac{10}{5\times 4.56}}{(\frac{s}{5}+1)(\frac{s}{4.56}+1)(s+0.44)}\approx\frac{0.44}{s+0.44}
$$
$$注：稳态性能无分系统阶次，直接计算即可\\
主导极点两类情形\left\{\begin{array}{l}非主导极点实部>5倍的主导极点实部\\
偶极子相消（相近的零极点，两点之差小于模本身一个数量级）
\end{array}\right.$$

## 闭环稳定零、极点对系统性能影响

**不考虑调节时间**
$$零点：反应变快，\sigma\%\uparrow\quad t_p\downarrow；随着零点向虚轴靠近越加明显$$
$$极点：反应变慢， \sigma\%\downarrow\quad t_p\uparrow；随着极点向虚轴靠近越加明显$$

## 响应曲线反得系统参数典例

![](pic-principal-of-automation-control\Markji_1751374383156.png)
$$\Phi(s)=\frac{K(s+a)}{s^v(Ts+1)+s+a}=\frac{K(s+a)}{Ts^{v+1}+s^v+s+a}\\
e(\infty)=0\Rightarrow v\geqslant1\\
系统稳定\Rightarrow v\leqslant2\\
c(\infty)=10\Rightarrow \lim\limits_{s\to0}s\cdot \frac{1}{s}\cdot\Phi(s)=10\Rightarrow K=10\\
c'(0)=10\Rightarrow \lim\limits_{t\to0}c'(t)=\lim\limits_{s\to\infty}s\cdot s\cdot\Phi(s)\frac{1}{s}=10\Rightarrow \lim\limits_{s\to\infty}\frac{Ks\cdot(s+a)}{Ts^{v+1}+s^v+s+a}=10\Rightarrow
\left\{\begin{array}{l}
v=1\\
\frac{K}{T}=10
\end{array}\right.$$
$$注：稳定性容易被忽略（特征多项式不缺项等）$$

# 根轨迹分析

考情分析

$$根轨迹校正不考\\
\ \\
根轨迹考查核心为
\left\{\begin{array}{l}
画图\\
解根
\end{array}\right.需灵活利用几何关系、灵活使用根轨迹各结论$$

## 复域首“1”标准型

$$G(s)=\frac{K^*(s-2)(s+3)}{(s+2)(s-1)(s+4)}（便于获取零极点）\\
\ \\
根轨迹增益K^*：首“1”标准型下的比例系数$$

## 根轨迹的本质

$$多项式D(s)=0解根：含参数多项式方程分析根的原理，利用开环传递函数归纳出大致的根轨迹$$

## 根轨迹的不确定性

**根轨迹绘制原理为不完备方法**
$$根轨迹绘制原理存在不确定情形，但考研不会出现$$

## 根轨迹基本概念

**参数变化时，系统特征根变化的轨迹**
**利用开环传递函数分析闭环根轨迹**
$$\Phi(s)=\frac{G_1(s)}{1+G_1(s)H(s)}\\
特征式\Delta=1+G_1(s)H(s)=0，即G_1(s)H(s)=-1\\
注：根轨迹对系统没有要求，但基本只考察单位反馈（正、负），无前馈系统\\
\ \\
在复平面s域中，{\color{blue}以向量把握}\\
模值条件：|G(s)H(s)|=\frac{k^*|s-z_1||s-z_2|\cdots|s-z_m|}{|s-p_1||s-p_2|\cdots|s-p_n|}=1\qquad (k^*:0\rightarrow +\infty)\\
注：知s即可求k^*=\frac{|s-p_1||s-p_2|\cdots|s-p_n|}{{|s-z_1||s-z_2|\cdots|s-z_m|}}\\
\ \\

相角条件：\angle G(s)H(s)=\sum_{i=1}^{m}\underbrace{\angle(s-z_i)}_{零点指向s}-\sum_{j=1}^{n}\underbrace{\angle(s-p_j)}_{极点指向s}=(2k+1)\pi$$
$$注：s点满足相角条件\Leftrightarrow s点在根轨迹上（对平面上任意点，总存在k^*满足模值条件）$$

## 根轨迹坐标图规范

$$实轴\text{Re}，虚轴\text{Im}$$

## 根轨迹基本原理(180度根轨迹) (0度根轨迹）
实轴上的根轨迹，渐近线，出射角，与虚轴交点，根之和，分离点

$$1.起于极点，终于零点与无穷远处\\
分支数为极点数，根轨迹对称于实轴$$
$$2.实轴上根轨迹（充要）：右方奇数个零极点（0度根轨迹为偶数个）$$
$$3.渐近线（0度根轨迹为2kπ）：\\
\left\{
\begin{array}{l}
\theta=\frac{(2k+1)\pi}{n-m} \\
\\
\sigma=\frac{\sum p_i -\sum z_i}{n-m}
\end{array}
\right.\\
注：\frac{(2k+1)\pi}{2}=\pm\frac{\pi}{2};\quad\frac{(2k+1)\pi}{3}=\pm\frac{\pi}{3},\pi;\quad \frac{(2k+1)\pi}{4}=\pm\frac{\pi}{4},\pm\frac{3\pi}{4};\quad \frac{(2k+1)\pi}{5}=\pm\frac{\pi}{5},\pm\frac{3\pi}{5},\pi$$
$$4.出射角与入射角（0度根轨迹为2k\pi）：\\
\sum\angle(s-z_i)-\sum\angle(s-p_j)+(-\theta_出，+\theta_入)=(2k+1)\pi\\
注：\theta取离(2k+1)\pi最近，2\theta,3\theta,\cdots 为多角\\
依题目要求决定是否计算出射角与入射角$$
$$5.与虚轴交点（k^*>0取舍\omega）：
\left\{\begin{array}{l}
\textcircled{1}D(j\omega)=0
\left\{\begin{array}{}
K=\\
\omega=
\end{array}\right.\\
\textcircled{2}劳斯判据,全零行P(s)=0
\end{array}\right.\\
注：高阶系统等幅振荡，即为此种情形$$
$$6.根之和与积：\\
D(s)=s^n+a_{n-1}s^{n-1}+\cdots+a_1s+a_0=(s-s_1)(s-s_2)\cdots(s-s_n)=0\\

\left\{\begin{array}{l}根之和，\sum_{i=1}^ns_i=\sum_{j=1}^np_j=-a_{n-1}\quad(n-m\geqslant2)\\

根之积，\prod_{i=1}^n(-s_i)=a_0
\end{array}\right.$$
$$7.分汇点(必要，取舍由实轴上的根轨迹决定)：只分不汇、只汇不分、汇合分离；实根或复根\\
\textcircled{1}\quad
\sum_{i=1}^{n}\frac{1}{\lambda-p_i}=\sum_{j=1}^{m}\frac{1}{\lambda-z_j}\quad （解得\lambda即为实轴上的根；\quad{\color{blue}可能不全，简单情形使用；以\textcircled{2}为准}）\\

\textcircled{2}
\left.\begin{array}{l}
M^{\prime}(s)N(s)-N^{\prime}(s)M(s)=0  \\ m=0时, N'(s)=0
\end{array}\right\} 分汇点必为方程的根；k阶根对应k+1重分汇点\\
\ \\
注：M(s),N(s)为不含系数的因式\\
\frac{dD(s)}{ds}=0\Leftrightarrow\frac{d}{ds}[1+G(s)H(s)]=\frac{d}{ds}[G(s)H(s)]=\frac{d}{ds}[\frac{kM(s)}{N(s)}]=\frac{d}{ds}[\frac{M(s)}{N(s)}]=0  

$$

## 0度根轨迹与180度根轨迹的关系

$$根轨迹绘制原理要求： 参数k,k^*=0\to +\infty（若为0\to -\infty需对应至0\to +\infty）$$
$$\Phi(s)=\frac{G_1(s)}{1{\color{red}\ \_\ }G_1(s)H(s)}\\判断方法：G_1(s)H(s)化为首1标准型，判断{\color{red}\ \_\ }处正负\\
“+”为180度根轨迹，“-”为0度根轨迹$$

## 参数根轨迹

$$构造等效开环传递函数\\
关键：等效传递函数分母阶数不得小于分子阶数\\
典例：G(s)=\frac{2s+3}{s(s+1)(Ts+1)}\\
D(s)=s(s+1)(Ts+1)+2s+3=0\\
\xrightarrow{阶次处理}s(s+1)(s+\frac{1}{T})+\frac{1}{T}(2s+3)=0\\
G^*(s)=\frac{\frac{1}{T}(s^2+3s+3)}{s^2(s+1)}\quad 注意根轨迹方向(T:0\to +\infty)$$
$$注：
G(s)与G^*(s)仅仅根轨迹相同，其他分析仍须使用G(s)$$

## 全根轨迹

$$提法：参数-\infty<k<+\infty的全根轨迹，或相角180\degree,0\degree的全根轨迹$$
$$典例（参数范围未知）：G(s)=\frac{s+5}{s(s+\rho)}\quad 找出闭环系统临界阻尼时的\rho\\
全根轨迹：G'(s)=\frac{\rho s}{s^2+s+5}\quad \rho范围未知，绘制参数全根轨迹\\
特征方程求解：D(s)|_{s=j\omega}=s(s+\rho)+s+5=0
$$

## 根轨迹分析系统动态性能

$$动态性能计算：按主导极点一、二阶系统计算$$
$$
参数对动态性能的影响：
\left\{\begin{array}{l}
过阻尼\\
临界阻尼\\
欠阻尼\\
临界稳定\\
不稳定
\end{array}\right.$$

## 多项式因子处理技巧

**比较灵活，经常穿插考查**
$$一、\left\{\begin{array}{l}
\left.\begin{array}{l}
极点代入D(s)=0，令\text{Re},\text{Im}为0，解得参数\\
待定系数D(s)=(s+4)(s^2+as+b)展开，系数对应
\end{array}\right\}本质相通\\
降阶长除法（无参数）\\
\end{array}\right.\\
1.使系统有一对复根的阻尼比为\xi=0.707\\
即存在二阶因式\xi=0.707，
D(s)=(s+a)(s^2+2\xi\omega_n s+\omega_n^2)=0\\

2.使系统以\omega=2\ \text{rad}/s等幅振荡，即\xi=0，无阻尼振荡频率\omega_n^2=4；\quad 或有虚根s=\pm j2\\

3.三阶系统D(s)=s^3+k_1s^2+as+1=0有主导极点s_{1,2}=-3\pm j3;\quad即复根代入方程解参数
$$
$${\color{blue}二、根之和公式：\sum_{i=1}^ns_i=\sum_{j=1}^np_j\quad(n-m\geqslant 2)}（中间结论）$$
$$三、劳斯判据求临界稳定因子P(s)\\
1.系统临界稳定：劳斯表出现全零行，
确定参数值\\
2.求全部特征根，一般根据劳斯表先求虚根P(s)=0，再得\theta(s)=D(s)/P(s)$$
$$注：\xi,\omega_n为典型二阶系统的概念，但题目会泛化使用\\
高阶多项式解根属于科研课题，尚无通法
$$

## 高阶特征多项式因子典例

$$G(s)=\frac{100k_1k_2}{s(s+5)(s+2+4k_2)(s^2+10s+50)}\\
闭环主导极点为-1\pm j2，求参数k_1,k_2\\
\ \\
\left\{\begin{array}{l}
\textcircled{1}含参数k_1,k_2，长除法无法求解\\
\textcircled{2}-1\pm j2代入D(s)=0过于复杂
\end{array}\right.\\
由主导极点-1\pm j2，得因式s^2+2s+5=0，即s^2=-2s-5（用于对D(s)降阶）\\
D(s)=s(s+5)(s+2+4k_2)(s^2+10s+50)+100k_1k_2=0\\
(188k_2-345)s-(925+1380k_2)+100k_1k_2=0\\
即
\left\{\begin{array}{l}
188k_2-345=0\\
100k_1k_2-(925+1380k_2)=0
\end{array}\right.解得\left\{\begin{array}{l}
k_1=18.84\\
k_2=1.835
\end{array}\right.
$$

## 根轨迹提法汇总

$$\left.\begin{array}{c}系统无振荡分量\\
过阻尼系统\\
不含振荡模态
\end{array}\right\}全部为实根$$

## 根轨迹分析-圆

$$G(s)=\frac{K(s+z)}{(s+p_1)(s+p_2)}\quad (z位于p_1,p_2的一侧，p_1,p_2不一定实根)\\
\ \\
根轨迹在复平面上为以s=-z为圆心的圆$$
$$证明：G(s)=\frac{K(s+3)}{s(s+2)}\quad
s=\sigma+j\omega代入D(s)=0\\
令实部、虚部均为0可得：
\left\{\begin{array}{l}
\sigma^2+2\sigma+K(\sigma+3)-\omega^2=0\\
2\sigma\omega+2\omega+K\omega=0
\end{array}\right.\\
整理得(\sigma+3)^2+\omega^2=(\sqrt{3})^2\qquad {\color{blue}（\sigma表示横坐标，\omega表示纵坐标）}$$
$$几何考查解根：\xi=0.5;\quad
\omega_d=1\ \text{rad/s}\quad\cdots$$

## 根轨迹解根典例

**灵活利用结论求解即可**
$$规则图形（圆、直线等）：直接几何解根$$
$$\sigma\%,\quad t_s,\quad \omega_d已知\\
\left\{\begin{array}{lcl}
实部：&t_s \rightarrow \xi\omega_n=\frac{3,4}{t_s} &令s=-\xi\omega_n+j\omega_d\\

虚部：&\omega_d & 令s=\delta+j\omega_d\\

阻尼比：&\sigma\%,\xi,\beta & 令s=\delta+j\frac{\sqrt{1-\xi^2}}{\xi}\delta
\end{array}\right.代入D(s)=0
\left\{\begin{array}{l}
\text{实部Re}=0\\
\text{虚部Im}=0
\end{array}\right.解未知参数\\
注：复根均为一对且关于x轴对称，但含参代入求解一般仅需一个$$
$$三阶系统，根据\xi、\omega_d、\xi\omega_n等条件与根之和设特征根\\
例：G(s)=\frac{k_0}{s(s+3)^2}，求k_0使闭环阻尼比\xi=0.707\\
设s_{1,2}=-\sigma\pm j\sigma，s_3=-a_{n-1}-s_1-s_2（\sum_{i=1}^np_i=-a_{n-1};\quad n-m\geqslant 2）\\
D(s)=s^3+6s^2+9s+k_0=(s-s_1)(s-s_2)(s-s_3)=0\quad 解待定系数即可
$$

## 根轨迹典例1

$$G(s)=\frac{k(s+2)}{s^2(s+a)}$$
<img src=pic-principal-of-automation-control\Markji_1751374419364.png width="37%"><img src=pic-principal-of-automation-control\Markji_1751374426561.png width="40%"><img src=pic-principal-of-automation-control\Markji_1751374433631.png width="23%">
$$注：零点对根轨迹有一定的“吸引”$$

## 根轨迹典例2

<img src=pic-principal-of-automation-control\Markji_1751374471679.png width="42%"><img src=pic-principal-of-automation-control\Markji_1751374477942.png width="55%">
$$注：实轴上重合的根轨迹无法确定轨迹分支的走势（可借助分汇点排除；不一定）$$

## 特殊根轨迹

<img src=pic-principal-of-automation-control\Markji_1751374506273.png width="50%"><img src=pic-principal-of-automation-control\Markji_1751374512307.png width="32%">

## 特殊根轨迹典例

**先计算各根轨迹特征，再绘图**
![](pic-principal-of-automation-control\Markji_1751374535780.png)

## 根特征反得系统传递函数典例

![](pic-principal-of-automation-control\Markji_1751374551103.png)
$$(1)\quad G(s)=\frac{k}{s^v\cdot \Delta}\qquad
\left\{\begin{array}{l}
k\in(0,5)时，系统稳定\Rightarrow v\leqslant 1\\
r(t)=1时，e_{ss}=0 \Rightarrow v\geqslant 1\\
\end{array}\right.\\
此时D(s)=s(as^2+bs+1)+k=0\\
k=5时，等幅振荡\omega=\sqrt{6}\Rightarrow D(j\sqrt{6})=0
\left\{\begin{array}{l}
实部\text{Re}=0\\
虚部\text{Im}=0
\end{array}\right.解得参数a,b$$

## 根轨迹解根典例

<img src=pic-principal-of-automation-control\Markji_1751374578251.png width="72%"><img src=pic-principal-of-automation-control\Markji_1751374592237.png width="20%">
$$(1)\quad G(s)=\frac{k}{s(s+p)^2}\quad D(j3)=0解得p=3,此时k=54\\
\ \\
(2)\quad Q(s)=\frac{k(s+z)}{s(s+3)^2}\quad \sum_{i=1}^n p_i=-6，故s_3=-6-(-4)=-2\\
即D(s)=s(s+3)^2+k(s+z)=(s+2)(s^2+4s+20)对应系数即可\\
注：代入法与待定系数法灵活使用$$

# ""频域分析""

## 考情分析

Nichols图、等M圆法不考

## 频域尾“1”标准型

$$G(s)=\frac{K(\frac{s}{\omega_1}+1)(-\frac{s}{\omega_2}-1)}{s^v(-\frac{s}{\omega_3}+1)(\frac{s}{\omega_3}-1)[(\frac{s}{\omega_4})^2+bs+1]}（便于得知转折频率\omega_i\quad \omega_i>0，且K>0）$$

## 正、余弦输入下的稳态输出

$$y(t)=|\Phi(j\omega_0)|\sin[\omega _0t+\theta+\angle\Phi(j\omega_0)]{\color{blue}（仅代表稳态输出）}\\

\left.\begin{array}{l}
|\Phi(j\omega)|_{\omega=\omega_0}\\
\angle\Phi(j\omega)|_{\omega=\omega_0}
\end{array}\right\}复数拆项计算更便捷$$
$$注：\cos(\omega_0 t+\theta)与\sin(\omega_0 t+\theta)同理，直接代入幅值比、相角差即可$$

## 频域基本概念

**由开环频率特性分析负反馈闭环特性**
$$正弦输入r(t)=\sin\omega t下，c_{ss}(t)=|G(j\omega)|\sin(\omega t+\angle{G(j\omega)}){\color{blue}（稳态输出）}\\
频率特性（{\color{blue}以复数向量处理-关键}）：\\
|G(j\omega)|\quad 模长相乘除，与象限无关\quad \sqrt{1+(\frac{\omega}{\omega_i})^2}\\
\angle{G(j\omega)}\quad 相角相加减$$
$$对数频率特性（任意象限）：\\

L(\omega)=20\lg|G|=20\lg\frac{K|j\frac{\omega}{\omega_1}+1||-j\frac{\omega}{\omega_2}-1|\cdots |j\frac{\omega}{\omega_m}+1|}{|-j\frac{\omega}{\tau_1}+1||j\frac{\omega}{\tau_2}-1|\cdots |j\frac{\omega}{\tau_n}+1|}（\text{Bode}折线图几何关系计算）(\frac{s}{\omega_1}+1)\rightarrow
\left\{\begin{array}{}
\frac{\omega_c}{\omega_1} & \omega_c>\omega_1\\
1 & \omega_c<\omega_1
\end{array}\right.\\
\ \\
G(j\omega)对数幅频特性与象限无关，20\lg[\sqrt{1+(\frac{\omega}{\omega_i})^2}]
$$
$$相频特性：\\
\varphi(\omega)=\angle G(j\omega)=\arctan\frac{\omega}{\omega_1}+\arctan\frac{\omega}{\omega_2}+\cdots-90\degree\cdot v-\arctan\frac{\omega}{\omega_i}-\cdots\\
\ \\
\left\{\begin{array}{l}
第一象限复数(j\frac{\omega}{\omega_i}+1\ 或\ jb+a)，\arctan\frac{\omega}{\omega_i}\quad 或\arctan\frac{b}{a}\\

第二象限复数(j\frac{\omega}{\omega_i}-1\ 或\ jb-a)，180\degree-\arctan\frac{\omega}{\omega_i}\quad或180\degree-\arctan\frac{b}{a}\\

第三象限复数(-j\frac{\omega}{\omega_i}-1\ 或\ -jb-a)，-180\degree +\arctan\frac{\omega}{\omega_i}\quad或-180\degree+\arctan\frac{b}{a}\\

第四象限复数(-j\frac{\omega}{\omega_i}+1\ 或\ -jb+a)， -\arctan\frac{\omega}{\omega_i}\quad或-\arctan\frac{b}{a}
\end{array}\right.\quad （K>0）$$
$$注：传递函数处理为频域标准型，且K>0$$

## 传函子环节存在三、四象限情形

$$向量关系分析方法仅适用于K>0时，s为正系数的情况，否则用G(j\omega)的复数本质分析[G]变化趋势$$
$$传递函数处理为频域标准型，仅保留一个三、四象限环节，利用定义分析$$
$$典例：\\
单位负反馈系统开环传函：G(s)=\frac{-0.5s+1}{s(0.2s+1)}e^{-\tau_0s}\\

利用定义分析绘制\text{Nyquist}图、\text{Bode}图\\
G(s)=\frac{-\frac{s}{2}+1}{s(\frac{s}{5}+1)}e^{-\tau_0s}\quad 灵活参照一、二象限环节分析

$$

## 准确Nyquist图绘制

$$整理G(j\omega)为实部与虚部，灵活计算$$

## 频域稳定判据

**Nyquist稳定判据**
$$\omega=0\to +\infty时 \\
Z=P-2N \left\{\begin{array}{l} N为开环传函G_1(s)H(s)包围(-1,j0)点的圈数（逆正顺负）\\
即曲线的环绕圈数（点在其外不算包围）\end{array}\right.\\
Z为右半s平面闭环极点个数，P为右半s平面开环极点个数\\
\ \\
注：频域稳定分析{\color{blue}仅考查负反馈系统}\\
\text{Nyquist}曲线穿过(-1,j0)，系统临界稳定\\
存在积分环节，注意无穷大虚线\\
Z不可能小于0$$
**对数稳定判据（主要针对最小相位系统）**
$$N=N_+-N_- \\
\text{Bode}图中，L(\omega)>0的部分（\text{Nyquist}图中单位圆以外），穿越-180°线，N_+往上穿，N_-往下穿\\
起于负实轴：所有穿越均为\frac{1}{2}穿越，\text{Bode}图中，往上正往下负\\
\ \\
注：若有不确定，以\text{Nyquist}稳定判据为准$$

## 幅值裕度与相角裕度

$${\color{blue}分析1+G(j\omega)H(j\omega)对原点的“包围性”以判断负反馈闭环系统的稳定性}$$
$$相角裕度\gamma=180\degree+\angle[G_1(j\omega_c)H(j\omega_c)]\qquad(|G_1(j\omega_c)H(j\omega_c)|=A(\omega_c)=1)\\
注：以近似A(\omega_c)计算，即
\text{Bode}图\omega_c处\\
部分特殊题型以准确A(\omega)为准（灵活判断）
$$
$$幅值裕量K_g=\frac{1}{|G_1(j\omega_g)H(j\omega_g)|}=\frac{1}{A(\omega_g)}\qquad (\varphi(\omega_g)=-180\degree)\\
增益裕量GM=-20\lg|G_1(j\omega_g)H(j\omega_g)|=-20\lg A(\omega_g)\quad 越大越稳定（幅频特性L(\omega_g),A(\omega_g)越小越好）\\
注：以近似A(\omega_g)计算
$$
$$\arctan A\pm\arctan B=\theta\rightarrow
\frac{A\pm B}{1\mp A B}=\tan\theta\\
\rightarrow \arctan A\pm\arctan B= \arctan\frac{A\pm B}{1\mp AB}$$
$$注：\left\{\begin{array}{}K_g=1&临界稳定\\K_g>1&稳定\end{array}\right.\qquad
\left\{\begin{array}{}\gamma=0&临界稳定\\\gamma>0&稳定\end{array}\right.\\相角裕度、幅值裕度判稳，非普适性方法，但考研不涉及失效情形$$

## 二阶闭环频域特性及性能

$$\Phi(s)=\frac{\omega_n^2}{s^2+2\xi \omega_ns+\omega_n^2}\\
{\color{blue}前提：\xi\leqslant 0.707时，才有以下公式}\\
谐振峰值：M_r=\frac{1}{2\xi\sqrt{1-\xi^2}}\\
谐振频率：\omega_r=\omega_n\sqrt{1-2\xi^2}\\
带宽频率：\omega_b=\omega_n\sqrt{1-2\xi^2+\sqrt{2+4\xi^4-4\xi^2}}\qquad \xi\uparrow \rightarrow \omega_b\uparrow\quad \omega_n\uparrow \rightarrow \omega_b\uparrow\\
注：|\Phi(j\omega_b)|=0.707|\Phi(j0)|\\
$$
$$注：动态性能以时域分析为准\\
高阶闭环频域特性与动态性能之间关系过于复杂，不考查$$

## 二阶开环频域特性及闭环性能

$$对数特性公式
\left\{\begin{array}{l}
\gamma=\arctan\frac{2\xi}{\sqrt{\sqrt{1+4\xi^4}-2\xi^2}}\\
\omega_c=\omega_n\sqrt{\sqrt{1+4\xi^4}-2\xi^2}
\end{array}\right.\\
\gamma一定时，\omega_c越大，闭环系统快速性越好，t_s,t_p越小\\
\omega_c一定时，\gamma越大，闭环系统平稳性越好，\sigma\%越小$$

## 二阶振荡环节的幅频误差

$$\Delta L(\omega_r)=L(\omega)-L_{渐}(\omega)=20\lg\frac{1}{2\xi\sqrt{1-\xi^2}}>0\quad （仅为谐振时，谐振处的误差）$$
$$\Delta L(\omega_n)=L(\omega)-L_{渐}(\omega)=20\lg\frac{1}{2\xi}\quad （转折频率处的误差，{\color{blue}无论谐振与否}）$$
$$注：\text{Bode}图中用来确定\xi$$

## 高阶系统超调量与调节时间的经验公式

**系统校正性能指标转化关键**
$$\sigma=0.16+0.4(\frac{1}{\sin\gamma}-1)\\
t_s=\frac{\pi}{\omega_c}\left[2+1.5\left(\frac{1}{\sin\gamma}-1\right)+2.5\left(\frac{1}{\sin\gamma}-1\right)^2\right]$$
$$高阶可定性认为：\\
\gamma越大，闭环系统平稳性越好，\sigma\%越小\\
\omega_c越大，闭环系统快速性越好，t_s,t_p越小（前提：保证稳定，即保证相角裕度足够大）$$

## 高频段小惯性环节等效

$$G(s)=\frac{K}{s(T_1s+1)(T_2s+1)(T_3s+1)}\quad （T_i较小）\\
G'(s)\approx \frac{K}{s(Ts+1)}\quad (T=T_1+T_2+T_3)
$$

## 典型环节的Nyquist图

$$比例环节G(j\omega)=K：点(K,0)\\
微分环节G(j\omega)=j\omega：上半轴(0\to +\infty)\\
积分环节G(j\omega)=\frac{1}{j\omega}：下半轴(-\infty\to0)$$
$$惯性环节G(j\omega)=\frac{1}{j\omega T\pm 1}：右半面下半圆（稳定）、左半面下半圆（不稳定）\\
一阶微分环节G(j\omega)=j\omega T\pm 1：直线s=-1上半，直线s=1上半（下半部分不考虑）
$$
$$二阶微分环节G(s)=T^2s^2+2\xi Ts+1\\
二阶振荡环节G(s)=\frac{\omega_n^2}{s^2+2\xi\omega_n s+\omega_n^2}：起于(1,0)，终于(0,0);\\
\xi>0稳定，下半弧；\xi<0不稳定，上半弧\\
0<\xi\leqslant0.707有谐振， \xi=0为无穷振荡\\
注：0<\xi<1时为振荡环节；\xi>1时图像类似，但非振荡环节$$
$$延迟环节G(s)=e^{-\tau s}：幅频特性为1，相频特性为-\tau\omega\frac{180\degree}{\pi}=-57.3\degree\tau\omega\quad （顺时针旋转的半径为1的圆）\\
注：延迟环节不影响幅频特性，使相角减小$$
$${\color{blue}注：G(j\omega)加负号，\text{Nyquist}曲线关于原点对称}$$

## 典型环节的Bode图

$${\color{blue}\text{Bode}图在转折点按折线绘制，无须准确曲线}$$
$$比例环节G(j\omega)=K
\left\{\begin{array}{}
L(\omega)=20\lg K\\
\varphi(\omega)=0\degree
\end{array}\right.\\
\ \\
微分环节G(j\omega)=j\omega\left\{\begin{array}{}
L(\omega)=20\lg \omega\\
\varphi(\omega)=90\degree
\end{array}\right.\\
\ \\
积分环节G(j\omega)=\frac{1}{j\omega}\left\{\begin{array}{}
L(\omega)=-20\lg \omega\\
\varphi(\omega)=-90\degree
\end{array}\right.$$
$$惯性环节G(j\omega)=\frac{1}{j\omega T\pm1}
\left\{\begin{array}{}
L(\omega)=-20\lg \sqrt{1+\omega^2T^2}\\
\varphi(\omega)=-\arctan\omega T（稳定）\\
\varphi(\omega)=-180\degree+\arctan\omega T（不稳定）
\end{array}\right.\\
\ \\
一阶微分环节G(j\omega)=j\omega T\pm 1
\left\{\begin{array}{}
L(\omega)=20\lg \sqrt{1+\omega^2T^2}\\
\varphi(\omega)=\arctan\omega T（稳定）\\
\varphi(\omega)=180\degree-\arctan\omega T（不稳定）
\end{array}\right.
$$
$$二阶振荡环节G(s)=\frac{\omega_n^2}{s^2+2\xi\omega_n s+\omega_n^2}：
\omega_n为\text{Bode}图转折频率，准确曲线在转折频率处有上谐振，即凸尖峰\\
0<\xi\leqslant0.707有谐振， \xi=0无穷振荡，即在\omega=\omega_n处L(\omega)趋于\infty\\

\ \\
二阶微分环节G(s)=\frac{s^2+2\xi\omega_n s+\omega_n^2}{\omega_n^2}：L(\omega)与\varphi(\omega)均与振荡环节关于实轴对称（若系数对应）
$$
$$延迟环节G(s)=e^{-\tau s}：对数幅频特性为0\ (20\lg1)，相频特性为-\tau\omega\frac{180\degree}{\pi}=-57.3\degree\tau\omega（弧度制无需深究）\\
注：延迟环节不影响幅频特性，使相角减小$$
$${\color{blue}注：G(j\omega)加负号，\text{Bode}图幅频不变，相频相差\pm 180\degree}$$

## 通用相角计算方法

$$分部法：各因式相角叠加\\
二阶典例：\Phi(j\omega)=\frac{K}{[1-(\frac{\omega}{\omega_n})^2]+2\xi\frac{\omega}{\omega_n}j}\\

\left\{\begin{array}{ll}
(\frac{\omega}{\omega_n})^2<1时，\varphi(\omega)=-\arctan\frac{2\xi\frac{\omega}{\omega_n}}{1-(\frac{\omega}{\omega_n})^2}\\
(\frac{\omega}{\omega_n})^2=1时，\varphi(\omega)=-180\degree
\ \\
(\frac{\omega}{\omega_n})^2>1时，\varphi(\omega)=-\left[180\degree-\arctan\frac{2\xi\frac{\omega}{\omega_n}}{(\frac{\omega}{\omega_n})^2-1}\right] \\
\end{array}\right.\quad（灵活推广）\\
\ \\
整体法：\Phi(j\omega)直接处理为实部、虚部，一次\arctan即可$$

## 坐标图规范

$$\text{Nyquist}图：实轴\text{Re}，虚轴\text{Im}；\quad 标注[G]\\
\text{Bode}图：虚轴{L(\omega)/dB}，实轴\omega(rad/s)$$

## 最小相位系统Nyquist图绘制

**由开环传递函数绘制**
$$最小相位系统\text{Nyquist}图：G(s)=\frac{K(\frac{s}{\omega_1}+1)(\frac{s}{\omega_2}+1)}{s^v(\frac{s}{\omega_3}+1)(\frac{s}{\omega_3}+1)[(\frac{s}{\omega_4})^2+bs+1]}\\
起始段\left\{\begin{array}{cl}
K\angle 0\degree,& v=0\\
虚线\ \infty\cdot \angle -90\degree v ,& v\neq 0
\end{array}\right.\qquad 注：复根对应相角相消后，初始相角仍为0，轨迹仍始于正实轴\\
1.\ s平面中，s=j\omega(\omega=0\to +\infty)\\
据向量关系定性分析|G(j\omega)|与\angle G(j\omega)变化趋势（仅一、二象限），所得绘制于[G]平面中\\
2.\ 若需要绘制渐近线，整理G(j\omega)为实部、虚部求极限$$
[Card#ID/2LV3U#][Card#ID/2LV3U#传函子环节存在三、四象限情形]
$$注：重点在0^+,+\infty时的图像，中间图像大致即可\\

K仅对\text{Nyquist}曲线进行放大缩小，不改变曲线形状$$

## 非最小相位系统Nyquist图绘制

$$典例：G(s)=\frac{10(s+0.5)}{s(s+1)(s-1)}\\
G(j\omega)整理为实部、虚部\\
G(j\omega)=\frac{-10\omega^2}{\omega^2(1+\omega^2)}+j\frac{5\omega}{\omega^2(1+\omega^2)}\\
G(j0^+)=-10+j\infty，增补\infty\cdot \angle -90\degree\cdot v虚线，0^+\to \infty部分据向量关系分析趋势即可\\
\omega=0\to -\infty部分由\omega=0\to +\infty部分关于实轴对称即可$$
[Card#ID/2LV3U#][Card#ID/2LV3U#传函子环节存在三、四象限情形]
![](pic-principal-of-automation-control\Markji_1751374641018.png)
$$注：非最小相角系统也可能始于正实轴\\
\left\{\begin{array}{l}
\omega= 0\to -\infty\\
\omega=0\to+\infty
\end{array}\right.的\text{Nyquist}曲线关于实轴对称;\quad
\left\{\begin{array}{l}
方向构成循环(0^+\to +\infty\to -\infty\to 0^-)\\
G(j\omega)幅频相等，相角相反
\end{array}\right.$$

## Nyquist曲线穿越虚轴点

$$G(s)=\frac{10(s+1)}{(s+5)(s-1)}$$
![](pic-principal-of-automation-control\Markji_1751374663887.png)
$$图像有错误，应以\pm\angle90\degree 趋于0\\
\ \\
G(j\omega)=\frac{10(-5+3\omega^2)}{(\omega^2+25)(\omega^2+1)}+j\frac{-10(9\omega+\omega^3)}{(\omega^2+25)(\omega^2+1)}\\
\omega\to 0^+,G(j\omega)\to 2\angle -180\degree\\
\omega\to \infty,G(j\omega)\to 0\angle -90\degree\\
虚轴交点：\omega=\sqrt{\frac{5}{3}}时，\text{Re}=0,\text{Im}=-常数$$
$$注：不确定是否与虚轴相交时，令\text{Re}=0,判断\text{Im}是否为0$$

## 系统Bode图绘制

**由开环传递函数绘制**
$$\text{Bode}图：几何折线图\\
低频段（高、陡为佳）\qquad 决定系统稳态误差e_{ss}\\
G_0(s)=\frac{K}{s^v}\left\{\begin{array}{}
20\lg|G_0|=20\lg K-20\cdot v\cdot\lg \omega\\
\angle G=-90\degree\cdot v\end{array}\right.\quad
静态误差系数法分析e_{ss}\\
\ \\
中频段（缓、宽为佳）\qquad 决定系统动态性能(\sigma\%,t_s)\\
\left\{
\begin{array}{lcc}
&L(\omega)&\varphi(\omega)变化趋势{\color{blue}（一、二象限复数）}\\
极点处 &-20dB/dec&趋向"-"90\degree\\
零点处 &+20dB/dec&趋向"+"90\degree
\end{array}
\right.\\
 \ \\
高频段（低、陡为佳）\qquad 决定系统抗高频干扰能力$$

## Bode图折线原理

**完整代表系统折线**
$$G(s)=\frac{6}{s(\frac{s}{10}+1)[(\frac{s}{100})^2+\frac{s}{100}+1]}$$
$$0<\omega<10：
\left\{\begin{array}{rl}
L(\omega)&=20\lg\frac{6}{\omega}\\
&=\underline{20\lg6}-20\lg\omega\\
\ \\
&A(\omega)\approx\frac{6}{\omega}
\end{array}\right.$$
$$10<\omega<100：
\left\{\begin{array}{rl}
L(\omega)&=20\lg\frac{6}{\omega\cdot\frac{\omega}{10}}\\
&=20\lg6-20\lg\omega-20\lg\frac{\omega}{10}\\
&=\underline{20\lg6}-20\lg\omega-20\lg\omega+\underline{20\lg{10}}\\
\ \\
&A(\omega)\approx\frac{6}{\omega\cdot\frac{\omega}{10}}
\end{array}\right.$$
$$\omega>100：
\left\{\begin{array}{rl}
L(\omega)&=20\lg\frac{6}{\omega\cdot\frac{\omega}{10}\cdot(\frac{\omega}{100})^2}\\

&=20\lg6-20\lg\omega-20\lg\frac{\omega}{10}-20\lg(\frac{\omega}{100})^2\\
&=\underline{20\lg6}-20\lg\omega-20\lg\omega+\underline{20\lg{10}}-40\lg\omega+\underline{40\lg100}\\
\ \\
&A(\omega)\approx\frac{6}{\omega\cdot\frac{\omega}{10}\cdot(\frac{\omega}{100})^2}
\end{array}\right.$$
$$注：“元变化率”：-20\lg\omega\\
分段折线过点(1,\sum “\_\_”)\\
二阶振荡环节[(\frac{s}{\omega_n})^2+2\xi \frac{s}{\omega_n }+1]折线视作[(\frac{s}{\omega_n})^2+1]处理\\
{\color{blue}A(\omega)表示幅频}$$

## Bode图绘制规范

**关键：低频段及其延长线**
$$G(s)=\frac{K(\frac{s}{\omega_i}+1)\cdots}{s^v(\frac{s}{\omega_j}+1)\cdots}\\
1.斜率（-20，-40，\cdots）\\
2.特殊点
\left\{\begin{array}{l}
{\color{blue}“轴点”(1,20\lg K)}\quad （若存在\omega_i<1，则低频段延长线过“轴点”）\\
各转折频率\omega\\
截止频率\omega_c\\
\end{array}\right.\\
3.低频段延长线及横轴交点(\sqrt[v]{K},0)\quad 注：20\lg K-v\cdot 20\lg\omega=0$$

## 截止频率计算方法

$$G(s)=\frac{K}{s(\frac{s}{\omega_1}+1)(\frac{s}{\omega_2}+1)[(\frac{s}{\omega_3})^2+2\xi\frac{s}{\omega_n}+1]}
$$
$$关键：确定\omega_c范围（若范围已知，则一步到位）$$
$$确定范围：{\color{blue}转折频率夹逼（便捷）}\\
A(\omega_1)>1,A(\omega_2)<1，则\omega_1<\omega_c<\omega_2\\
若L(\omega)单减不增，
\left\{\begin{array}{l}
A(\omega_1)<1，则\omega_c<\omega_1\\
A(\omega_3)>1，则\omega_c>\omega_3
\end{array}\right.\\
\ \\
计算：试探反解\\
令A(\omega_c)=\frac{K}{\omega_c\cdot \frac{\omega_c}{\omega_1}}=1，即可解得\omega_c$$
$$注：考研范围内，{\color{blue}L(\omega)单减不增}$$

## 最小相角系统

$$开环零、极点都在左半s平面或虚轴上$$
$$注：L(\omega)已知情况下，最小相角系统确定$$

## 特殊Nyquist曲线
$$含(s^2+1)环节的系统$$

$$G(s)=\frac{k(s^2+1)}{s(s+5)}$$
![](pic-principal-of-automation-control\Markji_1751374684480.png)

## Nyquist曲线反求传函

$$单位负反馈系统\text{Nyquist}图如下，G(j\sqrt{2})=-j\sqrt{2}，求系统传函$$
![](pic-principal-of-automation-control\Markji_1751374704881.png)
$$G(s)=\frac{K}{as^2+bs+1}\quad
\left\{\begin{array}{l}
G(j0)=3\Rightarrow K=3\\
G(j\sqrt{2})=\frac{3}{1-2a+j\sqrt{2}b}=-j\sqrt{2}\Rightarrow a=0.5,b=1.5
\end{array}\right.$$
$$注：考研考查不会复杂$$

## Bode图反求传函典例

![](pic-principal-of-automation-control\Markji_1751374719579.png)
$$“两个坐标点，两个未知参数”\\
G(s)=\frac{K}{s(\frac{s}{\omega_1}+1)}
\left\{\begin{array}{l}
(1,20\lg K)=(1,13.98)\\
20\lg\frac{K}{\omega\cdot\frac{\omega}{\omega_1}}\bigg|_{\omega=10}=-20\qquad (10,-20)代入分段折线
\end{array}\right.$$
$$注：最小相位系统时，直接根据幅频可得传函$$

## 相角裕度稳定题型

$$相角裕度判稳：G(s)=\frac{e^{-3 s}}{s(s+1)}\qquad （主要用相角裕度法）
$$
$$相角裕度反求参数：\\G(s)=\frac{e^{-\tau s}}{s(s+1)}，求稳定的\tau的范围
\left\{\begin{array}{l}
A(\omega_c)=1\\
\gamma(\omega_c)=0\degree
\end{array}\right.\\
\ \\
G(s)=\frac{Ke^{-2s}}{s},\quad K>0，求稳定的K的范围
\left\{\begin{array}{l}
\gamma(\omega_c)=0\degree\\
A(\omega_c)=1
\end{array}\right.\\
\ \\
G(s)=\frac{K}{(\tau s+1)^3},\quad \gamma(\omega_c)=45\degree，求K\left\{\begin{array}{l}
\gamma(\omega_c)=180\degree-3\arctan\tau\omega=45\degree\Rightarrow\omega=\frac{1}{\tau}\\
A(\omega_c)=\frac{K}{\sqrt{(j\frac{1}{\tau}\cdot\tau)^2+1^2}^3}=\frac{K}{\sqrt{2}^3}=1
\end{array}\right.
$$

## 对数稳定判据典例

$$最小相位系统，判断稳定性$$
![](pic-principal-of-automation-control\Markji_1751374740609.png)
$$判断L(\omega)>0部分的穿越性\\
N^-=1,N^+=1，故N=N^+-N^-=0\\
Z=P-2N=0-0=0$$

## 含延迟环节的Nyquist曲线

$$开环传函G(s)=\frac{Ke^{-2s}}{s}，求系统稳定时K的取值范围$$
![](pic-principal-of-automation-control\Markji_1751374754900.png)
$$含延迟环节的曲线均为无限收缩的螺线（曲线不甚准确）\\
e^{-2j\omega}需延迟90\degree，换算为弧度制，2\omega应为\frac{90\degree}{57.3\degree}\\
\varphi(\omega_g)=-90\degree-57.3\degree\times 2\omega_g=-180\degree\\
|G(\omega_g)|=\frac{K}{\omega_g}\leqslant 1$$

# 系统校正

## 考情分析

**基本考查三大校正，勿固化，灵活运用**
**难度不高，但较为繁琐，能满足要求即可**

## 校正指标

$$e_{ss}\\
K_p,K_v,K_a\\
\omega_c,\gamma
$$
$$K_g考查要求不高$$
$$\sigma\%,t_s
\left\{\begin{array}{l}
\textcircled{1}\ 目标二阶系统反解\xi,\omega_n\\
\textcircled{2}\star高阶系统转化为\omega_c,\gamma
\end{array}\right.
$$
[Card#ID/2elj8#高阶系统超调量与调节时间的经验公式]

## 三频段理论

$$低频段\left\{\begin{array}{l}
v\uparrow \\
K\uparrow
\end{array}\right.
\Rightarrow e_{ss}\downarrow，精度\uparrow\\
\ \\
中频段\left\{\begin{array}{l}
\gamma\uparrow，系统平稳性越好，\sigma\%越小\\
\omega_c\uparrow，系统快速性越好，t_s,t_p越小（前提：保证稳定，即保证相角裕度足够大）
\end{array}\right.\\

\ \\
注：希望L(\omega)以-20dB/dec斜率穿越0dB，并保持较宽的频段\\
（一般拉开10倍频，此时会有相当的相角裕度；-20dB/dec\quad\star\quad\gamma\to 90\degree）\\
\ \\
高频段\quad L(\omega)\downarrow \quad\Rightarrow 抗高频干扰能力\uparrow$$

## 频域矫正注意

$$幅频特性均以\text{Bode}图折线计算，无须精确A(\omega)$$

## 符号含义注明

$$\omega_c：系统原截止频率\\
\gamma_0：系统原相角裕度\\
\ \\
\omega_m：矫正参考位置\\
\gamma_m：系统本身在参考位置的相角裕度\\
\gamma_m'：矫正后系统在参考位置的相角裕度\\
\phi_m：相角差值，非具体相频特性\\
\varphi_m：具体相角值，系统相频特性$$

## 滞后校正

**灵活结合使用**
**以校正图像把握校正步骤**
$$相角校正幅度取决于系统：附加-20dB斜率，使系统幅频特性L(\omega)减小至0$$
$$校正步骤：\\
情形一：校正稳态性能（中频段）\\
\textcircled{1}计算\omega_m\quad(\gamma_m=\gamma+6\degree)\\
\textcircled{2}L(\omega_m)=20\lg\beta反解\beta（\text{Bode}图折线）\\
\\
\textcircled{3}\ 校正后检验（\gamma_m'\geqslant\gamma）\\
\ \\
G_c(s)=\frac{\frac{s}{\omega_2}+1}{\frac{s}{\omega_1}+1}=\frac{Ts+1}{\beta Ts+1}\quad{\color{blue}(\beta>1)}\\

\omega_1=\frac{\omega_m}{10\cdot\beta },\quad \omega_2=\frac{\omega_m}{10}
$$
$$情形二：校正低频段，中频段满足要求\\
\textcircled{1}确定K'\ (e_{ss};\quad K_p/K_v/K_a)，令\beta=\frac{K'}{K}（K'>K），此时\omega_m=\omega_c不变，\gamma减小少于6\degree\\
\ \\
G_c(s)=K\frac{\frac{s}{\omega_2}+1}{\frac{s}{\omega_1}+1}=\beta\frac{Ts+1}{\beta Ts+1}\quad{\color{blue}(\beta>1)}\\

\omega_1=\frac{\omega_m}{10\cdot\beta },\quad \omega_2=\frac{\omega_m}{10}$$
$$注：滞后校正不存在“耦合”问题，不必检验，但流程是必要的$$

## 超前滞后校正

**以校正图像把握校正步骤**
$$校正步骤：\\
\textcircled{1}\ 先滞后，在合适\omega_m处，挖掘系统相角\gamma_m，计算超前环节需提供的相角\phi_m=\gamma-\gamma_m+6\degree\\
\textcircled{2}\ 反解\alpha=\frac{1-\sin\phi_m}{1+\sin\phi_m}，计算\beta\quad 20\lg\beta+\underbrace{10\lg\alpha}_{<0}=L(\omega_m)，在原系统\omega_m处放置超前环节中点\\
\textcircled{3}\ 校正后检验（\gamma_m'\geqslant\gamma）$$
$$G_c(s)=\frac{\frac{s}{\omega_2}+1}{\frac{s}{\omega_1}+1}\cdot
\frac{\frac{s}{\omega_3}+1}{\frac{s}{\omega_4}+1}
=\frac{Ts+1}{\alpha Ts+1}\cdot\frac{Ts+1}{\beta Ts+1}\quad{\color{blue}(0<\alpha<1,\beta>1)}\\
\ \\
\omega_4=\frac{\omega_m}{\sqrt{\alpha}},\quad \omega_3=\omega_m \cdot\sqrt{\alpha},\quad \omega_2=\frac{\omega_m}{10},\quad \omega_1=\frac{\omega_m}{10\cdot \beta}$$
$$注：超前滞后校正不存在“耦合”问题，不必检验，但流程是必要的$$

## 超前校正

**以校正图像把握校正步骤**
$$校正步骤（最大提供超前角60\degree）：\\
情形一：\gamma不满足要求，\omega_c满足要求\\
\textcircled{1}在\omega_c处，计算所需提供的相角\phi_m=\gamma-\gamma_0+5\degree\sim 10\degree，反解\alpha=\frac{1-\sin\phi_m}{1+\sin\phi_m}\\
\textcircled{2}在原系统L(\omega_m)=10\lg\alpha{\color{blue}<0}处放置超前环节中点\\
\textcircled{3}\ 校正后检验（\gamma_m'\geqslant\gamma），若不合格，可适当增减相角偏差(5\degree\sim10\degree)，或直接调整校正装置系数（经验）$$
$$情形二：\gamma，\omega_c均不满足要求\\
\textcircled{1}首先取\omega_m满足要求，计算\alpha\quad L(\omega_m)=10\lg \alpha{\color{blue}<0}，检验(\gamma_m'\geqslant \gamma)\\
\textcircled{2}若不满足，\omega_m再适当往大取
$$
$$G_c(s)=\frac{\frac{s}{\omega_1}+1}{\frac{s}{\omega_2}+1}=\frac{Ts+1}{\alpha Ts+1}\quad{\color{blue}(0<\alpha<1)}\\

\omega_1=\omega_m\sqrt{\alpha},\quad \omega_2=\frac{\omega_m}{\sqrt{\alpha}}$$
$$\phi_m=\arcsin\frac{1-\alpha}{1+\alpha},\quad \alpha=\frac{1-\sin \phi_m}{1+\sin \phi_m}$$
$$注：超前校正存在“耦合”问题，必须检验$$

## 校正方案选择

$$根据系统特征与要求，依{\color{blue}直觉选择}合适校正方案；
无需倾向，否则浪费时间$$

## 速度反馈或微分反馈校正

$$K(\neq0),k_f任取均为典型二阶系统$$
![](pic-principal-of-automation-control\Markji_1751374809326.png)
$$
“子闭环”反馈\beta s\\
速度反馈(\beta s)校正后仍为典型二阶系统

$$

## 非主要校正方法

$$反馈校正：整理为传函，具体情况具体分析（影响稳定性，影响动态性能）\\
\ \\
\text{PID}校正：一般校正方式已知，反解参数\\
\ \\
希望特性校正：方法简单，辅助方法，或三大校正失效时使用$$

## K未知校正典例

![](pic-principal-of-automation-control\Markji_1751374826774.png)
$$思路一：校正中频段；\quad  根据K_v直接确定K，对G_0'(s)进行校正$$
$${\color{grey}思路二：校正低频段；\quad确定\gamma满足要求的截止频率，解得K}$$
$$注：K未知的校正题型
\left\{\begin{array}{l}
\textcircled{1}\ 先确定K，再对中频段进行校正\\
\textcircled{2}\ 先确定满足中频要求的K^*，再对低频段进行校正
\end{array}\right.以\textcircled{1}为准，暂不区分，幅频的上下平移$$

## 超前滞后校正与希望特性结合典例

**要求不苛刻时，此法校正速度最快**
![](pic-principal-of-automation-control\Markji_1751374841280.png)
$$\omega_c=2\sqrt{3},\quad\gamma=0\degree\\
\ \\
\frac{\omega_c}{\omega_3}=\frac{\omega_4}{\omega_c}=\sqrt{10};\qquad \omega_2=\frac{\omega_c}{10};\qquad
A(\omega_c)=\frac{12\cdot\frac{\omega_c}{\omega_2}\cdot\frac{\omega_c}{\omega_3}}{\omega_c^2\cdot\frac{\omega_c}{\omega_1}}=1$$

## 反馈校正与希望特性结合典例

![](pic-principal-of-automation-control\Markji_1751374862408.png)
![](pic-principal-of-automation-control\Markji_1751374868397.png)

## 串联校正典例

**希望特性的思想**
![](pic-principal-of-automation-control\Markji_1751374947886.png)
$$G(s)=\frac{31.6}{s(\frac{s}{31.6}+1)}\\
\textcircled{2}\quad e_{ss}\leqslant1，故系统v\geqslant2，设计G_c(s)=\frac{s+1}{s}\qquad (s+1)“妙”\quad“轴点”(1,20\lg K)$$

# 离散域

## 考情分析

模拟化校正不考，动态性能不考，动态误差系数法不考
**离散域的分析方法很匮乏**

## 离散域“延迟因子”标准型

$$G(z)=\frac{0.4z^{-1}(1+0.3z^{-1})}{(1-z^{-1})(1+0.5z^{-1})}\qquad(最小拍校正形式；便于获取零极点，负的z^{-1}系数即为零极点)$$
$$注：物理可实现系统(z的多项式n\geqslant m)$$

## 离散域基本概念

$$Z变换定义：E(z)=Z[e^*(t)]=E^*(s)|_{z=e^{Ts}}=\sum_{n=0}^{\infty}e(nT)z^{-n}$$

## 脉冲传递函数

$$零初始条件下，离散系统输出Z变换对输入Z变换之比$$

## 香农采样定理

$$\omega_s=\frac{2\pi}{T}=2\pi f\geqslant 2\omega_{\max}（连续信号频谱的上限频率）\\
\ \\
注：\omega_s为角频率，T为周期，f为频率$$

## 常见函数Z变换
$$\delta(t),\delta(t-kT), \ 1(t), \ t, \ \frac{t^2}{2}, \ a^{\frac{t}{T}}, \ e^{-aT}$$

$$\begin{array}{}
f(t)或f(k)& F(z)\\
\delta(t) & 1\\
\delta(t-kT) & z^{-k}\\
1(t) &\frac{1}{1-z^{-1}} & \frac{z}{z-1}\\
\ \\
t & \frac{Tz^{-1}}{(1-z^{-1})^2} & \frac{Tz}{(z-1)^2}\\
\ \\
\frac{t^2}{2} & \frac{T^2z^{-1}(1+z^{-1})}{2(1-z^{-1})^3} & \frac{T^2z(z+1)}{2(z-1)^3}\\
\ \\
a^{\frac{t}{T}},a^k & \frac{1}{1-az^{-1}} & \frac{z}{z-a}\\
\ \\
e^{-at},e^{-akT} & \frac{1}{1-e^{-aT}z^{-1}} & \frac{z}{z-e^{-aT}}
\end{array}$$
$$零阶保持器：Z\left[\frac{1-e^{-Ts}}{s}KG(s)\right]=K(1-z^{-1})Z\left[\frac{G(s)}{s}\right];\qquad
Z\left[\frac{1-e^{-Ts}}{s}e^{-Ts}G(s)\right]=z^{-1}(1-z^{-1})Z\left[\frac{G(s)}{s}\right]$$

## Z变换基本定理

**实质上是对连续信号离散后的信号进行Z变换**
$$线性性质：\\
Z[a\cdot e_1(t) +b \cdot e_2(t)] = aE_1(z)\pm bE_2(z)$$
$$实位移定理（延迟、超前）：\\
\left\{
\begin{array}{l}
Z[e(t-nT)]=Z^{-n}E(z) \\
Z[e(t+nT)]=Z^n[E(z)-\sum_{k=0}^{n-1}e(kT) \cdot z^{-k}]
\end{array}
\right.$$
$$复位移定理：\\
Z[e(t) \cdot e^{\mp at}]=E(z \cdot e^{\pm aT})$$
$$初值定理：\\
\lim\limits_{n\to 0}e(n)=\lim\limits_{z\to\infty}E(z)$$
$$终值定理：\\
\lim\limits_{n\to \infty}e(n)=\lim\limits_{z\to1}(z-1)E(z)$$

## Z变换

$$含重根时：\\
部分分式法：F(s)展开为部分分式，常见函数Z变换对应$$
$$纯单根时：\\
留数法：
E[z]=\sum \text{Res}[E(s) \cdot \frac{z}{z-e^{Ts}}]\big|_{s=s_i}
\\
\text{Res}[E(s) \cdot \frac{z}{z-e^{Ts}}]=\lim\limits_{s\to s_i}[(s-s_i) \cdot E(s) \cdot \frac{z}{z-e^{Ts}}]$$
$$注：含重根时，留数法可能存在理论问题\\
Z变换的计算考查不会很复杂，无须深究$$

## Z反变换

$$纯单根时：\\
部分分式法：\frac{X(z)}{z}展开成部分分式，分母的z乘至部分分式的分子位置\\
\ \\
注：Z反变换的通式计算考查很简单，一般只考纯单根\\
部分分式法通用性不强，适用单根，重根一般不易对应时域表达式\quad如\frac{T^2z(1+z)}{2(z-1)^3}\\
$$

$$长除法（无穷项）：z^{-1}的升阶长除法$$

## 离散稳定判定

$$1.特征根判定（二阶解根用韦达定理）：\\
解D(z)=0的根，单位圆内稳定；单位圆上临界稳定；单位圆外不稳定\\
2.劳斯判据:双线性变换：z=\frac{\omega+1}{\omega-1}代入D(z)，通分后分子为D^*(\omega)，对D^*(\omega)=0使用劳斯判据即可\\
3.朱利二阶系统判别，特征多项式D(z)=z^2+a_1z+a_0
\left\{
\begin{array}{}
|D(0)|=|a_0|<1\\
D(1)=1+a_1+a_0>0\\
D(-1)=1-a_1+a_0>0
\end{array}
\right.\\
4.\star\star含参数的离散根轨迹与单位圆的关系\star\star$$
$$注：离散稳定性与连续稳定性无必然联系\\
$$

## 离散域静态误差系数及稳态误差

$$k_p, \ k_v, \ k_a \\
e_p(\infty), \ e_v(\infty), \ e_a(\infty)$$

**稳态误差计算前提：先判断稳定性**
**直接用“静态误差系数”计算稳态误差即可**
$$通法：e_{ss}=\lim\limits_{z\to 1}(z-1)E(z)=\lim\limits_{z\to 1}(z-1)\cdot R(z)\cdot\Phi_e(z)\\
\ \\
\begin{array}{lll}
静态误差系数：&稳态误差：\\
k_p=\lim\limits_{z\to1}GH(z)& e_p(\infty)=\frac{A}{1+k_p}&\frac{A}{1+\lim\limits_{z\to1}GH(z)}\\

k_v=\lim\limits_{z\to1}(z-1)GH(z)&e_v(\infty)=\frac{AT}{k_v}&\frac{AT}{\lim\limits_{z\to1}(z-1)GH(z)}\\

k_v=\lim\limits_{z\to1}(z-1)^2GH(z)&e_a(\infty)=\frac{AT^2}{k_a}&\frac{AT^2}{\lim\limits_{z\to1}(z-1)^2GH(z)}
\end{array}$$
$$注：离散稳态误差用静态误差系数法一般不失效$$

## 离散域稳态误差

**稳态误差计算前提：先判断稳定性**
**用梅森增益公式求传函，“直连项”整体Z变换**
$$e_{ss}=e(\infty)=\lim\limits_{z\to 1}(z-1)E(z)=\lim\limits_{z\to 1}(z-1)\cdot \Phi_e(z)\cdot R(z)\\

e_{ss}=e(\infty)=\lim\limits_{z\to 1}(z-1)E(z)=\lim\limits_{z\to 1}(z-1)\cdot[R(z)-B(z)]\\

e_{ss}=e(\infty)=\lim\limits_{z\to 1}(z-1)E(z)=\lim\limits_{z\to 1}(z-1)\cdot[E_R(z)-E_N(z)]（输入+干扰）$$

## 离散输出与连续输出的关系

$$\begin{array}{ll}
连续\to 连续 & 连续\to 离散\\
离散\to 连续 & 离散\to 离散
\end{array}$$
$$理论上，离散输出与连续输出有本质区别：（较复杂，适当把握即可）\\
同一系统（连续或离散化），输入给定“符合”的连续与离散信号，其输出必然不同（激励不同，结果必然不同）\\
同一信号，给到连续或被离散化的系统（连续信号不被等效为离散），其输出也必然不同（单纯的输出离散化系统除外）$$
$${\color{blue}脉冲响应不变性}：由于脉冲信号本身可视为连续或离散，且只作用某一时刻；\\
同一系统（连续或离散化）在脉冲信号激励下，连续或离散化输出一致
$$
$${\color{blue}除脉冲响应外，其余响应的离散与连续基本不“符合”}$$
$$注：离散化的系统子环节仍为连续$$

## 求脉冲传递函数与离散输出

$$列写连续域表达式与传递函数
\left\{
\begin{array}{}
子环节间存在“直线”连通，则一起Z变换\\
子环节间无“直线”连通，则分开Z变换
\end{array}\right.$$
$$注：考研范围内，此法均适用，
但事实上存在失效情况\\
脉冲传递函数可能无法求，输入与内部之间无“开关”，或内部耦合无法相消
$$
![](pic-principal-of-automation-control\Markji_1751375002452.png)
$$列写C(s)表达式，按照“直连”原则改写即可\\
前馈与中间环节捆绑，导致脉冲传递函数不存在$$
![](pic-principal-of-automation-control\Markji_1751375019609.png)
$$脉冲传递函数典例：内部耦合无法相消，即失效情形$$

## 极点在z平面分布与瞬态响应的关系

$$重根情形较复杂，{\color{blue}定性理解即可}，考研不涉及计算$$
![](pic-principal-of-automation-control\Markji_1751375046666.png)
$$\left\{\begin{array}{l}
0<z<1的实根，衰减无振荡\\
-1<z<0的实根，衰减振荡\\
\\
z=1，等值不变\\
z=-1，等值振荡\\
|z|=1的复根，等幅振荡\\
\ \\
z>1的实根，发散无振荡\\
z<-1的实根，发散振荡\\
\ \\
|z|<1的复根，衰减振荡\\
|z|>1的复根，发散振荡\\

\end{array}\right.$$

## 离散域中的根轨迹

$$前提：脉冲传递函数存在\\
根据开环传递函数G(z)画根轨迹，根据极点与单位圆之间的关系判稳\\
$$
$$注：整理为关于z的多项式$$

## 最小拍校正

$$标准型：G(z)=\frac{0.4z^{-1}(1+0.3z^{-1})}{(1-z^{-1})(1+0.5z^{-1})}$$
$$\Phi(z)=\frac{D(z)G(z)}{1+D(z)G(z)}\quad 纯延迟因子，G(z)单位圆上、外的零点\\
\Phi_e(z)=\frac{1}{1+D(z)G(z)}\quad 输入分母（z^{-1}形式），G(z)单位圆上、外的极点\\
注：\Phi_e(z)的“极点因子”与“输入分母因子”{\color{blue}不应叠加}，取阶次高者即可$$
$${\color{blue}保证三条原则}：延迟因子，单位圆上、外的零极点，\Phi(z)与\Phi_e(z)为z^{-1}齐次\\
对应设z^{-1}的多项式，解未知系数
\left\{
\begin{array}{l}
\Phi(z)=az^{-1}(1+bz^{-1})\cdots\\
\Phi_e(z)=(1+z^{-1})(1+cz^{-1})\cdots
\end{array}
\right.\quad
 \Phi(z)=1-\Phi_e(z)解参数\\
整体思路：“凑”\qquad 凑不出来设高阶\qquad 调整拍数取决于具体系统，不一定$$
$$反解校正传函：D(z)=\frac{\Phi(z)}{G(z)\Phi_e(z)}\quad $$
$$注：
最小拍校正需满足\Phi(z)=1-\Phi_e(z)，即无前馈，无输入传函，且单位负反馈；其它情形不考，难以使用

$$
$$补：系统各观测点的各采样点间无波动即为无波纹系统（长除法求输出判断）$$

## 离散系统的差分方程或输出

$$\Phi(z)=\frac{0.368z^{-1}+0.264z^{-1}}{1-z^{-1}+0.632z^{-1}}$$
$$差分方程：\\

C(z)=\Phi(z)\cdot R(z)=\frac{0.368z^{-1}+0.264z^{-2}}{1-z^{-1}+0.632z^{-2}}\cdot R(z)\\
(0.368z^{-1}+0.264z^{-2})R(z)=(1-z^{-1}+0.632z^{-2})C(z)\\
0.368r(n-1)+0.264r(n-2)=c(n)-c(n-1)+0.632c(n-2)$$
$$系统输出（差分方程代入，或长除法）：\\
C(z)=\Phi(z)\cdot R(z)=\frac{0.368z^{-1}+0.264z^{-2}}{1-z^{-1}+0.632z^{-2}}\cdot \frac{1}{(1-z^{-1})}\\
C(z)=0.368z^{-1}+z^{-2}+1.4z^{-3}+\cdots\\
c(t)=0.368\delta(t-T)+\delta(t-2T)+1.4\delta(t-3T)+\cdots$$

## 已知稳态误差反解参数范围

![](pic-principal-of-automation-control\Markji_1751375072618.png)
$$G(z)=Z[\frac{1-e^{-Ts}}{s}\times\frac{Ke^{-Ts}}{s}]=\frac{KT}{z(z-1)}\\

\left\{\begin{array}{ll}
K_p=\lim\limits_{z\to1}G(z)=\infty, & e_{ssp}=\frac{2}{1+K_p}=0\\

K_v=\lim\limits_{z\to 1}(z-1)G(z)=0.2K, & e_{ssv}=\frac{1}{K}
\end{array}\right.\\
\ \\
\left\{\begin{array}{l}
稳态误差：e_{ss}=e_{ssp}+e_{ssv}=\frac{1}{K}<0.25\\
\star 系统稳定：D(z)=z^2-z+0.2K=0
\end{array}\right.$$
$${\color{blue}注：连续系统同理，确保系统稳定}$$

# """非线性系统分析"""

## 考情分析

只考几类典型的非线性特性、非线性校正不考

## 非线性分析题型方法对应

$$\begin{array}{l}
相平面分析\#微分方程 & 相平面分析\#系统框图\\
\ \\
描述函数法\#微分方程 & 描述函数法\#系统框图

\end{array}$$

## 奇点（平衡点）

$$\ddot{x}+f(x,\dot{x})=0\Leftrightarrow\frac{d\dot{x}}{dx}=-\frac{f(x,\dot{x})}{\dot{x}}（非所有二阶非线性微分方程均有此形式）\\
\ \\
奇点(x_0,\dot{x_0})：\\
满足
\left\{\begin{array}{}
\dot{x}=0\\
f(x,\dot{x})=0
\end{array}\right.的点\Leftrightarrow 满足\left\{\begin{array}{}
\dot{x}=0\\
\ddot{x}=0
\end{array}\right.的点$$
$$注：线性二阶系统只有一个平衡点（一个奇点），即原点(x,\dot{x}_0)=(0,0)$$

## 二阶系统相平面图

<img src=pic-principal-of-automation-control\Markji_1751375117094.png width="49%"><img src=pic-principal-of-automation-control\Markji_1751375123932.png width="50%">
$$相轨迹运动方向：
\left\{\begin{array}{}
\dot{x}>0&上半平面向右\\
\dot{x}<0&下半平面向左
\end{array}
\right.$$
$$\star渐近线：\dot{x}=\lambda_1x,\quad \dot{x}=\lambda_2x$$

## 相平面分析基本概念

$$仅适用于一阶、二阶形如\ddot{x}=f(\dot{x},x)线性，或非系统的分析$$

## 相平面绘制的两大方法

**相轨迹绘制基本只用分段线性化，特别要求时才用等倾斜线法**
$$分段线性化（解析法）：\\
形如\ddot{x}+f(x,\dot{x})=0的方程
\ \\
\left\{
\begin{array}{ll}
\dot{x}=0\\
\ddot{x}=0
\end{array}
\right.代入原方程解x_0,
在奇点(x_0,\dot{x}_0)即(x_0,0)处线性化：\\

 s^2+as+b=0\left\{\begin{array}{l}
a=\frac{\partial{f}}{\partial{\dot{x}}}\big|_{(x_0,\dot{x}_0)}\\

b=\frac{\partial{f}}{\partial{x}}\big|_{(x_0,\dot{x}_0)}
\end{array}\right.\quad 即(x-x_0)''+\frac{\partial{f}}{\partial{\dot{x}}}\big|_{(x_0,\dot{x}_0)}(x-x_0)'+\frac{\partial{f}}{\partial{x}}\big|_{(x_0,\dot{x}_0)}(x-x_0)=0$$
$$等倾斜线法（图解法）：适用范围有限\\
{\color{blue}前提：}可化为等倾斜线方程的形式\\
\ddot{x}+\dot{x}+x=0\qquad {\color{blue}相轨迹方程}\\
令\frac{d\dot{x}}{dx}=\frac{-\dot{x}-x}{\dot{x}}=\alpha\\
\ \\
\left\{\begin{array}{l}
\dot{x}=-\frac{1}{\alpha+1}x（-\frac{1}{\alpha+1}为倾斜线的斜率）\qquad {\color{blue}等倾斜线方程}\\
\ \\
\frac{d\dot{x}}{dx}=\alpha（经过\dot{x}=-\frac{1}{\alpha+1}x倾斜线的曲线斜率为\alpha）

\end{array}\right.$$

## 本质非线性与非本质非线性分析

$$本质非线性系统：未经过线性化处理，准确的相轨迹\\
例：\ddot{x}+\dot{x}+|x|=0\quad
\left\{\begin{array}{l}
\ddot{x}+\dot{x}+x=0 & x>0\\
\ddot{x}+\dot{x}-x=0 &x<0
\end{array}\right.\qquad {\color{blue}开关线方程\ x=0}$$
$$非本质非线性方程：经过线性化处理，近似的相轨迹\\
例：\ddot{x}+3\dot{x}+x^2=0\\
在奇点(0,0)处线性化：\ddot{x}+3\dot{x}=0$$

## 非线性微分方程的相平面分析

$$光滑、无法分区间讨论情形：绘制奇点附近的相轨迹\\
1.\ddot{x}+f(x,\dot{x})=0求奇点(x_0,\dot{x}_0)\\
2.奇点附近线性化\quad
(x-x_0)''+\frac{\partial{f}}{\partial{\dot{x}}}\big|_{(x_0,\dot{x}_0)}(x-x_0)'+\frac{\partial{f}}{\partial{x}}\big|_{(x_0,\dot{x}_0)}(x-x_0)=0\\
3.拉氏变换求特征根，对比二阶线性系统特征根，判断奇点类型，对应绘制$$
$$划分区域讨论情形： 分别绘制不同区间在奇点附近的相轨迹\\
例：\ddot{x}+\dot{x}+|x|=0\\
\left\{\begin{array}{}
\ddot{x}+\dot{x}+x=0 & x\geqslant 0\\
\ddot{x}+\dot{x}-x=0 & x< 0
\end{array}
\right.$$

## 非线性控制框图的相平面分析

$$给定输入r(t)，根据控制系统框图列写：关于误差e的微分方程（探讨e的性质）\\
\left\{\begin{array}{ll}
\ddot{e}=0 & |e|<2\\
\ddot{e}+e-2=0 & e>2\\
\ddot{e}+e+2=0 & e<-2
\end{array} \right.
\xrightarrow{奇点处线性化}
\left\{\begin{array}{lll}
s^2=0 &奇点(C,0)& |e|<2\\
s^2+1=0 & 奇点(2,0) & e>2\\
s^2+1=0 & 奇点(-2,0)& e<-2
\end{array} \right.\\
各区域在对应奇点处分别线性化，得特征方程\\
利用二阶系统相平面图分段绘制奇点附近的相轨迹$$

## 描述函数定义与性质

$$定义：非线性环节在正弦输入f(t)=A\sin\omega t下的基波y(t)=Y\sin(\omega t+\phi)\\
\left\{\begin{array}{}
N(A)为一复变函数\\
|N(A)|=\frac{Y}{A},\,\quad \angle N(A)=\phi
\end{array}\right.$$
[Card#ID/2gNcZ#描述函数的计算]
$$性质：
\left\{\begin{array}{}N(A)=N_1(A)+N_2(A)\\
N(A)\neq N_1(A)\times N_2(A)
\end{array}\right.\\
当非线性特性为单值奇函数时，A_1=0，即N(A)为实数\\
{\color{blue}易混点：y(t)周期仅与\omega有关，与非线性环节无关}$$
$$注：非线性环节应为奇对称，保证直流分量A_0为0\\
\ \\{\color{blue}此情形考研不涉及}-当非线性环节包含储能环节，即N特性用微分方程描述时\\
描述函数才是关于A与\omega的函数，记为N(A,\omega)$$

## 描述函数的计算

$${\color{blue}一般描述函数N(A)与\omega无关，仅与A有关，输入为x(t)=A\sin t即可}$$
$$在正弦输入x(t)=A\sin t{\color{blue}（A>0）}下，根据非线性环节得出y(t)表达式\\
\\

y(t)=A_1\cos t+B_2\sin  t=Y\sin( t+\phi)\\
\ \\
\left\{\begin{array}{l}
Y=\sqrt{A_1^2+B_1^2}\quad \phi=\arctan\frac{A_1}{B_1}\\
\ \\
N(A)=\frac{B_1+jA_1}{A}=\frac{Y}{A}\angle\phi
\end{array}\right.
\left\{\begin{array}{l}
A_1=\frac{1}{\pi}\int_0^{2\pi}y(t)\cos t\ dt\\
\ \\
B_1=\frac{1}{\pi}\int_0^{2\pi}y(t)\sin t\ dt\\
\end{array}\right.（灵活利用奇偶性）
$$
$$注：物理意义上，t>0，故积分区间应该(0,\quad)\\
$$

## 典型非线性特性及负倒描述函数

**考试不一定提供描述函数，单值描述函数及表达式均须记忆**
![](pic-principal-of-automation-control\Markji_1751375154647.png)
$$死区特性：N(A)=\frac{2k}{\pi}\left[\frac{\pi}{2}-\arcsin(\frac{a}{A})-\frac{a}{A}\sqrt{1-(\frac{a}{A}^2)}\right]\\
立方函数(y=x^3)：N(A)=\frac{3}{4}A^2\\
一般非线性(y=\frac{1}{2}x+\frac{1}{4}x^3)：N(A)=\frac{1}{2}+\frac{3}{16}A^2$$
$$注：单值非线性描述函数为实数，多值非线性描述函数为复数\\
考查多值特性时会补充条件，一般不考$$

## 极限环与自持振荡定义

$$离开极限环均在轻微扰动下发生\\
\ \\
稳定的极限环：t\to \infty时，所有轨迹均收敛于它\\
不稳定的极限环：t\to \infty时，所有轨迹均远离它\\
半稳定的极限环：t\to \infty时，部分轨迹收敛于它，部分轨迹远离它$$
$$自持振荡（自激振荡）：\\
在没有外界周期变化信号的作用时，系统内产生的具有固定频率和振幅的周期运动$$
$$注：哈工大教材定义，自持振荡为稳定的极限环(\text{page\ 409})$$

## 描述函数法判定自持振荡

**灵活结合使用，考查情形不会太复杂**
$$传递函数通法\quad
\Phi=\frac{G_1}{1+G_1+G_1G_2G_3N(A)}\\
列写特征方程：D(s)=1+G_1+G_1G_2G_3N(A)=0（未约分直接列写）\\
利用\frac{G_1G_2G_3}{1+G_1}=-\frac{1}{N(A)}判断\\
令G=\frac{G_1G_2G_3}{1+G_1}
\left\{
\begin{array}{l}
G(j\omega)不包围-\frac{1}{N(A)} &稳定\\
G(j\omega)包围-\frac{1}{N(A)} & 不稳定\\
G(j\omega)与-\frac{1}{N(A)}相交 & 极限环（可能自持振荡）\\
\end{array}（包围方向等勿要考虑）
\right.$$
$$非线性环节等效标准化（关于稳定性判别的等效）：\\
按信号流向先等效为一个前向通路的非线性环节（{\color{blue}r=0可忽略}，乱序会导致等效结果不同）\\
且反馈通路为单位负反馈，等效后用G(j\omega)=-\frac{1}{N(A)}判断$$
$$自持振荡（稳定极限环）判定：由包围区域至不包围区域的交点$$
$$注：描述函数法为工程近似方法，{\color{blue}会使用即可}，理论问题不清晰
$$

## 等效线性部分传函

![](pic-principal-of-automation-control\Markji_1751375184962.png)
$$传递函数通法求等效传递函数结果不唯一\\
\Phi(s)=\frac{G_1}{1+G_1+G_1H_1N(A)}
\left\{\begin{array}{ll}
前向通路：N(A)\#\frac{G_1}{1+G_1}& 回路：H_1\\
前向通路：\frac{G_1}{1+G_1} & 回路：N(A)\# H_1
\end{array}\right.
$$

## 自持振荡的振幅与角频率

$$-\frac{1}{N(A)}在实轴上（只考此情形）：\\
令G(j\omega)的虚部为零，解\omega\\
代入G(j\omega)=-\frac{1}{N(A)}，解A即可$$

## 非线性控制框图处理典例1

![](pic-principal-of-automation-control\Markji_1751375203973.png)![](pic-principal-of-automation-control\Markji_1751375210695.png)
$$注：框图处理的“决断点”在b处，可上升为一般特点，灵活分析$$

## 非线性控制框图处理典例2

![](pic-principal-of-automation-control\Markji_1751375234726.png)
$$0.5\ddot{c}+\dot{c}=u=
\left\{\begin{array}{}
8e_1,&|e_1|<0.5\\
4,&e_1>0.5\\
-4,&e_1<-0.5
\end{array}\right.\quad

关系式\left\{\begin{array}{l}
e_1=-0.5\dot{c}-c\\
c=-e
\end{array}\right.\\

代入整理得：-0.5\ddot{e}-\dot{e}=
\left\{\begin{array}{}
0.5\dot{e}+e,& |0.5\dot{e}+e|<0.5\\
4,& 0.5\dot{e}+e>0.5\\
-4,& 0.5\dot{e}+e<-0.5
\end{array}\right.$$

## 相轨迹分析系统性能指标

**所见即所得**
![](pic-principal-of-automation-control\Markji_1751375259028.png)

## 描述函数法信号关系典例

![](pic-principal-of-automation-control\Markji_1751375276446.png)
![](pic-principal-of-automation-control\Markji_1751375282452.png)
$$等效处理，线性部分G(s)=\frac{10ke^{-\tau s}}{s(s+2)^2}$$
$$(1)\quad G(s)=\frac{10k}{s(s+2)^2}\Rightarrow G(j\omega)=\frac{10k}{-4\omega^2+j(4\omega-\omega^3)}\\
令\text{Im}[G(j\omega)]=0，得\omega=2，此时G(j\omega)=-\frac{5k}{8}\\

\left\{\begin{array}{l}
自振：-\frac{1}{N(A)}=-\frac{5k}{8}\Rightarrow k=\frac{2\pi}{5}A\\
\ \\
输入振幅：A= \frac{10}{4}
\end{array}\right.

\left\{\begin{array}{l}
k=\pi\\
A=\frac{5}{2}
\end{array}\right.$$
$$(2)\quad G(j\omega)与-\frac{1}{N(A)}相交（即实轴相交）：\\
\varphi(\omega)\big|_{\omega=1}=-90\degree-2\arctan\frac{1}{2}-57.3\degree \tau=-180\degree\Rightarrow \tau=0.643\\
\ \\
G(j)=-\frac{1}{N(A)}=-\frac{5}{8}\pi\Rightarrow -k=-\frac{5\pi}{16}，即k=0.98$$
$$注：c(t)振幅仅在暗示A的大小，
不可按频率特性传递分析，按自振G(j\omega)=-\frac{1}{N(A)}解参数即可（理论问题不清晰）$$

## 微分方程的描述函数分析典例1

$$系统满足方程\ddot{x}+\dot{x}+x-\frac{1}{2}x^3=0$$

![](pic-principal-of-automation-control\Markji_1751375306088.png)

$$\ddot{x}+\dot{x}+x=-\frac{1}{2}(-x)^3=y\\
\ \\
等效为两部分
\left\{\begin{array}{l}
线性部分：\ddot{x}+\dot{x}+x=y\Rightarrow
G(s)=\frac{X(s)}{Y(s)}=\frac{1}{s^2+s+1}
\\
\ \\
非线性部分：-\frac{1}{2}(-x)^3=y\Rightarrow N(A)=-\frac{1}{2}x^3
\end{array}\right.$$

## 微分方程的描述函数分析典例2

![](pic-principal-of-automation-control\Markji_1751375324435.png)
<img src=pic-principal-of-automation-control\Markji_1751375333501.png width="50%"><img src=pic-principal-of-automation-control\Markji_1751375338988.png width="48%">

# 横向知识点对比

## 稳定判据对比

$$劳斯稳定判据\\
\ \\
\text{Nyquist}稳定判据\\
\ \\
对数稳定判据\\
\ \\
相角裕度、幅值裕度$$

## 临界稳定反求参数

$$\left\{\begin{array}{l}
劳斯判据（全零行）：D(s)=0\\
特征方程D(j\omega)=0：实部、虚部均为0
，可解得参数与振荡\omega
\end{array}\right.$$
$$\text{Nyquist}稳定判据：G(j\omega)虚部为0，实部为-1，可解得参数与振荡\omega\quad （分类讨论，具体情况具体分析）
$$

# 备用知识点

## 典型环节传递函数

**典型问题：已知模型，构造系统**
$$G(s)=-\frac{R_2}{R_1}\qquad G(s)=-\frac{1}{R_1C_1s}\qquad G(s)=-\frac{R_2}{R_1(R_2C_2s+1)}$$
<img src=pic-principal-of-automation-control\Markji_1751375386725.png width="32%"><img src=pic-principal-of-automation-control\Markji_1751375392653.png width="35%"><img src=pic-principal-of-automation-control\Markji_1751375398308.png width="32%">

## Nyquist稳定判据证明

$$F(s)=1+G(s)H(s)=\frac{D(s)}{N(s)}$$
$$
\omega:0\to +\infty

\left\{\begin{array}{l}
\Delta\angle D(s)=(n-z)\frac{\pi}{2}-z\frac{\pi}{2}=(n-2z)\frac{\pi}{2}\\
\ \\
\Delta\angle N(s)=(n-p)\frac{\pi}{2}-p\frac{\pi}{2}=(n-2p)\frac{\pi}{2}\\
\ \\
\Delta\angle F(s)=(n-2z)\frac{\pi}{2}-(n-2p)\frac{\pi}{2}=(p-z)\pi
\end{array}\right.故Z=P-2N_1（N_1表示包围圈数，逆正顺负）$$
$$\omega:-\infty\to +\infty

\left\{\begin{array}{l}
\Delta\angle D(s)=(n-z)\pi-z\pi=(n-2z)\pi\\
\ \\
\Delta\angle N(s)=(n-p)\pi-p\pi=(n-2p)\pi\\
\ \\
\Delta\angle F(s)=(n-2z)\pi-(n-2p)\pi=(p-z)2\pi
\end{array}\right.故Z=P-N_2（N_2表示包围圈数，逆正顺负）$$

## 截止频率范围确定补充

$$G(s)=\frac{K}{s(\frac{s}{\omega_1}+1)(\frac{s}{\omega_2}+1)[(\frac{s}{\omega_3})^2+2\xi\frac{s}{\omega_n}+1]}
$$
$$试探反解：
令A(\omega_c)=\frac{K}{\omega_c\cdot \frac{\omega_c}{\omega_1}}=1，若\omega_1<\omega_c<\omega_2，即为所求\\
若L(\omega)单减不增，
\left.\begin{array}{l}
\omega_c<\omega_1\\
\omega_c>\omega_2
\end{array}\right\}即为所求，需另确定范围$$

## 朱利稳定判据
稳定要求、朱利表列法

$$稳定要求：\\
1. D(1)>0\\
2. 最高次幂：\left\{\begin{array}{}奇数，D(-1)<0\\偶数，D(-1)>0\end{array}\right.\\
3. 朱利表第一组首列"<"，其余行首列">"

$$
$$朱利表列法（剩三列为止）：\\
\begin{array}{}
   & Z^0 & Z^1 & Z^2 & Z^3 \\
1 & -39 & 119 & -117 & 45 \\
2 & 45 & -117 & 119 & -39 \\
\\
3
&
\underbrace{ \left|\begin{array}{}
-39 & 45 \\ 45 & -39
\end{array}\right|}_{-504} &   \underbrace{\left|\begin{array}{}
-39 & -117\\ 45 & 119
\end{array}\right|}_{624}
&  
\underbrace{\left|\begin{array}{}
-39 & 119\\ 45 & -117
\end{array}\right|}_{-792}\\
\ \\
4 &-792 & 624 &-504 \\
\\
5 & \cdots
\end{array}$$

## Z正反变换留数法

**怀疑此方法有问题**
$$Z变换：\text{Res}[E(s) \cdot \frac{z}{z-e^{Ts}}]=\frac{1}{(r-1)!}\lim\limits_{s\to s_i}\frac{d^{r-1}}{ds^{r-1}}[(s-s_i)^r \cdot  E(s) \cdot \frac{z}{z-e^{Ts}}]（对s求导，z视作常数）$$
$$Z反变换：\\
单根\text{ Res}[E(z)z^{n-1}]=\lim\limits_{z\to z_i}[(z-z_i) \cdot E(z) \cdot z^{n-1}]\\

重根\text{ Res}[E(z)z^{n-1}]=\frac{1}{(r-1)!}\lim\limits_{z\to z_i}\frac{d^{r-1}}{dz^{r-1}}[(z-z_i)^r \cdot E(z) \cdot z^{n-1}]$$
$$注：具体原理未知，且与部分分式所得结果不同$$

## 离散根输出求解

$$Y(z)=\Phi(z)R(z)=\frac{k\prod_{i=1}^m(z-z_i)}{\prod_{j=1}^n(z-p_j)}\frac{z}{z-1}\\
当特征方程{\color{blue}无重根时}：Y(z)=\frac{Az}{z-1}+\sum_{j=1}^n\frac{B_j z}{z-p_j}\\
瞬态分量\left\{
\begin{array}{l}
实根：y(kT)=\sum_{j=1}^nB_j\ p_j^k\\
\ \\
复根（偏，无须掌握）：y(kT)=\sum_{j=1}^nC_j\lambda_j^k\cos(k\theta_j+\phi_j)\\ p_j=a\pm jb\quad\lambda_j=\sqrt{a^2+b^2}=|p_j|\quad\theta_j=\arctan\frac{b}{a}
\end{array}
\right.$$

## 离散系统频率分析法

**方法简单，但原理未知，考频低，姑且搁置**
$$G(z)=K\frac{0.368(z+0.7)}{z^2-1.368z+0.368}利用频率分析系统稳定性$$

## 相平面分析典例

$$典例（难点）：摩擦非线性特性的随动系统，
速度反馈的非线性控制系统$$

## 自持振荡的必要条件

$$\frac{N(A)G(j\omega)R}{1+N(A)G(j\omega)}=C
\longrightarrow [N(A)\cdot G(j\omega)+1 ]C=N(A)\cdot G(j\omega)R\\
R=0且t\to \infty时（激励响应消失）\\
C\neq0且[N(A)\cdot G(j\omega)+1]=0 \Leftrightarrow 系统存在极限环\\
\ \\
\ [N(A)\cdot G(j\omega)+1]=0为自持振荡的必要条件
$$

## 傅里叶公式推演

$$A_1=\frac{1}{l}\int_0^{2l}y(t)\cdot\cos\frac{\pi}{l} t\ dt\xlongequal{\omega=\frac{\pi}{l}}\frac{\omega}{\pi}\int_0^\frac{2\pi}{\omega}y(t)\cos\omega t\ dt=\underbrace{\frac{1}{\pi}\int_0^\frac{2\pi}{\omega}y(t)\cos\omega t\ d(\omega t) \xlongequal{u=\omega t}\frac{1}{\pi}\int_0^{2\pi}y(\frac{u}{\omega})\cos u\ du}_{规范步骤}$$

## 离散稳定性的频率判别法

$$双线性变换z=\frac{w+1}{w-1}后，w视作s，对G(w)利用\text{Nyquist}判据或相角裕度判稳$$
$$注：未见考点姑且搁置$$

# 拓展知识点

欧拉公式

$$a+bj=re^{j\theta}
\left\{\begin{array}{}
r=\sqrt{a^2+b^2}\\
\theta=\arctan\frac{b}{a}
\end{array}
\right.$$

## 长除法

$$升阶长除法：商的阶数逐项递增\\
降阶长除法：商的阶数逐项递减$$

# 计算问题

## 不可使用计算器问题

$$情形一：数值会特别设置，便于计算\\
部分计算方式不统一的情形，也要灵活观察，选择题目暗示的计算方式
$$
$$情形二：数值确实较特殊，试卷会特别提供计算结果\\
也应注意观察，依照数值暗示进行计算，勿臆定$$

# 待处理问题

801控制原理迭代程度不高，理论与方法存在不完备问题
