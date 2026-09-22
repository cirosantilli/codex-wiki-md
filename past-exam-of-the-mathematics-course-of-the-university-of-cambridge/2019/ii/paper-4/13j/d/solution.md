<h1 id="13j/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For $k=1,\ldots,C$, define the class degree sum

$$
T_k(y)=\sum_{i:z_i=k}\ \sum_{j:j\ne i}y_{\min(i,j),\max(i,j)},
$$

and define the number of within-college friendships by

$$
T_0(y)=\sum_{i<j}\delta_{z_i z_j}y_{ij}.
$$

Each between-college edge contributes once to the degree sum of each endpoint's college, while each within-college edge contributes twice to its college's degree sum. The model-3 likelihood can therefore be written

$$
L_3(\beta;y)
=\frac{
\exp\!\left\{\beta_0T_0(y)+\sum_{k=1}^C\beta_kT_k(y)\right\}}
{\displaystyle\prod_{i<j}
\left(1+e^{\beta_{z_i}+\beta_{z_j}+\beta_0\delta_{z_i z_j}}\right)}.
$$

The [Fisher-Neyman factorization theorem](../../../../../../fisher-neyman-factorization-theorem.md) shows that $T=(T_0,T_1,\ldots,T_C)$ is sufficient.

For two networks $y,y'$, the likelihood ratio is

$$
\frac{L_3(\beta;y)}{L_3(\beta;y')}
=\exp\!\left\{
\beta_0[T_0(y)-T_0(y')]
+\sum_{k=1}^C\beta_k[T_k(y)-T_k(y')]
\right\}.
$$

Because the parameters range independently over $\mathbb R^{C+1}$, this ratio is constant in $\beta$ exactly when every displayed difference vanishes. The [likelihood-ratio criterion for minimal sufficiency](../../../../../../likelihood-ratio-criterion-for-minimal-sufficiency.md) therefore gives the answer

$$
\boxed{T(y)=\bigl(T_0(y),T_1(y),\ldots,T_C(y)\bigr).}
$$

This is the [degree-sum sufficient statistic for an additive logistic network model](../../../../../../degree-sum-sufficient-statistic-for-an-additive-logistic-network-model.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [13J](../../13j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
