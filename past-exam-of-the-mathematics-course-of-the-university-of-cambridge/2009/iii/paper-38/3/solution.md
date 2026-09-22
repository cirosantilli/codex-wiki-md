<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $C_i$ be the disease count among $m_i$ miners in exposure group $i$, with representative exposure $t_i$, for $i=1,\ldots,8$. The [grouped-binomial logistic regression](../../../../../grouped-binomial-logistic-regression.md) is

$$
C_i\sim\operatorname{Bin}(m_i,p_i)\quad\text{independently},\qquad
\log\frac{p_i}{1-p_i}=\alpha+\beta t_i.
$$

The model assumes independent miners, a common disease probability within each group at its representative exposure, and binomial variation without an extra dispersion parameter. The use of average exposure is a grouping approximation, not a claim that every miner in a group has identical exposure. The input response is $C_i/m_i$ and `weights=miners` supplies the binomial denominators $m_i$, not inverse variances; together they yield this count [likelihood function](../../../../../likelihood-function.md). The default binomial link is the [logit link](../../../../../logit.md).

For $H_0:\beta=0$, the [likelihood-ratio test](../../../../../likelihood-ratio-test.md) compares the intercept-only model with the linear-exposure model. The reduction in [binomial deviance](../../../../../binomial-deviance.md) is

$$
\boxed{56.9028-6.0508=50.8520,\qquad \Delta\mathrm{df}=1,\qquad p\approx9.96\times10^{-13}.}
$$

Under the usual regular large-sample approximation it has a [chi-squared distribution](../../../../../chi-squared-distribution.md) with one [degree of freedom](../../../../../degree-of-freedom.md). There is very strong evidence of exposure dependence, with a positive estimated coefficient $\widehat\beta=0.09346$.

For goodness of fit against separate probabilities in all eight groups, the residual [binomial deviance](../../../../../binomial-deviance.md) $6.0508$ has approximately $8-2=6$ [degrees of freedom](../../../../../degree-of-freedom.md). Its upper-tail probability is about $0.418$, giving no evidence of lack of fit. This is an approximate check, particularly because the earliest exposure groups have small expected disease counts. It supports adequacy of this mean structure, not proof that all its assumptions or possible confounding variables have been addressed.

The `predict` call asks for a prediction at exposure $40$, sets `type="response"` to return the fitted probability rather than its [log odds](../../../../../log-odds.md), and requests the [standard error](../../../../../standard-error.md) of that fitted probability. It gives

$$
\boxed{\widehat p(40)=0.2576988,\qquad \operatorname{se}(\widehat p(40))=0.03637976.}
$$

For $z=(1,40)^T$, the [linear predictor](../../../../../linear-predictor.md) is $z^T\widehat\beta$, and the [delta method](../../../../../delta-method.md) gives

$$
\operatorname{se}(\widehat p)=\widehat p(1-\widehat p)\sqrt{z^T\widehat{\operatorname{cov}}(\widehat\beta)z}.
$$

The intercept-slope covariance is included in this expression. This measures uncertainty in the fitted mean probability; it is not the [standard deviation](../../../../../standard-deviation.md) of a new individual's binary disease outcome or of an unspecified new sample proportion.

The model's [odds](../../../../../odds.md) at exposure $t$ are $O(t)=e^{\alpha+\beta t}$. Hence $O(t+h)/O(t)=e^{h\beta}$, independently of $t$. By invariance of [maximum likelihood estimation](../../../../../maximum-likelihood-estimation.md), estimate this [odds ratio](../../../../../odds-ratio.md) by $e^{h\widehat\beta}$. A [Wald confidence interval](../../../../../wald-confidence-interval.md) for $\beta$ is $\widehat\beta\pm1.96\operatorname{se}(\widehat\beta)$; exponentiating its endpoints after multiplication by $h>0$ gives the interval for the multiplier. Using the printed coefficient and [standard error](../../../../../standard-error.md) $0.01543$ yields

$$
\boxed{\begin{array}{c|cc}
\text{exposure increase}&\text{odds multiplier}&95\%\text{ confidence interval}\\\hline
1\text{ year}&e^{0.09346}\approx1.098&\bigl(e^{0.09346-1.96(0.01543)},e^{0.09346+1.96(0.01543)}\bigr)\approx(1.065,1.132)\\
10\text{ years}&e^{0.9346}\approx2.546&\bigl(e^{10(0.09346-1.96(0.01543))},e^{10(0.09346+1.96(0.01543))}\bigr)\approx(1.882,3.445)
\end{array}}
$$

Thus the estimated odds rise by about $9.8\%$ per year, or by a factor about $2.55$ per decade. These are changes in odds, not fixed multiplicative changes in probabilities.

The second fit keeps the same independent [binomial distributions](../../../../../binomial-distribution.md) but permits a quadratic [linear predictor](../../../../../linear-predictor.md),

$$
\log\frac{p_i}{1-p_i}=\alpha+\beta t_i+\gamma t_i^2.
$$

In the sequential analysis, each exposure term adds one coefficient. With the first model's deviances, all nine missing entries are recovered in this completed table:

$$
\boxed{\begin{array}{c|rrrr}
\text{step}&\text{added df}&\text{deviance reduction}&\text{residual df}&\text{residual deviance}\\\hline
\text{intercept only}&-&-&7&56.9028\\
\text{add years}&1&50.8520&6&6.0508\\
\text{add years}^2&1&2.769&5&3.282
\end{array}}
$$

The final reduction is $6.0508-3.282\approx2.769$, with rounding to the precision of the printed output. Testing $\gamma=0$ therefore gives $p\approx0.096$ on one [degree of freedom](../../../../../degree-of-freedom.md). At the $5\%$ [significance level](../../../../../significance-level.md) I would retain the simpler linear-exposure model: it already fits adequately and the extra curvature is not clearly established. The quadratic fit does improve the likelihood somewhat; its [Akaike information criterion](../../../../../akaike-information-criterion.md) is about $0.77$ smaller, since $\Delta\mathrm{AIC}\approx-2.769+2$. Thus different reasonable selection criteria may weakly prefer different models, but these data do not give strong evidence that the additional term is necessary.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 38](../../paper-38-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
