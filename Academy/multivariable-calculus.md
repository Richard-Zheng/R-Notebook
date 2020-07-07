# 多元微积分

## 对符号的理解

### 微分与极限

#### 微分

在数学中，微分是对函数的局部变化率的一种线性描述。

![Dydx_zh.jpg](https://i.loli.net/2020/07/07/W9H3CKd8ItlAYSb.jpg)

当某些函数 $\textstyle f$ 的自变量 $\textstyle x$ 有一个微小的改变 $\textstyle h$ 时，函数的变化可以分解为两个部分。

一个部分是线性部分：在一维情况下，它正比于自变量的变化量 $\textstyle h$，可以表示成 $\textstyle h$ 和一个与 $\textstyle h$ 无关，只与函数 $\textstyle f$及 $\textstyle x$ 有关的量的乘积；在更广泛的情况下，它是一个线性映射作用在 $\textstyle h$ 上的值。

另一部分是比 $\textstyle h$ 更高阶的无穷小，也就是说除以 $\textstyle h$ 后仍然会趋于零。当改变量 $\textstyle h$ 很小时，第二部分可以忽略不计，函数的变化量约等于第一部分，也就是函数在 $\textstyle x$ 处的**微分**，记作 $\displaystyle f'(x)h$ 或 ${\displaystyle \displaystyle {\textrm {d}}f_{x}(h)}$ 。如果一个函数在某处具有以上的性质，就称此函数在该点可微。

#### 以另一个角度理解符号 $d$

在很多地方，人们都倾向于把 $\dfrac {d}{dx}$ 当作一个运算符来理解。但是，我认为有些更简单的定义可以把相同的概念表述地很好：

我们把 $d$ 看作『在它后面那个值附近的微小变化量』。也就是说，我们可以用极限表达这个意思：
$$
df\left( x\right) =\lim _{\Delta x\rightarrow 0}f\left( \Delta x+x\right) -f\left( x\right)
$$
要注意的是，这里的 $d$ 已经**不再是微分**。此式表示什么意思？$f\left( \Delta x-x\right)$ 显然是将 $f\left( \Delta x\right)$ 沿 $x$ 轴平移 $x$ 个单位，随后则是沿 $y$ 轴平移 $-f\left( x\right)$ 个单位。因为后一项不包含 $\Delta x$ ，所以我们可以将它们直接视作一个整体求极限。而极限的结果很明显是0.

虽然这个单独的极限等于 $0$，但是当两个极限相除的时候，事情就变得不一样了。当 $f\left( x\right) =x$ 时，我们可以直接写出
$$
dx=\lim _{\Delta x\rightarrow 0}\left( \Delta x+x\right) -x=\lim _{\Delta x\rightarrow 0}\Delta x
$$
当 $f\left( x\right) =x^2$ 时，我们也可以写出
$$
dx^{2}=\lim _{\Delta x\rightarrow 0}\left( \Delta x+x\right) ^{2}-x^{2}
$$
两式相除，得：
$$
\begin{aligned}
\dfrac {dx^{2}}{dx}&=\dfrac {\lim _{\Delta x\rightarrow 0}\left( \Delta x+x\right) ^{2}-x^{2}}{\lim _{\Delta x\rightarrow 0}\Delta x}\\ 
&=\lim _{\Delta x\rightarrow 0}\dfrac {\left( x+\Delta x\right) ^{2}-x^{2}}{\Delta x }
\end{aligned}
$$
这正好是求导公式！