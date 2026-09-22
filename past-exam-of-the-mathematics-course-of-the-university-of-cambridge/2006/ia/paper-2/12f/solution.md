<h1 id="12f/solution">Solution</h1>

↑ **Parent:** [12F](../12f.md)

Normalization uses $\int_{-\infty}^{\infty}(1+x^2)^{-1}\,dx=\pi$, hence

$$
\boxed{\gamma=\frac1\pi.}
$$

Each variable therefore has the standard [Cauchy distribution](../../../../../cauchy-distribution.md). Let $S_n=X_1+\cdots+X_n$. We prove by induction that its [probability density function](../../../../../probability-density-function.md) is

$$
\boxed{f_{S_n}(x)=\frac n{\pi(n^2+x^2)}.}
$$

It holds for $n=1$. If it holds for $n=m$, [independence](../../../../../independent-random-variables.md) and [convolution of probability densities](../../../../../convolution-of-independent-random-variables.md) give

$$
f_{S_{m+1}}(x)=\frac m{\pi^2}\int_{-\infty}^{\infty}\frac{dy}{(1+y^2)[m^2+(x-y)^2]}.
$$

The supplied integral identity makes this $(m+1)/\{\pi[(m+1)^2+x^2]\}$, completing the induction. Thus addition increases the Cauchy scale to $n$.

For $\overline X_n=S_n/n$, the density transformation is $f_{\overline X_n}(x)=n f_{S_n}(nx)$, giving

$$
\boxed{f_{\overline X_n}(x)=\frac1{\pi(1+x^2)}\quad\text{for every }n\ge1.}
$$

The [Cauchy sample mean has an unchanged distribution](../../../../../cauchy-sample-mean-has-an-unchanged-distribution.md). In particular, for every $\delta>0$,

$$
\mathbb P(|\overline X_n|>\delta)=1-\frac2\pi\arctan\delta>0,
$$

independently of $n$, so the average does not converge in probability to zero.

There is no contradiction with the usual [weak law of large numbers](../../../../../weak-law-of-large-numbers.md), whose finite-first-moment hypothesis is absent: $\mathbb E|X_1|=(2/\pi)\int_0^\infty x/(1+x^2)\,dx=\infty$. The positive and negative parts of $X_1$ both have infinite expectations, so $\mathbb EX_1$ is undefined. Its symmetric principal value is zero, but a principal value is not an [expected value](../../../../../expected-value.md). The law therefore supplies no conclusion that these sample averages must approach zero.

## ↑ Ancestors (10)

1. [12F](../12f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
