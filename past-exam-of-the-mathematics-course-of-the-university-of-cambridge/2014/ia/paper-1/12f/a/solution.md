<h1 id="12f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a bounded real function on $[0,1]$, take a partition $P$ with nodes $0=x_0<\cdots<x_N=1$. Its [lower Darboux sum](../../../../../../lower-darboux-sum.md) and [upper Darboux sum](../../../../../../upper-darboux-sum.md) are

$$
L(f,P)=\sum_j\inf_{[x_{j-1},x_j]}f\,(x_j-x_{j-1}),\qquad
U(f,P)=\sum_j\sup_{[x_{j-1},x_j]}f\,(x_j-x_{j-1}).
$$

The function is [Riemann integrable](../../../../../../riemann-integrable-function.md) when $\sup_P L(f,P)=\inf_P U(f,P)$; their common value is its [Riemann integral](../../../../../../riemann-integral.md). Equivalently, for every $\eta>0$ some partition has $U-L<\eta$. Indeed a common refinement of nearly extremizing upper and lower partitions proves necessity, while arbitrarily small gaps force equality of the two integrals. This is the [Riemann integrability criterion](../../../../../../riemann-integrability-criterion.md).

A [continuous](../../../../../../continuous-function.md) function on a compact interval is bounded and [uniformly continuous](../../../../../../uniform-continuity.md). Choose a mesh small enough that its oscillation on each subinterval is less than $\eta$. Then $U-L\leq\eta\sum_j(x_j-x_{j-1})=\eta$; using $\eta/2$ first makes the desired inequality strict. Thus **every [continuous](../../../../../../continuous-function.md) function on $[0,1]$ is [Riemann integrable](../../../../../../riemann-integrable-function.md)**.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [12F](../../12f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
