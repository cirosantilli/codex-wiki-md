<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First take a bounded elementary [predictable process](../../../../../../predictable-process.md) $\alpha=\sum_jK_j\mathbf1_{(s_j,t_j]}$, with each $K_j$ bounded and $\mathcal F_{s_j}$-measurable and with finite time support. The [Itô integral](../../../../../../ito-integral.md) is the corresponding finite sum $\sum_jK_j(W_{t_j}-W_{s_j})$. Applying part (a) term by term gives

$$
\mathbb E\left[\phi(W_T)\int_0^\infty\alpha_u\,dW_u\right]=\mathbb E\int_0^T\phi'(W_T)\alpha_u\,du.
$$

Such elementary [predictable processes](../../../../../../predictable-process.md) are dense among predictable processes in $L^2(d\mathbb P\,du)$. The [Itô isometry](../../../../../../ito-isometry.md) makes the left functional continuous, with bound

$$
\left|\mathbb E\left[\phi(W_T)\int\alpha\,dW\right]\right|\le\|\phi\|_\infty\left(\mathbb E\int_0^\infty\alpha_u^2\,du\right)^{1/2}.
$$

The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) makes the right functional continuous, with bound $\|\phi'\|_\infty\sqrt T\left(\mathbb E\int\alpha_u^2du\right)^{1/2}$. Approximation therefore proves **the same identity for every allowed predictable $\alpha$**. The integral over the infinite time interval is the $L^2$ limit of its finite-horizon [Itô integrals](../../../../../../ito-integral.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
