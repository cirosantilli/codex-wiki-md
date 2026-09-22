<h1 id="11f/solution">Solution</h1>

↑ **Parent:** [11F](../11f.md)

Integrating the [uniform density](../../../../../continuous-uniform-distribution.md) gives $\mathbb EX^k=\int_0^1x^k\,dx=1/(k+1)$. By [independence of random variables](../../../../../independent-random-variables.md), $\mathbb E(XY)^k=\mathbb EX^k\,\mathbb EY^k=1/(k+1)^2$. For the remaining [expected value](../../../../../expected-value.md), integrate first in $x$:

$$
\begin{aligned}
\mathbb E(1-XY)^k
&=\int_0^1\int_0^1(1-xy)^k\,dx\,dy\\
&=\frac1{k+1}\int_0^1\frac{1-(1-y)^{k+1}}y\,dy
=\frac1{k+1}\sum_{j=0}^k\int_0^1(1-y)^j\,dy.
\end{aligned}
$$

The value at $y=0$ is supplied by continuity. Therefore, with the [harmonic number](../../../../../harmonic-number.md) $H_m=\sum_{j=1}^m1/j$,

$$
\boxed{\mathbb E(1-XY)^k=\frac{H_{k+1}}{k+1}.}
$$

Conditional on one sample point being $(x,y)$, it is a [maximal external point](../../../../../maximal-external-point.md) precisely when none of the other $n-1$ points falls in the upper-right rectangle $(x,1]\times(y,1]$. Its area is $(1-x)(1-y)$, so its conditional probability of being maximal is $[1-(1-x)(1-y)]^{n-1}$. Both $1-X$ and $1-Y$ are independent [uniform random variables](../../../../../uniform-random-variable.md), hence a given point is maximal with probability $H_n/n$. Summing their [indicator random variables](../../../../../indicator-random-variable.md) and applying [linearity of expectation](../../../../../linearity-of-expectation.md) gives the [expected number of coordinatewise maxima](../../../../../expected-number-of-coordinatewise-maxima.md):

$$
\boxed{\mathbb E[\text{number of maximal external points}]=H_n.}
$$

This grows only logarithmically with the sample size, even though all $n$ points are potential candidates.

## ↑ Ancestors (10)

1. [11F](../11f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
