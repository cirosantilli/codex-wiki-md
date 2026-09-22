<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Differentiating the residualized objective gives

$$
\beta_4
=\frac{\mathbb E[\widetilde A\widetilde Y]}
{\mathbb E[\widetilde A^2]}
=\frac{\mathbb E[(A-e(X))(Y-\mu(X))]}
{\mathbb E[(A-e(X))^2]}
=\beta_3.
$$

This is the population [Frisch–Waugh–Lovell theorem](../../../../../../frisch-waugh-lovell-theorem.md).

For a [semiparametric estimator](../../../../../../semiparametric-estimator.md), estimate $e(x)=\mathbb E[A\mid X=x]$ and $\mu(x)=\mathbb E[Y\mid X=x]$ flexibly. With [cross-fitting](../../../../../../cross-fitting.md), obtain held-out predictions $\widehat e_i,\widehat\mu_i$ and regress the residualized outcome on the residualized treatment through the origin:

$$
\widehat\beta_3
=\frac{\sum_{i=1}^n(A_i-\widehat e_i)(Y_i-\widehat\mu_i)}
{\sum_{i=1}^n(A_i-\widehat e_i)^2}.
$$

Cross-fitting limits overfitting bias and permits flexible nuisance estimators under the usual convergence and overlap conditions.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [Paper 221](../../../paper-221-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
