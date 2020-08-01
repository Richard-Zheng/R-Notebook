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

我们把 $d$ 看作「在它后面那个值附近的微小变化量」。也就是说，我们可以用极限表达这个意思：
$$
df\left( x\right) =\lim _{\Delta x\rightarrow 0}f\left( \Delta x+x\right) -f\left( x\right)
$$
这基本上就是一元微分的定义。此式表示什么意思？$f\left( \Delta x-x\right)$ 显然是将 $f\left( \Delta x\right)$ 沿 $x$ 轴平移 $x$ 个单位，随后则是沿 $y$ 轴平移 $-f\left( x\right)$ 个单位。因为后一项不包含 $\Delta x$ ，所以我们可以将它们直接视作一个整体求极限。而极限的结果很明显是0. 整体来看，它描述的就是 $f\left( x\right)$ 在 $x$ 附近的微小增量 $\Delta x$ 所引起的函数值变化的极限。

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

#### 极限

观察上面的推导过程，不难发现导数的定义是建立在**极限相除**的基础之上的。这也是极限最不同寻常的地方：极限相除时如果分子分母的极限值都为0，也能给出结果。而你能通过这个方法去度量「无穷小」。

我们度量的实际上是无穷小的「阶」。特别地，当除数为 $\lim _{x\rightarrow 0}x$ 时，得到的结果就定义为被除数的「阶数」。另外，当相除得到的结果为 $1$ 时，我们把分子分母称为「等阶无穷小」，也就是说这两个无穷小是等价的。

#### 什么是无穷小量？

来源Wikipedia：

**无穷小量**是数学分析中的一个概念，用以严格地定义诸如“最终会消失的量”、“绝对值比任何正数都要小的量”等非正式描述。在经典的微积分或数学分析中，无穷小量通常它以函数、序列等形式出现，例如，一个序列 $a=(a_{n})_{n\in \mathbb {N} }$ 若满足如下性质：

对任意的预先给定的正实数 $\varepsilon>0$ ，存在正整数 $N$ 使得
$$
|a_{k}|<\varepsilon
$$
在 $k>N$ 时必定成立；或用极限符号把上述性质简记为
$$
\lim_{n\to \infty} a_n = 0
$$
则序列 $a$ 被称为 $n\to \infty$ 时的无穷小量。