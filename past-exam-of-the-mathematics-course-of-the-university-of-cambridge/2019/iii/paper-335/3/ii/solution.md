<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A [regularization of an inverse problem](../../../../../../regularization-of-an-inverse-problem.md) replaces the unbounded generalized inverse by bounded operators $R_\alpha:Y\to X$ satisfying $R_\alpha y\to A^\dagger y$ as $\alpha\downarrow0$ on admissible exact data. A [spectral regularization method](../../../../../../spectral-regularization-method.md) can be written

$$
\boxed{x_\alpha=R_\alpha y=\sum_j\frac{f_\alpha(\sigma_j)}{\sigma_j}\langle y,u_j\rangle v_j,}
$$

where $f_\alpha(\sigma)\to1$ for fixed $\sigma>0$ while $f_\alpha(\sigma)/\sigma$ remains bounded for each fixed $\alpha$. A uniform bound on $f_\alpha$ supplies the usual dominated-convergence argument on exact data.

This defines $f_\alpha$ as the dimensionless damping factor. In the alternative convention calling the entire inverse coefficient the [spectral filter](../../../../../../spectral-filter.md), that filter is $f_\alpha(\sigma)/\sigma$. For data error bounded by $\delta$, a sufficient [regularization parameter choice](../../../../../../regularization-parameter-choice.md) also requires $\delta\|R_{\alpha(\delta)}\|\to0$; consistency alone does not control noise.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
