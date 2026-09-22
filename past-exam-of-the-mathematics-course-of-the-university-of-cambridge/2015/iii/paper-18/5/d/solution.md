<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Choose a positive [Hermitian metric](../../../../../../hermitian-metric-on-a-holomorphic-vector-bundle.md) on $L$. Its curvature form $\omega=iF_h$ is a [Kähler form](../../../../../../kahler-form.md) on the compact [complex manifold](../../../../../../complex-manifold.md) of dimension one. Part (c) gives a threshold $k_0$ with $H^1(X,\mathcal O(L^k))=0$ for every $k\geq k_0$. We use this to prescribe a finite [principal part of a meromorphic section](../../../../../../principal-part-of-a-meromorphic-section.md).

Fix a smooth cutoff $\chi$ supported inside the given coordinate chart and equal to one near $x_0$. Let $P(z)=\sum_{j=-r}^{-1}a_jz^j$. On the punctured manifold define $t_k=\chi P(z)\zeta^k$ inside the chart, extended by zero outside. Its [Dolbeault operator](../../../../../../dolbeault-operator.md)

$$
\eta_k=\bar\partial_{L^k}t_k=(\bar\partial\chi)P(z)\zeta^k
$$

is smooth globally: it vanishes near the pole and near the boundary of the chart. It is $\bar\partial_{L^k}$-closed, either by the square-zero identity or because there are no $(0,2)$-forms in complex dimension one. The vanishing of $H^1(X,\mathcal O(L^k))$, together with the [Dolbeault theorem](../../../../../../dolbeault-theorem.md), therefore gives a global smooth section $u_k$ with $\bar\partial_{L^k}u_k=\eta_k$.

The section $s_k=t_k-u_k$ is holomorphic on $X\setminus\{x_0\}$. Near $x_0$, $\eta_k=0$, so $u_k=f_k(z)\zeta^k$ with $f_k$ holomorphic through zero. Its [Taylor series](../../../../../../taylor-series.md) then gives

$$
\boxed{s_k(z)=\left(\sum_{j=-r}^{-1}a_jz^j+\sum_{j\geq0}a_{jk}z^j\right)\zeta^k,\qquad z\ne0,}
$$

where the second series converges near zero and its coefficients are those of $-f_k$. The threshold is determined by the fixed bundle $L$ and $X$, and is independent of the prescribed coefficients. In fact the same threshold works for every finite pole order $r$, since the [Dolbeault cohomology](../../../../../../dolbeault-cohomology.md) obstruction is the same $H^1(X,L^k)$ for every such cutoff construction.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
