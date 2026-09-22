<h1 id="5/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $Y_{it}\in\{0,1\}$ indicate a smoking-free week, $S_i$ the recorded sex indicator, $A_i$ age in years and $T_i$ assigned treatment. The screening history supplies $Y_{i0}=0$; earlier lag initializations are also zero. A [history-dependent logistic regression](../../../../../../../conditional-logistic-model-for-longitudinal-binary-data.md) for the first model is

$$
Y_{it}\mid\mathcal H_{i,t-1},S_i,A_i,T_i\sim\operatorname{Bernoulli}(p_{it}),\qquad
\log\frac{p_{it}}{1-p_{it}}=\beta_0+\beta_SS_i+\beta_AA_i+\beta_TT_i+\gamma Y_{i,t-1}.
$$

Here $t=1,\ldots,10$, $\mathcal H_{i,t-1}$ is the observed past, and the five unknown [regression coefficients](../../../../../../../regression-coefficient.md) have time-invariant values. Conditional on baseline [covariates](../../../../../../../covariate.md), this model has the first-order [Markov property](../../../../../../../markov-property.md): only the immediately preceding outcome enters the current conditional [probability](../../../../../../../probability.md). Distinct subjects have independent histories. There is no subject [random effect](../../../../../../../random-effect.md) or additional time trend in this fit.

Using the [chain rule for probabilities](../../../../../../../chain-rule-for-probabilities.md), the individual conditional [likelihood](../../../../../../../likelihood-function.md) is

$$
\boxed{L_i(\beta,\gamma)=\prod_{t=1}^{10}p_{it}^{y_{it}}(1-p_{it})^{1-y_{it}},\qquad
p_{it}=\frac{e^{\eta_{it}}}{1+e^{\eta_{it}}}.}
$$

The lagged values in $\eta_{it}$ are the individual's actual preceding outcomes. This product is a sequential conditional [likelihood](../../../../../../../likelihood-function.md), not an assertion of unconditional independence of the ten readings. The full conditional [likelihood](../../../../../../../likelihood-function.md) is $\prod_iL_i$; no extra [Bernoulli distribution](../../../../../../../bernoulli-distribution.md) factor is attached to the fixed screening history.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Paper 30](../../../../paper-30-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
