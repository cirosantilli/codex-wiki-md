<h1 id="7/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A [right-censored](../../../../../../right-censoring.md) subject contributes survival up to the recorded censoring time, not no information. Under [independent censoring](../../../../../../independent-censoring.md), write $x_i=\min(T_i,C_i)$ and $v_i=\mathbf1_{\{T_i\leq C_i\}}$. For exponential death rate $\lambda$, the event-model [survival likelihood](../../../../../../survival-likelihood.md) is

$$
\boxed{L(\lambda)\propto\lambda^{\sum_i v_i}
 e^{-\lambda\sum_i x_i},\qquad
\widehat\lambda_{\mathrm{full}}=\frac{\sum_i v_i}{\sum_i x_i}.}
$$

**Discarding censored subjects drops observed exposure and selects people whose death occurred before censoring.** Their recorded event times are not an unselected sample of all death times. The death-only conditional distribution can differ from the marginal death-time distribution even when censoring is independent. A correct [maximum-likelihood estimate](../../../../../../maximum-likelihood-estimator.md) uses the total observed person-time, including censored follow-up.

## ↑ Ancestors (11)

1. [6](../6.md)
2. [7](../../7.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
