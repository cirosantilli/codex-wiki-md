<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For [independent random variables](../../../../../../independent-random-variables.md) $Y_i\sim\operatorname{Bernoulli}(p_i)$, the full [logistic regression](../../../../../../logistic-regression.md) has [linear predictor](../../../../../../linear-predictor.md)

$$
\log\frac{p_i}{1-p_i}=\beta_0+\beta_1x_i+\beta_B\mathbf1_{\{L_i=B\}}+\beta_C\mathbf1_{\{L_i=C\}}.
$$

Layout A is the [reference level in a regression factor](../../../../../../reference-level-in-a-regression-factor.md). The smaller model sets $\beta_B=\beta_C=0$, leaving the same [logit link](../../../../../../logit.md) and the price predictor. In either case

$$
\ell(p)=\sum_i[y_i\log p_i+(1-y_i)\log(1-p_i)].
$$

The [saturated statistical model](../../../../../../saturated-statistical-model.md) allows a separate probability per observation; its maximizing probabilities are $p_i=y_i$, with [log-likelihood](../../../../../../log-likelihood.md) zero under $0\log0=0$. Hence the [binomial deviance](../../../../../../binomial-deviance.md) for either fitted model is

$$
\boxed{D=2(\ell_{\rm sat}-\ell_{\rm fit})=-2\sum_i[y_i\log\widehat p_i+(1-y_i)\log(1-\widehat p_i)].}
$$

Equivalently, write the summands as $2[y_i\log(y_i/\widehat p_i)+(1-y_i)\log((1-y_i)/(1-\widehat p_i))]$. The fitted probabilities differ between the two models, but the definition of [binomial deviance](../../../../../../binomial-deviance.md) is the same. A residual deviance for individual binary data need not itself have an accurate [chi-squared distribution](../../../../../../chi-squared-distribution.md) approximation; the nested-model difference used next has a different asymptotic justification.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
