<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write $a$ for the scalar intercept denoted $\mu$ in the question, to distinguish it from the individual means $\mu_i$. The [log-likelihood](../../../../../log-likelihood.md) of the [independent](../../../../../independent-random-variables.md) [Poisson observations](../../../../../poisson-observation.md) is

$$
\ell(a,\beta)=\sum_i\left[y_i(a+\beta x_i)-e^{a+\beta x_i}-\log(y_i!)\right].
$$

Differentiating gives the [score equations](../../../../../score-equation.md) for an interior [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md):

$$
\boxed{\sum_i(y_i-\widehat\mu_i)=0,\qquad
\sum_i x_i(y_i-\widehat\mu_i)=0,\qquad
\widehat\mu_i=e^{\widehat a+\widehat\beta x_i}.}
$$

In particular, when $m=\sum_i y_i>0$,

$$
e^{\widehat a}=\frac{m}{\sum_i e^{\widehat\beta x_i}},\qquad
\frac{\sum_i x_i e^{\widehat\beta x_i}}{\sum_i e^{\widehat\beta x_i}}
=\frac{\sum_i x_i y_i}{m}.
$$

The left side is a weighted covariate mean whose derivative is its weighted [variance](../../../../../variance-split.md), so it is strictly increasing when the covariates are not all equal. An interior solution is unique if the observed count-weighted mean is strictly between the smallest and largest covariates. At an extreme it may require a limiting slope, and if all counts are zero the maximum occurs as $a\to-\infty$, rather than at finite parameters. Constant covariates make the slope and intercept unidentifiable.

Put $S_j=\sum_i x_i^j\mu_i$. The negative [Hessian matrix](../../../../../hessian-matrix.md) is deterministic at given parameters and is also the [Fisher information matrix](../../../../../fisher-information-matrix.md):

$$
I(a,\beta)=\begin{pmatrix}S_0&S_1\\ S_1&S_2\end{pmatrix},\qquad
I(a,\beta)^{-1}=\frac1{S_0S_2-S_1^2}
\begin{pmatrix}S_2&-S_1\\-S_1&S_0\end{pmatrix}.
$$

Under the usual interior, increasing-information regularity for [asymptotic normality of a maximum likelihood estimator](../../../../../asymptotic-normality-of-a-maximum-likelihood-estimator.md), replace the unknown means by their fitted values and read the lower-right entry:

$$
\boxed{\operatorname{Var}(\widehat\beta)\approx
\frac{\sum_i\widehat\mu_i}{(\sum_i\widehat\mu_i)(\sum_i x_i^2\widehat\mu_i)-(\sum_i x_i\widehat\mu_i)^2}.}
$$

Equivalently, [Poisson slope information after eliminating an intercept](../../../../../poisson-slope-information-after-eliminating-an-intercept.md) is $\sum_i\mu_i(x_i-\bar x_\mu)^2$, with $\bar x_\mu=S_1/S_0$. This explains both the positive denominator for varying covariates and the loss of slope information when their spread is small.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 41](../../paper-41-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
