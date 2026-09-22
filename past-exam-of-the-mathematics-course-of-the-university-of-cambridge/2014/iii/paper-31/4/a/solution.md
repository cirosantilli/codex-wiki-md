<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [gamma distribution](../../../../../../gamma-distribution.md) shape-rate convention: $\Theta\sim\operatorname{Gamma}(\alpha,\beta)$ with $\alpha,\beta>0$. The conditional [Poisson distribution](../../../../../../poisson-distribution.md) has mean and variance both equal to $\Theta$, so the [Bühlmann–Straub model](../../../../../../buhlmann-straub-model.md) parameters are

$$
\boxed{m_0=v=\frac{\alpha}{\beta},\qquad
a=\frac{\alpha}{\beta^2},\qquad \frac va=\beta.}
$$

For $W=\sum_jm_j$ and $y=\sum_jy_j$, the [Bühlmann–Straub credibility factor](../../../../../../buhlmann-straub-credibility-factor.md) is $Z=W/(W+\beta)$. Thus

$$
\widehat\mu=\frac{W}{W+\beta}\frac{y}{W}
+\frac{\beta}{W+\beta}\frac{\alpha}{\beta}
=\frac{y+\alpha}{W+\beta},
$$

and the required expected-count estimate is

$$
\boxed{\widehat{\mathbb E[Y_{n+1}\mid\Theta]}
=m_{n+1}\frac{\alpha+\sum_{j=1}^n y_j}{\beta+\sum_{j=1}^n m_j}.}
$$

The total exposure determines how much information the observed count carries; the number of years alone is not the appropriate denominator.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
