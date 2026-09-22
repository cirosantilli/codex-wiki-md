<h1 id="19h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $Q=\sum_i x_i^2>0$. Under the usual nondegenerate regression assumption $n>2$, maximizing the normal likelihood is equivalent to minimizing the [residual sum of squares](../../../../../../residual-sum-of-squares.md). The normal equations and $\sum_i x_i=0$ give the [maximum-likelihood estimators](../../../../../../maximum-likelihood-estimator.md)

$$
\boxed{\widehat\alpha=\overline Y,\qquad\widehat\beta=\frac{\sum_i x_iY_i}{Q}.}
$$

Write $A=\overline\varepsilon$ and $B=\sum_i x_i\varepsilon_i/Q$. Then $\widehat\alpha=\alpha+A$, $\widehat\beta=\beta+B$, and the residual is $r_i=\varepsilon_i-A-x_iB$. Independence of the errors gives

$$
\operatorname{Var}(A)=\sigma^2/n,\quad\operatorname{Var}(B)=\sigma^2/Q,\quad\operatorname{Cov}(A,B)=\frac{\sigma^2\sum_i x_i}{nQ}=0.
$$

For each $i$,

$$
\operatorname{Cov}(A,r_i)=\sigma^2/n-\sigma^2/n=0,\qquad\operatorname{Cov}(B,r_i)=\sigma^2x_i/Q-x_i\sigma^2/Q=0.
$$

Thus the three requested variables are pairwise uncorrelated.

They are linear functions of the jointly normal error vector. More strongly, the whole vector $(A,B,r_1,\ldots,r_n)$ has a [multivariate normal distribution](../../../../../../multivariate-normal-distribution.md), and its block covariances show that $A$, $B$ and the residual vector are independent, by [uncorrelated jointly normal variables are independent](../../../../../../uncorrelated-jointly-normal-variables-are-independent.md). Independence is preserved when applying a measurable function to the residual block. Hence

$$
\boxed{\widehat\alpha,\ \widehat\beta,\ \sum_i r_i^2\text{ are mutually independent}.}
$$

The residual projection is $I-\mathbf1\mathbf1^{\mathsf T}/n-xx^{\mathsf T}/Q$, of rank $n-2$, so additionally $\sum_i r_i^2/\sigma^2\sim\chi^2_{n-2}$. This is the [orthogonal projection of a Gaussian vector](../../../../../../orthogonal-projection-of-a-gaussian-vector.md) interpretation of the same result. The printed design conditions alone allow $n=2$; then the fit is exact, the positive-variance likelihood has no finite maximizer, and the residual test in part (b) is undefined. The standard testing question therefore needs $n>2$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [19H](../../19h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
