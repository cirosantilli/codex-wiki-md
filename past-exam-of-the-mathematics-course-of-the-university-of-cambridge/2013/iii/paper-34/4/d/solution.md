<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Model $m$ gives the sequential forecast $f_{mt}(y_t)=p_m(y_t\mid y_1,\ldots,y_{t-1})$. The probability chain rule yields

$$
p_m(y_1,\ldots,y_T)=\prod_{t=1}^Tf_{mt}(y_t).
$$

Application of [Bayes' theorem](../../../../../../bayes-theorem.md) makes the factors successive [posterior predictive distributions](../../../../../../posterior-predictive-distribution.md), and their product is the [Bayesian model evidence](../../../../../../bayesian-model-evidence.md). Under conditionally independent sampling it is

$$
\int\prod_{t=1}^Tp_m(y_t\mid\theta_m)\,
p_m(\theta_m)\,d\theta_m.
$$

Taking logarithms gives the [prequential log score identity](../../../../../../prequential-log-score-identity.md)

$$
T_m=\sum_t\log f_{mt}(y_t)=\log p_m(y_1,\ldots,y_T).
$$

Therefore the [Bayes factor](../../../../../../bayes-factor.md) is

$$
\boxed{B_{12}
=\frac{p_1(y_1,\ldots,y_T)}{p_2(y_1,\ldots,y_T)}
=e^{T_1-T_2}.}
$$

This solves the second half of part (d), which is missing from the TeX. Proper priors and finite positive evidences are needed; unrelated improper-prior normalizing constants do not cancel.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
