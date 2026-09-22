<h1 id="4f/solution">Solution</h1>

↑ **Parent:** [4F](../4f.md)

The [moment-generating function](../../../../../moment-generating-function.md) of a [random variable](../../../../../random-variable-split.md) $X$ is $M_X(t)=\mathbb E(e^{tX})$, defined for real $t$ where that expectation is finite. For a [standard normal distribution](../../../../../standard-normal-distribution.md), completing the square gives

$$
M_X(t)=\frac1{\sqrt{2\pi}}\int_{-\infty}^{\infty}e^{tx-x^2/2}\,dx
=e^{t^2/2}\frac1{\sqrt{2\pi}}\int_{-\infty}^{\infty}e^{-(x-t)^2/2}\,dx
=\boxed{e^{t^2/2}}.
$$

It is finite for every real $t$. Derivatives at zero give the [moments](../../../../../moment.md): the expansion $e^{t^2/2}=1+t^2/2+t^4/8+O(t^6)$ therefore gives

$$
\boxed{\mathbb EX^0=1,\quad \mathbb EX=0,\quad \mathbb EX^2=1,
\quad \mathbb EX^3=0,\quad \mathbb EX^4=3.}
$$

For $Y$ with the [normal distribution](../../../../../normal-distribution.md) of mean $\mu$ and variance $\sigma^2$, write $Y=\mu+\sigma X$ in distribution. Its [moment-generating function](../../../../../moment-generating-function.md) is consequently

$$
\boxed{M_Y(t)=e^{\mu t}M_X(\sigma t)
=\exp(\mu t+\sigma^2t^2/2).}
$$

This formula also covers the constant random variable when $\sigma=0$.

## ↑ Ancestors (10)

1. [4F](../4f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
