<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

With the stated flat priors, the full joint density, up to a constant, is

$$
\boxed{
\mathbf1_{\{\sigma^2>0,\tau^2>0\}}
\prod_{i=1}^N
N(x_i\mid\xi_i,\sigma_{x,i}^2)
N(y_i\mid\eta_i,\sigma_{y,i}^2)
N(\eta_i\mid\alpha+\beta\xi_i,\sigma^2)
N(\xi_i\mid\mu,\tau^2).}
$$

The priors on $\alpha,\beta,$ and $\mu$ contribute constants on $\mathbb R$, while those on the two variances contribute constants on $(0,\infty)$. These are [improper priors](../../../../../../improper-prior.md), so posterior propriety must be checked; the full-rank, sufficiently large-data case used below is proper.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
