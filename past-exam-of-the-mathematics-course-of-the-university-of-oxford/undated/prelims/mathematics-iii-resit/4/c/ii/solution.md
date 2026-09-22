<h1 id="4/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Summing the [joint probability mass function](../../../../../../../joint-probability-mass-function.md) over $y$ with the [geometric series](../../../../../../../geometric-series.md) gives the [marginal probability mass function](../../../../../../../marginal-probability-mass-function.md)

$$
p_X(x)=\frac{(1-q)q^x}{1-q^{10}},\qquad x=0,\ldots,9.
$$

Divide the [joint probability mass function](../../../../../../../joint-probability-mass-function.md) by this positive [marginal probability mass function](../../../../../../../marginal-probability-mass-function.md) to obtain the [conditional distribution](../../../../../../../conditional-distribution.md):

$$
\boxed{\mathbb P(Y=y\mid X=x)=(1-q^{10})q^{10y},\qquad y\ge0,\quad0\le x\le9.}
$$

It is the [geometric distribution](../../../../../../../geometric-distribution.md) counting failures before the first success, with success [probability](../../../../../../../probability.md) $1-q^{10}$. For the other nonnegative integers $x\ge10$, $\mathbb P(X=x)=0$; the elementary [conditional probability](../../../../../../../conditional-probability.md) given $X=x$ is undefined and supplies no additional case.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [4](../../../4.md)
4. [Mathematics III resit](../../../../mathematics-iii-resit-split.md)
5. [Prelims](../../../../split.md)
6. [Undated](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
