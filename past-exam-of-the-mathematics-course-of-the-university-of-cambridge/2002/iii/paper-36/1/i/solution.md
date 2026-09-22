<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $\mathbf1$ for the all-ones vector and set

$$
P_0=\frac{\mathbf1\mathbf1^{\mathsf T}}n,\qquad
P_X=X(X^{\mathsf T}X)^{-1}X^{\mathsf T},\qquad
\nu=n-p-1.
$$

The centering assumption makes $P_0P_X=0$. Thus the full [normal linear model](../../../../../../normal-linear-model.md) has fitted-value [orthogonal projection](../../../../../../orthogonal-projection.md) $P_0+P_X$, and its [residual sum of squares](../../../../../../residual-sum-of-squares.md) is $R=Y^{\mathsf T}(I-P_0-P_X)Y$. Assume $\nu>0$, as is needed to estimate the unknown error [variance](../../../../../../variance-split.md) from residuals.

For the null that all slopes vanish, the reduced fitted value is $\bar Y\mathbf1$, with residual sum of squares $R_0=Y^{\mathsf T}(I-P_0)Y$. The [F-test](../../../../../../f-test.md) is

$$
\boxed{F=\frac{(R_0-R)/p}{R/\nu}
=\frac{Y^{\mathsf T}P_XY/p}{R/\nu}\sim F_{p,\nu}\quad\text{under the null}}.
$$

Reject for an upper-tail value exceeding the $1-\alpha$ quantile of this [F-distribution](../../../../../../f-distribution.md). The required theorem is [Cochran's theorem](../../../../../../cochran-s-theorem.md): for an isotropic [normal distribution](../../../../../../normal-distribution.md), projections onto orthogonal subspaces are [independent](../../../../../../independent-random-variables.md), and the squared norm on a rank-$r$ subspace divided by $\sigma^2$ has a [chi-squared distribution](../../../../../../chi-squared-distribution.md) with $r$ degrees of freedom. Here the null makes the projected mean in $\operatorname{col}(X)$ zero, so $(R_0-R)/\sigma^2\sim\chi_p^2$, independently of $R/\sigma^2\sim\chi_\nu^2$.

Let $p_1,p_2$ be the numbers of columns in the two predictor blocks. To test the first block while retaining the second as nuisance, form

$$
P_2=X_2(X_2^{\mathsf T}X_2)^{-1}X_2^{\mathsf T},\qquad
R_2=Y^{\mathsf T}(I-P_0-P_2)Y.
$$

The [partial F-test for nested linear models](../../../../../../partial-f-test-for-nested-linear-models.md) is

$$
\boxed{F_1=\frac{(R_2-R)/p_1}{R/\nu}\sim F_{p_1,\nu}\quad\text{when }\beta_1=0}.
$$

Again reject in the upper tail. The difference of the nested fitted-value projections has rank $p_1$, is orthogonal to the full residual projection, and annihilates the null mean, which gives the same [independent](../../../../../../independent-random-variables.md) chi-squared argument. If a block has no columns, the corresponding test is vacuous.

The phrase [orthogonal statistical parameters](../../../../../../orthogonal-statistical-parameters.md) refers to zero cross-block [Fisher information](../../../../../../fisher-information-matrix.md), not to the numerical parameter vectors being perpendicular. In this model the cross-block information is $X_1^{\mathsf T}X_2/\sigma^2$, so the [orthogonal coefficient blocks in a centered normal linear model](../../../../../../orthogonal-coefficient-blocks-in-a-centered-normal-linear-model.md) condition is

$$
\boxed{X_1^{\mathsf T}X_2=0}.
$$

Then the two fitted subspaces are orthogonal, the block [least-squares estimators](../../../../../../ordinary-least-squares-estimators.md) have zero [covariance](../../../../../../covariance.md) and are [independent](../../../../../../independent-random-variables.md) because they are jointly Gaussian, and each block's [extra sum of squares](../../../../../../extra-sum-of-squares.md) is unchanged by including the other block. Centering also makes both blocks orthogonal to the intercept.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
