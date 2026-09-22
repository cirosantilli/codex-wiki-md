<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $T_i=X_i+Y_i$. Since the two counts are independent [Poisson distributions](../../../../../../poisson-distribution.md) with means $\lambda_i$ and $\beta\lambda_i$, their total is a [Poisson distribution](../../../../../../poisson-distribution.md) with mean $(1+\beta)\lambda_i$. For a fixed observed total $t_i=x_i+y_i$, divide the joint [probability mass function](../../../../../../probability-mass-function.md) by that of the total:

$$
\Pr(Y_i=y_i\mid T_i=t_i)
=\frac{e^{-(1+\beta)\lambda_i}\lambda_i^{x_i}(\beta\lambda_i)^{y_i}/(x_i!y_i!)}
{e^{-(1+\beta)\lambda_i}[(1+\beta)\lambda_i]^{t_i}/t_i!}
=\binom{t_i}{y_i}\frac{\beta^{y_i}}{(1+\beta)^{t_i}}.
$$

Define $p=\beta/(1+\beta)$, so $1-p=1/(1+\beta)$. Then

$$
Y_i\mid T_i=t_i\sim\operatorname{Bin}(t_i,p).
$$

For independent patients, the [paired Poisson conditional likelihood](../../../../../../paired-poisson-conditional-likelihood.md) is

$$
\boxed{L_c(p)=\prod_i\binom{t_i}{y_i}p^{y_i}(1-p)^{t_i-y_i}
\ \propto\ p^{\sum_i y_i}(1-p)^{\sum_i x_i}.}
$$

Every nuisance rate $\lambda_i$ cancels, while each patient's own baseline count level is retained through the conditioning total. A patient with total zero would contribute the constant one.

For these data, $\sum_i x_i=161$, $\sum_i y_i=23$, and $\sum_i t_i=184$. Maximizing this [conditional likelihood](../../../../../../conditional-likelihood.md) gives

$$
\widehat p=\frac{23}{184}=\frac18,\qquad
\widehat\beta=\frac{\widehat p}{1-\widehat p}
=\frac{23}{161}=\frac17.
$$

These are the fit under the model without a cure component, not the estimates of the mixture model in the later parts.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
