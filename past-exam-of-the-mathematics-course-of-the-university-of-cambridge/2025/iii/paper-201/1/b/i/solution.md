<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a partition of $[a,b]$, every [Riemann sum](../../../../../../../riemann-sum.md) $S_n=\sum_jB_{t_j}\Delta t_j$ is a centered [Gaussian random variable](../../../../../../../normal-distribution.md), with

$$
\operatorname{Var}S_n=\sum_{i,j}\min(t_i,t_j)\Delta t_i\Delta t_j.
$$

Path continuity gives $S_n\to\int_a^bB_sds$ almost surely, and the covariance bound $\mathbb E|B_s-B_t|^2=|s-t|$ also gives convergence in $L^2$. Hence the limit is Gaussian, centered, and passage to the limit in the displayed sums gives variance

$$
\boxed{\int_a^b\int_a^b\min(s,t)\,ds\,dt.}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 201](../../../../paper-201-split.md)
5. [Iii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
