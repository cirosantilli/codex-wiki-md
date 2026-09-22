<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The coefficient labelled `yr2` identifies year as a factor. With $z_i=0$ in the first year and $z_i=1$ in the second, the [Poisson regression](../../../../../../poisson-regression.md) assumes independent daily counts conditional on year,

$$
Y_i\sim\operatorname{Pois}(\mu_i),\qquad
\log\mu_i=\beta_0+\beta_1z_i.
$$

The unknown mean [statistical parameters](../../../../../../statistical-parameter.md) are the first-year log daily rate $\beta_0$ and the second-year log rate ratio $\beta_1$; the [dispersion parameter](../../../../../../dispersion-parameter.md) is fixed at one. Approximate 95% [Wald confidence intervals](../../../../../../wald-confidence-interval.md) are

$$
\begin{aligned}
\widehat\beta_0&=1.78810,&\quad \beta_0&\in1.78810\pm1.96(0.02141)=(1.74614,1.83006),\\
\widehat\beta_1&=-0.09816,&\quad \beta_1&\in-0.09816\pm1.96(0.03105)=(-0.15902,-0.03730).
\end{aligned}
$$

Exponentiating yields the first-year fitted daily mean $5.978$, with [confidence interval](../../../../../../confidence-interval.md) $(5.732,6.234)$, and

$$
\boxed{\frac{\widehat\mu_2}{\widehat\mu_1}=0.9065,\qquad
\frac{\mu_2}{\mu_1}\in(0.8530,0.9634).}
$$

The second-year fitted daily mean is $e^{1.78810-0.09816}=5.419$. Thus this [Poisson regression](../../../../../../poisson-regression.md) estimates a 9.35% fall, with an approximate interval for the percentage fall from 3.66% to 14.70%. These [confidence intervals](../../../../../../confidence-interval.md) rely on the [Poisson distribution](../../../../../../poisson-distribution.md) and independence assumptions.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
