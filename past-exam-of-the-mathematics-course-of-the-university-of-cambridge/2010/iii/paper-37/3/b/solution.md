<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Independence gives the [log-likelihood](../../../../../../log-likelihood.md)

$$
\ell(\beta)=\sum_i\left[y_i\beta^Tx_i-\log(1+e^{\beta^Tx_i})\right].
$$

Differentiating yields the [score equations](../../../../../../score-equation.md)

$$
\boxed{\sum_i x_i\bigl[y_i-p_i(\hat\beta)\bigr]=0.}
$$

When a finite [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md) exists, multiplying these equations by $\hat\beta^T$ gives

$$
\sum_i y_i\operatorname{logit}p_i(\hat\beta)=\sum_i p_i(\hat\beta)\operatorname{logit}p_i(\hat\beta).
$$

The qualification about a finite estimator matters under [complete separation](../../../../../../complete-separation.md) in [logistic regression](../../../../../../logistic-regression.md), where coefficient estimates can escape to infinity.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
