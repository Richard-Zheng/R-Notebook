Field lines draw all of their validity from [Gauss's law for the electrostatic field](http://en.wikipedia.org/wiki/Gauss_law),

场线的有效性从静电场的高斯定律得出。
$$
\nabla\cdot \mathbf{E}=\frac1{\epsilon_0}\rho,\ \text{or equivalently}\ 
\oint_{\partial\Omega}\mathbf{E}\cdot\text d\mathbf{S}=\frac1{\epsilon_0}Q_\Omega,
$$
$Q_\Omega=\int_\Omega\rho\,\text d\mathbf{r}$ 体积为 $\Omega$ 而表面积为 $\partial \Omega$ 中的电荷量。它可以精确地映射到稳态下某些流体的连续性方程中，方程指出：
$$
\nabla\cdot \mathbf{j}=\sigma,\ \text{or equivalently}\ 
\oint_{\partial\Omega}\mathbf{j}\cdot\text d\mathbf{S}=\Sigma_\Omega
$$
$\mathbf{j}$ 指的是『流量密度』，也即单位时间内通过单位面积的流体量。$\sigma$ 指的是每单位体积每单位时间产生的流体量。而$\Sigma_\Omega=\int_\Omega\sigma\,\text d\mathbf{r}$ 是单位时间内在 $\Omega$ 中产生的流体量。

这两个形式完全相同的方程意味着：我们可以将电场有效地解释为虚构的“流体”的速度，该速度是否守恒取决于电荷是否存在。 更具体地说，我们可以引入一种有用的描述流体的方式——使用流线图，以帮助我们可视化电场（实际上，本文也适用于静磁场和引力场）。

然后，让我们使用上面的这种映射问题的方式，映射您的问题：“电场线图如何以及为什么起作用？”在转化为对应的问题：

> “流线图如何以及为什么起作用？”

流线图描绘的是有限数量的线，这些线在所有点均与那一点的 $\mathbf{j}=\rho_\text{fluid}\mathbf{v}$ 相切。 这表明，在流线上开始流动的粒子将会随着流体的流动一直停留在那条流线上。

![FluidFlow](https://i.stack.imgur.com/qYidM.jpg)

当流线突然彼此靠近时，事情就变得有趣起来。 这意味着要么流体被压缩，要么流体的单位体积被拉伸，从而沿流线更长（例如，如[该图](https://en.wikipedia.org/wiki/File:BernoullisLawDerivationDiagram.svg)所示），因此流体流动得更快。 不论哪种方式，流体电流密度 $|\mathbf{j}|$ 增加。

分析可以变得更加精确。例如，在上面的机翼图像中，选择了流线“种子”（在左侧的表示流线开始的点），以使两条相邻流线间，单位时间内流入此图片的流量是相等的。 因为没有流体流过流水线，所以该流体流率必须保持恒定。 因此，当流线更靠近时，每单位面积的流体流动速率（即电流密度）更大。

（除此之外，如果在某些地方产生或破坏了流体，那么您可能需要引入或删除一些流线，因为在这种情况下，原始流线之间的流体流率当然不再是守恒的。）