<h1 id="5/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose the unbounded [function](../../../../../../../function-split.md) $\boxed{g(x)=1/x}$ on $E=(0,1/2]$. It is unbounded because $g(1/k)=k$ for all [integers](../../../../../../../integer-split.md) $k\geq2$. For each $x\in E$, the [geometric series](../../../../../../../geometric-series.md) gives the sum and its remainder after degree $N$:

$$
\sum_{n=0}^{\infty}x^ng(x)=\frac1{x(1-x)},
\qquad
\frac1{x(1-x)}-\sum_{n=0}^Nx^{n-1}=\frac{x^N}{1-x}.
$$

Since $0<x\leq1/2$,

$$
\boxed{\sup_{x\in E}\left|\frac1{x(1-x)}-\sum_{n=0}^Nx^{n-1}\right|\leq2^{1-N}\longrightarrow0.}
$$

This proves [uniform convergence](../../../../../../../uniform-convergence.md). Although the first term $1/x$ and the sum are unbounded, the late tails have a bound tending to zero independently of $x$. [Uniform convergence](../../../../../../../uniform-convergence.md) concerns those tails and does not require the individual [functions](../../../../../../../function-split.md) to be bounded.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Mathematics II](../../../../mathematics-ii-split.md)
5. [Prelims](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
