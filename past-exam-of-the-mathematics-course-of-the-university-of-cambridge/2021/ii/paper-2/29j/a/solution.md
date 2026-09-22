<h1 id="29j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Kolmogorov-Smirnov theorem](../../../../../../kolmogorov-smirnov-theorem.md) states that, for continuous $F$,

$$
\sqrt n\sup_x|\widehat F_n(x)-F(x)|
\xrightarrow{d}\sup_{0\leq t\leq1}|B(t)|,
$$

where $B$ is a [Brownian bridge](../../../../../../brownian-bridge.md); the finite-sample law is also independent of continuous $F$. To test $H_0:F=F_0$, compute

$$
D_n=\sup_x|\widehat F_n(x)-F_0(x)|
$$

and reject when $\sqrt nD_n$ exceeds the appropriate null quantile.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [29J](../../29j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
