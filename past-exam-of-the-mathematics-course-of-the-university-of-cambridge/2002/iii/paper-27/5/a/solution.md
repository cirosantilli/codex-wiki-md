<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $m_l=\lfloor Nt_l\rfloor-\lfloor Nt_{l-1}\rfloor$ and $\phi(v)=\mathbb E e^{iv\xi}$. Since $\mathbb E\xi=0$ and $\mathbb E\xi^2=1$, the [characteristic function](../../../../../../characteristic-function.md) expansion at zero is $\phi(v)=1-v^2/2+o(v^2)$. Indeed, $|e^{ix}-1-ix|\le x^2/2$ for real $x$, and $(e^{iv\xi}-1-iv\xi)/v^2\to-\xi^2/2$. The [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md), with dominating variable $\xi^2/2$, proves the expansion after taking expectations. Initially omit the endpoint interpolation terms. The integer-time increments involve disjoint sets of [independent](../../../../../../independent-random-variables.md) steps, so their joint [characteristic function](../../../../../../characteristic-function.md) is

$$
\prod_{l=1}^k\phi(\lambda_l/\sqrt N)^{m_l}.
$$

Here $m_l/N\to t_l-t_{l-1}$. Taking the logarithm near $1$ gives

$$
\sum_lm_l\log\phi(\lambda_l/\sqrt N)
\longrightarrow-\frac12\sum_l\lambda_l^2(t_l-t_{l-1}).
$$

This proves the claimed limit for the integer-time approximation.

At a fixed time $t$, the omitted endpoint term is $R_N(t)=N^{-1/2}(Nt-\lfloor Nt\rfloor)\xi_{\lfloor Nt\rfloor+1}$, and $\mathbb E|R_N(t)|^2\le1/N$. A fixed linear combination of the errors in the $k$ increments therefore tends to zero in $L^1$, by the triangle inequality and [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md), even when two endpoint terms share a step. Since $|e^{ix}-e^{iy}|\le|x-y|$, restoring interpolation changes the joint [characteristic function](../../../../../../characteristic-function.md) by a quantity tending to zero. Hence

$$
\boxed{\varphi^N_{t_1,\ldots,t_k}(\lambda_1,\ldots,\lambda_k)
\longrightarrow \exp\left(-\frac12\sum_{l=1}^k\lambda_l^2(t_l-t_{l-1})\right).}
$$

The limit is the joint [characteristic function](../../../../../../characteristic-function.md) of [independent](../../../../../../independent-random-variables.md) centered [normal](../../../../../../normal-distribution.md) increments with the indicated variances. By [Lévy continuity theorem](../../../../../../levy-continuity-theorem.md), the increment vectors converge in distribution to [Brownian increment](../../../../../../brownian-increment.md) vectors. The value vector is obtained by the fixed invertible triangular map of cumulative sums; thus the [continuous mapping theorem](../../../../../../continuous-mapping-theorem.md) gives convergence of $(S_{t_1}^N,\ldots,S_{t_k}^N)$ to $(B_{t_1},\ldots,B_{t_k})$. This proves every required [finite-dimensional distribution](../../../../../../finite-dimensional-distribution.md) limit. The finite [fourth moment](../../../../../../fourth-moment.md) is not needed for this part; it will give tightness in part (b).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
