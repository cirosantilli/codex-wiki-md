<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A Gaussian [generalised additive model](../../../../../../generalized-additive-model.md) with the identity link specifies

$$
\boxed{Y_i=\beta_0+\sum_{j=1}^p f_j(x_{ij})+\varepsilon_i,\qquad\varepsilon_i\text{ independent }N(0,\sigma^2).}
$$

The $f_j$ are unknown smooth functions estimated from the data, rather than necessarily straight lines. The model is additive in their effects, so it does not automatically contain [interactions](../../../../../../interaction-statistics.md) between [covariates](../../../../../../covariate.md). To identify the intercept separately from the smooths, impose a constraint such as $\sum_i f_j(x_{ij})=0$ for each $j$. Linear terms can also be included alongside smooth terms. More generally a specified [link function](../../../../../../link-function.md) can make $g(E(Y_i))$ additive; for the normal identity-link model the mean itself has the displayed form. Smoothness is typically controlled through a basis and a [roughness penalty](../../../../../../roughness-penalty.md), preventing an unrestricted smooth from interpolating all the noise.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
