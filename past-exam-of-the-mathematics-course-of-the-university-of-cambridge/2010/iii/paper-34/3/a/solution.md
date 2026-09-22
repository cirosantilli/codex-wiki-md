<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume independent individuals and [independent censoring](../../../../../../independent-censoring.md), with the censoring law not involving the event-rate parameters. If $T_j$ is the [survival time](../../../../../../survival-time.md) and $C_j$ its censoring time, we observe $x_j=\min(T_j,C_j)$ and $v_j=\mathbf1_{\{T_j\leq C_j\}}$. The [exponential distribution](../../../../../../exponential-distribution.md) gives

$$
f_j(x)=\theta_j e^{-\theta_jx},\qquad S_j(x)=e^{-\theta_jx}.
$$

An observed event contributes $f_j(x_j)$, while a [right-censored](../../../../../../right-censoring.md) observation contributes $S_j(x_j)$, because it only says the event has not occurred by $x_j$. Multiplying these [survival likelihood](../../../../../../survival-likelihood.md) contributions and omitting censoring factors independent of the parameters gives

$$
L(\theta_1,\ldots,\theta_n)\propto\prod_{j=1}^n\theta_j^{v_j}e^{-\theta_jx_j},
\qquad
\boxed{\ell(\theta)=\sum_{j=1}^n\{v_j\log\theta_j-\theta_jx_j\}+\text{constant}.}
$$

Without [independent censoring](../../../../../../independent-censoring.md) the censoring factors cannot generally be discarded in this way.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
