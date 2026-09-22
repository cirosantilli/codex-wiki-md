<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The response errors have standard deviations proportional to $|\mu_i|$. Thus, when fitted means approximate the true means, increasing absolute [fitted values](../../../../../../fitted-values.md) tends to accompany increasing residual spread. A residual-versus-fitted plot shows a fan for positive means, or spread increasing away from zero for means of either sign. Standardization by one common residual standard deviation, even with the usual [regression leverage](../../../../../../regression-leverage.md) correction, does not remove this systematic [heteroscedasticity](../../../../../../heteroscedastic.md).

Under independent errors the exact [covariance matrix](../../../../../../covariance-matrix.md) after fitting is

$$
\operatorname{Cov}(\widehat\varepsilon)=G\,\operatorname{diag}(k\mu_1^2,\ldots,k\mu_n^2)\,G,
\qquad G=I-H,
$$

where $k>0$ is the common proportionality constant. Hence the simple fan description is a diagnostic tendency, not an assertion that each fitted residual has exactly [variance](../../../../../../variance-split.md) $k\mu_i^2$.

For positive responses, the intended [variance-stabilizing transformation](../../../../../../variance-stabilizing-transformation.md) is the [natural logarithm](../../../../../../natural-logarithm.md). The [delta method](../../../../../../delta-method.md) gives

$$
\operatorname{Var}(\log Y_i)\approx\frac{\operatorname{Var}(Y_i)}{\mu_i^2}=k,\qquad
\mathbb E(\log Y_i)\approx\log\mu_i-\frac{k}{2}.
$$

**Use $\log Y_i$ for positive data with modest relative error, then refit and check the transformed mean and residual structure.** In particular, if the original mean was $X_i^T\beta$, the transformed mean is approximately $\log(X_i^T\beta)-k/2$, not automatically a linear function of the original covariates.

There is a domain qualification in the literal printed model: a nondegenerate [normal distribution](../../../../../../normal-distribution.md) has negative support. For positive $\mu_i$, the probability of $Y_i\leq0$ is $\Phi(-1/\sqrt{k})$, so a real $\log Y_i$ is not defined throughout the stated sampling model. When $k$ is small this is a negligible-tail approximation, not an exact transformation to normal errors. If signed values must be retained and all $\mu_i\ne0$, write $Y_i=\mu_i(1+\sqrt{k}Z_i)$ with standard [normal](../../../../../../normal-distribution.md) $Z_i$. Then

$$
\log|Y_i|=\log|\mu_i|+\log|1+\sqrt{k}Z_i|.
$$

The second term has a common distribution with finite [variance](../../../../../../variance-split.md), so [log absolute value stabilization of a normal scale family](../../../../../../log-absolute-value-stabilization-of-a-normal-scale-family.md) is exact, but loses the sign of the mean and does not produce normal errors. Zeros and a zero mean are excluded from this transform. Alternatively retain the response scale and fit the stated variance model with [weighted least squares](../../../../../../weighted-least-squares.md) weights proportional to $1/\widehat\mu_i^2$ where the means stay away from zero. No arbitrary addition of a constant before taking logarithms exactly solves the given variance relation.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
