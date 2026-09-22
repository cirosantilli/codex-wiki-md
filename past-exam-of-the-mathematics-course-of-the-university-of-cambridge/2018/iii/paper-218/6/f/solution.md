<h1 id="6/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

One suitable criterion among the three unpenalized [normal linear models](../../../../../../normal-linear-model.md) is the [Akaike information criterion](../../../../../../akaike-information-criterion.md). With $d$ estimated mean coefficients and the variance also estimated, minimizing AIC is equivalent to minimizing

$$
\boxed{\operatorname{AIC}=n\log(RSS/n)+2(d+1)+\text{a common constant}.}
$$

The values of $d$ are $2,2,3$ for model1, model2 and model3. This compares fit and complexity rather than choosing solely by individual coefficient significance. The [Bayesian information criterion](../../../../../../bayesian-information-criterion.md) or a common-fold predictive comparison would also be reasonable, depending on the selection objective.

For the [ridge regression](../../../../../../ridge-regression.md) tuning parameter, use [K-fold cross-validation](../../../../../../k-fold-cross-validation.md) with squared prediction loss:

$$
\boxed{CV(\lambda)=\frac1n\sum_{k=1}^K\sum_{i\in I_k}\{y_i-\widehat f_{-I_k,\lambda}(x_i)\}^2.}
$$

Use the same folds for every candidate, estimate any centering or scaling within each training fold, choose a minimizing $\lambda$, and refit on all observations. This estimates [mean squared prediction error](../../../../../../mean-squared-prediction-error.md) while avoiding [data leakage](../../../../../../data-leakage.md). The printed summaries do not supply all residual sums of squares or validation losses, so they do not determine which model or penalty wins.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [6](../../6.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
