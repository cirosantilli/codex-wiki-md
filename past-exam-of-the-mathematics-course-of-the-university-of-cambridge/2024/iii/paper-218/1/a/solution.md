<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $Y_i$ for the colony count and $d_i$ for the dose on plate $i$. The first fit is the [Poisson regression](../../../../../../poisson-regression.md)

$$
Y_i\mathrel{\perp\!\!\!\perp}Y_j\quad(i\ne j),
\qquad
Y_i\sim\operatorname{Pois}(\mu_i),
\qquad
\log\mu_i=\beta_0+\beta_1d_i.
$$

Thus its [log-likelihood](../../../../../../log-likelihood.md) is

$$
\ell(\beta_0,\beta_1)
=\sum_{i=1}^{18}\left[y_i(\beta_0+\beta_1d_i)
-e^{\beta_0+\beta_1d_i}-\log(y_i!)\right].
$$

The [Poisson deviance](../../../../../../poisson-deviance.md) relative to the saturated model is

$$
D=2\sum_{i=1}^{18}
\left\{y_i\log\frac{y_i}{\widehat\mu_i}
-(y_i-\widehat\mu_i)\right\},
$$

where a summand with $y_i=0$ uses $0\log0=0$.

At dose zero the fitted [expected value](../../../../../../expected-value.md) is $e^{\widehat\beta_0}=e^{3.321995}\simeq27.72$ eradicated colonies. Increasing dose by one unit multiplies the fitted mean by $e^{\widehat\beta_1}=e^{0.0001901}\simeq1.000190$; for example, an increase of $100$ units multiplies it by about $1.0192$. The positive fitted effect is small and its displayed two-sided $p$-value, $0.105$, gives little evidence against a zero dose coefficient.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
