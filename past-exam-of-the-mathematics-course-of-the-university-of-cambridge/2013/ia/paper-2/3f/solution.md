<h1 id="3f/solution">Solution</h1>

↑ **Parent:** [3F](../3f.md)

Expand around the [expectation](../../../../../expected-value.md) $\mu$:

$$
G(a)=\mathbb E[(X-\mu)^2]+2(\mu-a)\mathbb E[X-\mu]+(\mu-a)^2
=\sigma^2+(\mu-a)^2.
$$

Thus [variance as the minimum mean squared error of a constant](../../../../../variance-as-the-minimum-mean-squared-error-of-a-constant.md) gives

$$
\boxed{G(a)\geq\sigma^2,\quad\text{with equality exactly at }a=\mu}.
$$

The finite [second moment](../../../../../second-moment.md) also guarantees the finite first absolute moment needed below.

For a [probability density function](../../../../../probability-density-function.md) $f$, splitting at $a$ gives

$$
H(a)=\int_{-\infty}^a(a-x)f(x)\,dx+
\int_a^\infty(x-a)f(x)\,dx.
$$

Let $F$ be the [cumulative distribution function](../../../../../cumulative-distribution-function.md). Since a density gives no mass at a singleton, differentiating under this integral yields $H'(a)=F(a)-(1-F(a))=2F(a)-1$. This [derivative](../../../../../derivative.md) is nondecreasing, so $H$ is [convex](../../../../../convex-function.md) and

$$
\boxed{H\text{ is minimized at every }a\text{ with }F(a)=\frac12}.
$$

This is the [median minimizes expected absolute loss](../../../../../median-minimizes-expected-absolute-loss.md) property. The minimizer need not be unique: a gap in the density can give an interval of [medians](../../../../../median.md), all with the same loss.

## ↑ Ancestors (10)

1. [3F](../3f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
