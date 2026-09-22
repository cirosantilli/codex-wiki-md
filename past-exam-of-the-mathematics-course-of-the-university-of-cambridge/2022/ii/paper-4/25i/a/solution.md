<h1 id="25i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [periodic Wirtinger inequality](../../../../../../periodic-wirtinger-inequality.md) says that if $f$ is continuously differentiable, $L$-periodic, and has mean zero, then

$$
\int_0^L f(s)^2\,ds
\leq \frac{L^2}{4\pi^2}\int_0^L f'(s)^2\,ds.
$$

Equality holds exactly for a linear combination of $\cos(2\pi s/L)$ and $\sin(2\pi s/L)$.

First suppose $\partial\Omega$ is one positively oriented simple closed curve, parametrized by [arc length](../../../../../../arc-length.md) as $\gamma(s)=(x(s),y(s))$ for $0\leq s\leq L$. Translating the origin, which changes neither length nor area, makes both $x$ and $y$ have mean zero. [Green theorem](../../../../../../green-theorem.md) and the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) give

$$
\begin{aligned}
2\operatorname{Area}(\Omega)
&=\int_0^L(xy'-yx')\,ds\\
&\leq
\left(\int_0^L(x^2+y^2)\,ds\right)^{1/2}
\left(\int_0^L((x')^2+(y')^2)\,ds\right)^{1/2}.
\end{aligned}
$$

Applying Wirtinger's inequality to both coordinate functions and using the unit-speed identity $(x')^2+(y')^2=1$ yields

$$
2\operatorname{Area}(\Omega)
\leq\frac{L}{2\pi}\,L,
$$

and therefore the [planar isoperimetric inequality](../../../../../../planar-isoperimetric-inequality.md)

$$
\boxed{4\pi\operatorname{Area}(\Omega)\leq L^2}.
$$

For several boundary components, apply the simple-curve result to the relevant enclosed regions and use $\sum_jL_j^2\leq(\sum_jL_j)^2$; holes only decrease the area.

Equality in both inequalities forces

$$
(x,y)=A\cos(2\pi s/L)+B\sin(2\pi s/L)
$$

for constant vectors $A,B$, with the unit-speed and Cauchy-Schwarz equality conditions making $A$ and $B$ perpendicular and equally long. Thus the boundary is a circle. Conversely, a circular domain has area $\pi R^2$ and perimeter $2\pi R$, so equality holds.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [25I](../../25i.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
