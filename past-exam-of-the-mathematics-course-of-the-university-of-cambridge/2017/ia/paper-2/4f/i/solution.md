<h1 id="4f/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Integrate the [joint probability density](../../../../../../joint-probability-density.md) over $y$ to obtain the [marginal density](../../../../../../marginal-density.md) of $X$:

$$
f_X(x)=\int_0^\infty xe^{-x(y+1)}\,dy=e^{-x},\qquad x>0.
$$

Thus $X$ has an [exponential distribution](../../../../../../exponential-distribution.md) of rate one. Dividing the [joint probability density](../../../../../../joint-probability-density.md) by this [marginal density](../../../../../../marginal-density.md) gives the [conditional density](../../../../../../conditional-density.md)

$$
\boxed{f_{Y\mid X=x}(y)=xe^{-xy}\mathbf1_{\{y\geq0\}},\qquad x>0.}
$$

Equivalently, $Y\mid X=x$ has an [exponential distribution](../../../../../../exponential-distribution.md) of rate $x$. The value at $x=0$ can be assigned arbitrarily: it is a probability-zero conditioning value and the density ratio there is not meaningful.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4F](../../4f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
