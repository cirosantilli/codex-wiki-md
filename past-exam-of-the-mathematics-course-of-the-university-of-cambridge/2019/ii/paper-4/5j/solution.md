<h1 id="5j/solution">Solution</h1>

↑ **Parent:** [5J](../5j.md)

A $(1-\alpha)$ [prediction interval](../../../../../prediction-interval.md) is a pair of statistics $L(Y),U(Y)$ such that, for every $\beta$ and $\sigma^2>0$, an independent future response $Y^*$ at the specified input satisfies

$$
\Pr_{\beta,\sigma^2}\{L(Y)\leq Y^*\leq U(Y)\}=1-\alpha.
$$

In the [normal linear model](../../../../../normal-linear-model.md), assume $X$ has full column rank and write

$$
\widehat\beta=(X^TX)^{-1}X^Ty,
\qquad
s^2=\frac{\|y-X\widehat\beta\|_2^2}{n-p}.
$$

For a new observation

$$
Y^*=x^{*T}\beta+\varepsilon^*,
\qquad
\varepsilon^*\sim N(0,\sigma^2),
$$

independent of the training sample, the prediction error is

$$
Y^*-x^{*T}\widehat\beta
=\varepsilon^*-x^{*T}(\widehat\beta-\beta).
$$

The two terms on the right are independent centered [normal random variables](../../../../../gaussian-random-variable.md), while

$$
\operatorname{Var}(\widehat\beta)=\sigma^2(X^TX)^{-1}.
$$

Consequently, with the new-point [regression leverage](../../../../../regression-leverage.md)

$$
h^*=x^{*T}(X^TX)^{-1}x^*,
$$

we have

$$
\frac{Y^*-x^{*T}\widehat\beta}{\sigma\sqrt{1+h^*}}\sim N(0,1).
$$

The assumption in the question gives

$$
\frac{(n-p)s^2}{\sigma^2}
=\frac{\|y-X\widehat\beta\|_2^2}{\sigma^2}
\sim\chi^2_{n-p}.
$$

This variable is independent of $\widehat\beta$; it is also independent of the new error $\varepsilon^*$. Therefore it is independent of the standardized prediction error, and the defining normal-over-chi-square representation of [Student's t-distribution](../../../../../student-s-t-distribution.md) gives

$$
\frac{Y^*-x^{*T}\widehat\beta}{s\sqrt{1+h^*}}
\sim t_{n-p}.
$$

If $t_{n-p,1-\alpha/2}$ is the corresponding upper quantile, symmetry yields

$$
\Pr\left(
\left|\frac{Y^*-x^{*T}\widehat\beta}{s\sqrt{1+h^*}}\right|
\leq t_{n-p,1-\alpha/2}
\right)=1-\alpha.
$$

Solving these inequalities for $Y^*$ proves that the [prediction interval in a normal linear model](../../../../../prediction-interval-in-a-normal-linear-model.md) is

$$
\boxed{
x^{*T}\widehat\beta
\mathbin\pm t_{n-p,1-\alpha/2}
s\sqrt{1+x^{*T}(X^TX)^{-1}x^*}.}
$$

Its center and endpoints depend only on the observed data and $x^*$, and the pivotal calculation proves the required coverage uniformly in the unknown $\beta$ and $\sigma^2$.

## ↑ Ancestors (10)

1. [5J](../5j.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
