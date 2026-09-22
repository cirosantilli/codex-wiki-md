<h1 id="4/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For the [geometric distribution](../../../../../../../geometric-distribution.md), $\mu=1/p$, so the [probability generating function](../../../../../../../probability-generating-function.md) of the [size-biased distribution](../../../../../../../size-biased-distribution.md) is

$$
G_{\widetilde Y}(s)=\frac{p^2s}{(1-qs)^2}.
$$

If $X_1,X_2$ are [independent and identically distributed](../../../../../../../independent-and-identically-distributed-random-variables.md) with [geometric distribution](../../../../../../../geometric-distribution.md) of parameter $p$, the [probability generating function of an independent sum](../../../../../../../probability-generating-function-of-an-independent-sum.md) gives

$$
G_{X_1+X_2-1}(s)=s^{-1}\left(\frac{ps}{1-qs}\right)^2
=\frac{p^2s}{(1-qs)^2}.
$$

At zero, interpret the expression by its continuous extension. The [probability generating functions](../../../../../../../probability-generating-function.md) agree, hence

$$
\boxed{\widetilde Y\overset d=X_1+X_2-1,\qquad X_1,X_2\sim\operatorname{Geom}(p)\text{ independently}.}
$$

One can also check the [probability mass functions](../../../../../../../probability-mass-function.md) directly: for $k\ge1$, there are $k$ positive integer pairs with sum $k+1$, each having [probability](../../../../../../../probability.md) $p^2q^{k-1}$. Thus both sides assign [probability](../../../../../../../probability.md) $kp^2q^{k-1}$ to $k$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Mathematics III](../../../../mathematics-iii-split.md)
5. [Prelims](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
