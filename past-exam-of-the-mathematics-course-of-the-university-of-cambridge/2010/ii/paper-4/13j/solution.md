<h1 id="13j/solution">Solution</h1>

↑ **Parent:** [13J](../13j.md)

A natural [grouped-binomial logistic regression](../../../../../grouped-binomial-logistic-regression.md) assumes independent

$$
Y_i\sim\operatorname{Bin}(100,p_i),\qquad
\log\frac{p_i}{1-p_i}
=\beta_0+\beta_1B_i+\beta_2W_i+\beta_3R_i+
\beta_4B_iW_i+\beta_5B_iR_i,
$$

where $B_i$ is beer intake and $W_i,R_i$ indicate Weird and Relaxed expressions. This uses the [logit link](../../../../../logit.md). Independence of the individual throws conditional on the day's predictors gives the binomial sampling model; extra within-day dependence would instead produce overdispersion. The interactions let the beer slope depend on facial expression, rather than requiring one common slope. With the data frame named darts, R code is

```
darts$Expression <- relevel(factor(darts$Expression), ref = "Mad")
barney <- glm(cbind(BullsEye, 100 - BullsEye) ~ Beer * Expression, family = binomial, data = darts)
```

Mad is the baseline category. Its intercept and beer slope are already represented by the first two coefficients; including all three category indicators together with an intercept would make the design matrix rank deficient. For three beers and Weird expression,

$$
\boxed{\eta=-0.37258-3(0.09055)-0.10005+3(0.03666)=-0.63430.}
$$

The fitted probability is $(1+e^{0.63430})^{-1}$, approximately 0.347.

The Weird intercept and interaction are individually nonsignificant, suggesting that Mad and Weird might be combined. The Relaxed beer interaction is significant, so dropping all interactions would discard supported structure. A candidate reduced model retains only the Relaxed indicator and its interaction:

```
reduced <- glm(cbind(BullsEye, 100 - BullsEye) ~ Beer * I(Expression == "Relaxed"), family = binomial, data = darts)
anova(reduced, barney, test = "Chisq")
```

This fits without changing the data file. The joint [likelihood-ratio test](../../../../../likelihood-ratio-test.md), rather than the two separate coefficient [p-values](../../../../../p-value.md) alone, decides whether the simplification is supported. Also inspect [regression residuals](../../../../../regression-residual.md) and the ratio of residual deviance to residual degrees of freedom for overdispersion or lack of fit; a quasibinomial analysis may be appropriate if the binomial [variance](../../../../../variance-split.md) is inadequate.

## ↑ Ancestors (10)

1. [13J](../13j.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
