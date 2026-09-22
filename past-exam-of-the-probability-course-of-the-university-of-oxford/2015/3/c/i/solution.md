<h1 id="3/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Since $Y_n\to+\infty$ [almost surely](../../../../../almost-sure-convergence.md), only finitely many early values can attain the global [minimum](../../../../../minimum-of-a-subset-of-a-total-order.md); it is a finite [integer](../../../../../integer-split.md). Also $W\leq Y_0=0$. For every [nonnegative integer](../../../../../natural-number.md) $m$, the unit-step property and translation invariance of the increments give

$$
\mathbb P(-W\geq m)
=\mathbb P_0(\text{ever visit }-m)
=\mathbb P_m(\text{ever visit }0)=\beta^m,
\qquad\beta=\frac{1-p}{p}.
$$

Subtracting consecutive tails yields the [probability mass function](../../../../../probability-mass-function.md)

$$
\boxed{\mathbb P(-W=m)=(1-\beta)\beta^m,\qquad m=0,1,\ldots.}
$$

Thus $-W$ has the [geometric distribution](../../../../../geometric-distribution.md) counting failures before the first success, with success parameter

$$
\boxed{1-\beta=\frac{2p-1}{p}.}
$$

This support convention is essential: the [minimum of an upward-biased random walk](../../../../../minimum-of-an-upward-biased-random-walk.md) can equal its starting position, so $-W=0$ has positive [probability](../../../../../probability.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
