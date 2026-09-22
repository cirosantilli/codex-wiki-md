<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a steady [flow network](../../../../../../flow-network.md), let each origin-destination class $k$ have fixed demand $d_k$. Route flows $h_r\geq0$ satisfy $\sum_{r\in R_k}h_r=d_k$. The link flow is $y_j=\sum_rA_{jr}h_r$, and a link has continuous travel delay $\ell_j(y_j)$. Its route delay is $c_r(h)=\sum_jA_{jr}\ell_j(y_j)$.

A [Wardrop equilibrium](../../../../../../wardrop-equilibrium.md) describes nonatomic traffic: each traveler is too small to alter aggregate delays by changing route. For each class there is a minimum delay $\lambda_k$ such that

$$
\boxed{h_r>0\Longrightarrow c_r(h)=\lambda_k,\qquad h_r=0\Longrightarrow c_r(h)\geq\lambda_k}.
$$

Thus all used routes of one class have equal minimum cost, and an unused route cannot offer a shorter trip. The condition concerns private travel time, rather than total network delay.

Equivalently, for every feasible route vector $\widetilde h$,

$$
\sum_r c_r(h)(\widetilde h_r-h_r)\geq0.
$$

Indeed, each used route has class minimum cost, so reallocating demand cannot reduce the cost evaluated at the original flows; conversely a positive flow on a non-minimum route gives an improving transfer. This [variational inequality](../../../../../../variational-inequality.md) form remains meaningful even when route costs are not separable link functions.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
