<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [kink in a phi-six model](../../../../../../kink-in-a-phi-six-model.md), choose the sector from $\phi=0$ to $\phi=2$ and the increasing sign of the [Bogomolny equation](../../../../../../bogomolny-equations.md):

$$
\phi'=\sqrt{2U(\phi)}
=\sqrt2\,\phi(4-\phi^2).
$$

For $y=\phi^2$ this becomes the [logistic differential equation](../../../../../../logistic-differential-equation.md)

$$
y'=2\sqrt2\,y(4-y).
$$

After translating the centre to $x_0$, its solution is

$$
\boxed{
\phi(x)=\frac2{\sqrt{1+e^{-8\sqrt2(x-x_0)}}}}.
$$

It tends to $0$ as $x\to-\infty$ and to $2$ as $x\to+\infty$. Spatial reflection and $\phi\mapsto-\phi$ generate the other kink and antikink sectors.

Because the first-order equation saturates the [Bogomolny bound](../../../../../../bogomolny-bound.md), its mass is

$$
\begin{aligned}
M&=\int_{-\infty}^{\infty}
\left[\frac12(\phi')^2+U(\phi)\right]dx
=\int_0^2\sqrt{2U(\phi)}\,d\phi\\
&=\sqrt2\int_0^2\phi(4-\phi^2)d\phi
=\boxed{4\sqrt2}.
\end{aligned}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 313](../../../paper-313-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
