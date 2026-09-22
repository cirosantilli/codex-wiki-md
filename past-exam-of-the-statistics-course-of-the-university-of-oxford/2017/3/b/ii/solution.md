<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $A=a+s>1$ and $B=b+n-s>1$ as in part (a), and let $F_{A,B}$ be the [cumulative distribution function](../../../../../cumulative-distribution-function.md) of the [beta distribution](../../../../../beta-distribution.md) $\operatorname{Beta}(A,B)$. The two endpoint equations are

$$
\boxed{\begin{aligned}
F_{A,B}(\theta_2)-F_{A,B}(\theta_1)&=0.95,\\
\theta_1^{A-1}(1-\theta_1)^{B-1}
&=\theta_2^{A-1}(1-\theta_2)^{B-1}.
\end{aligned}}
$$

The first equation fixes the [posterior probability](../../../../../posterior-probability.md), and the second makes the two endpoint [posterior densities](../../../../../posterior-density.md) equal. Their admissible ordering is

$$
0<\theta_1<\frac{A-1}{A+B-2}<\theta_2<1.
$$

To justify sufficiency and uniqueness, the [derivative](../../../../../derivative.md) of the logarithm of the [posterior density](../../../../../posterior-density.md) is

$$
\frac{A-1}{\theta}-\frac{B-1}{1-\theta},
$$

which is positive below $m=(A-1)/(A+B-2)$ and negative above it. Thus the [posterior density](../../../../../posterior-density.md) increases strictly to its unique [mode](../../../../../mode-statistics.md) and decreases strictly thereafter, vanishing at both ends. Each density threshold $k$ between zero and the maximum determines exactly one endpoint on each side of $m$. The [probability](../../../../../probability.md) between these endpoints decreases continuously and strictly from one to zero as $k$ increases, so exactly one threshold gives 0.95. This is the [beta highest posterior density endpoint characterization](../../../../../beta-highest-posterior-density-endpoint-characterization.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
