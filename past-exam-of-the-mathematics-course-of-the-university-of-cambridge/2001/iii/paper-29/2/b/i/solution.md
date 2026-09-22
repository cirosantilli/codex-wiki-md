<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume independent individuals and [independent censoring](../../../../../../../independent-censoring.md) conditional on their explanatory variables, with the [censoring](../../../../../../../censoring-statistics.md) mechanism carrying no parameter $\theta$. A failure contributes its failure-time [probability density function](../../../../../../../probability-density-function.md) $f_i(x_i;\theta)$, while a censored observation contributes the [survival function](../../../../../../../survival-function.md) $F_i(x_i;\theta)$ because its failure time exceeds $x_i$. Terms from the [censoring](../../../../../../../censoring-statistics.md) distribution then factor out of the survival-parameter [likelihood](../../../../../../../likelihood-function.md). Thus the [survival likelihood](../../../../../../../survival-likelihood.md) and its logarithm are

$$
L(\theta)\propto\prod_{i=1}^n f_i(x_i;\theta)^{v_i}F_i(x_i;\theta)^{1-v_i},
$$



$$
\boxed{\ell(\theta)=\sum_{i=1}^n\{v_i\log f_i(x_i;\theta)+(1-v_i)\log F_i(x_i;\theta)\}+\text{constant}.}
$$

The individual subscripts allow the same parameter vector to act through different [covariate](../../../../../../../covariate.md) values.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 29](../../../../paper-29-split.md)
5. [Iii](../../../../split.md)
6. [2001](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
