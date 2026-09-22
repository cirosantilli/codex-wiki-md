<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\phi_\rho$ denote the centered unit-variance [bivariate normal distribution](../../../../../../bivariate-normal-distribution.md) density,

$$
\phi_\rho(x,y)=\frac1{2\pi\sqrt{1-\rho^2}}\exp\left(-\frac{x^2-2\rho xy+y^2}{2(1-\rho^2)}\right).
$$

The complement of rejecting either [null hypothesis](../../../../../../null-hypothesis.md) is $W_1\le c,W_2\le c$. Therefore **the probability of at least one rejection** is

$$
\boxed{1-\int_{-\infty}^{c-m_1}\int_{-\infty}^{c-m_2}\phi_\rho(x,y)\,dy\,dx.}
$$

When both [null hypotheses](../../../../../../null-hypothesis.md) are true, this is the [familywise error rate](../../../../../../familywise-error-rate.md). If one [null hypothesis](../../../../../../null-hypothesis.md) is false, a rejection of that hypothesis is not a [Type I error](../../../../../../type-i-and-type-ii-errors.md), so the displayed probability is then an any-rejection probability rather than the [familywise error rate](../../../../../../familywise-error-rate.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
