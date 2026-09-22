<h1 id="12f/solution">Solution</h1>

↑ **Parent:** [12F](../12f.md)

For a partition $D=\{a=x_0<x_1<\cdots<x_n=b\}$, put $\Delta x_k=x_k-x_{k-1}$ and

$$
m_k=\inf_{[x_{k-1},x_k]}f,\qquad M_k=\sup_{[x_{k-1},x_k]}f.
$$

Boundedness makes these finite. The [lower Darboux sum](../../../../../lower-darboux-sum.md) and [upper Darboux sum](../../../../../upper-darboux-sum.md) are

$$
\boxed{s(f,D)=\sum_{k=1}^nm_k\Delta x_k,\qquad S(f,D)=\sum_{k=1}^nM_k\Delta x_k.}
$$

Since $m_k\leq M_k$ and the widths are positive, $s(f,D)\leq S(f,D)$.

Splitting a partition interval into smaller intervals can only increase each infimum and decrease each supremum. The smaller widths sum to the original width. Its new lower contribution is therefore at least its old lower contribution, and its new upper contribution at most its old upper contribution. Repeating this for every inserted point proves [Darboux sum refinement monotonicity](../../../../../darboux-sum-refinement-monotonicity.md):

$$
\boxed{D\subseteq D'\ \Longrightarrow\ s(f,D)\leq s(f,D'),\quad S(f,D')\leq S(f,D).}
$$

For arbitrary partitions, take their common [partition refinement](../../../../../partition-refinement.md) $D_*=D_1\cup D_2$. Then

$$
\boxed{s(f,D_1)\leq s(f,D_*)\leq S(f,D_*)\leq S(f,D_2).}
$$

No compatibility of the original partitions is required.

Finally suppose $f\geq0$ is [Riemann integrable](../../../../../riemann-integrable-function.md). Then $t_k=m_k\Delta x_k\geq0$, so every product factor is nonnegative and the exponential inequality can be multiplied safely:

$$
p(f,D)=\prod_k(1+t_k)\leq\prod_ke^{t_k}=e^{s(f,D)}.
$$

A lower Darboux sum is no greater than the [Riemann integral](../../../../../riemann-integral.md), since the integral equals the supremum of all lower sums. Monotonicity of the exponential therefore gives the [exponential bound for a lower-sum product](../../../../../exponential-bound-for-a-lower-sum-product.md)

$$
\boxed{p(f,D)\leq\exp\left(\int_a^b f(x)\,dx\right).}
$$

For a degenerate interval $a=b$, the empty product and the exponential are both one.

## ↑ Ancestors (10)

1. [12F](../12f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
