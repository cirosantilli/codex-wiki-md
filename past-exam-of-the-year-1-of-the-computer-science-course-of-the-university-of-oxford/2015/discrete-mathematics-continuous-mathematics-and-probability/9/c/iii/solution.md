<h1 id="9/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The source prints bare differentials $\mathrm d$ in both [integrals](../../../../../../integral-split.md); the integration variable is $t$, so we write them as $dt$.[Printed page 10, Question 9(c)(iii), both displayed differentials omit the variable](../../../../../../discrete-mathematics-continuous-mathematics-and-probability-examination-2015-by-university-of-oxford.md)

The [normalization of a probability distribution](../../../../../../normalization-of-a-probability-distribution.md) for $Y$ gives

$$
1=\int_0^\infty f_Y(t)\,dt
=\frac1{\sqrt\pi}\int_0^\infty t^{-1/2}e^{-t}\,dt.
$$

Therefore

$$
\boxed{\int_0^\infty t^{-1/2}e^{-t}\,dt=\sqrt\pi.}
$$

Next, the [standard normal distribution](../../../../../../standard-normal-distribution.md) has $\mathbb E[Z]=0$ and $\operatorname{var}(Z)=1$, so the second [moment](../../../../../../moment.md) is $\mathbb E[Z^2]=1$. Since $Y=Z^2/2$, [linearity of expectation](../../../../../../linearity-of-expectation.md) yields $\mathbb E[Y]=1/2$. Expressing this [expectation](../../../../../../expected-value-split.md) using the [probability density function](../../../../../../probability-density-function.md) gives

$$
\frac12=\int_0^\infty t f_Y(t)\,dt
=\frac1{\sqrt\pi}\int_0^\infty t^{1/2}e^{-t}\,dt.
$$

Consequently

$$
\boxed{\int_0^\infty t^{1/2}e^{-t}\,dt=\frac{\sqrt\pi}{2}.}
$$

These evaluate the [gamma function](../../../../../../gamma-function.md) at $1/2$ and $3/2$, respectively, directly from a transformed [normal random variable](../../../../../../gaussian-random-variable.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [9](../../../9.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
