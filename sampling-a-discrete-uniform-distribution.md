# Sampling a discrete uniform distribution

↑ **Parent:** [Discrete uniform distribution](discrete-uniform-distribution.md)

Let the numerical [support of a probability distribution](support-of-a-probability-distribution.md) be $x_1<\cdots<x_n$. Its [cumulative distribution function](cumulative-distribution-function.md) counts how many values have been passed:

$$
F_X(t)=\mathbb P(X\leq t)=\frac{|\{x\in S:x\leq t\}|}{n}.
$$

It is zero below $x_1$, equals $j/n$ on $x_j\leq t<x_{j+1}$ for $1\leq j<n$, and is one at and above $x_n$. Every jump is $1/n$, even when the horizontal gaps differ.

For [inverse transform sampling](inverse-transform-sampling.md), take an ideal [continuous uniform distribution](continuous-uniform-distribution.md) for $U$ on $[0,1)$. Partition that [interval](interval-mathematics.md) into $n$ [intervals](interval-mathematics.md) of width $1/n$ and output

$$
X=x_j\quad\text{when}\quad\frac{j-1}{n}\leq U<\frac{j}{n},\qquad j=1,\ldots,n.
$$

Each [interval](interval-mathematics.md) has [probability](probability.md) $1/n$, proving the desired [discrete uniform distribution](discrete-uniform-distribution.md). Using the [floor function](floor-function.md), the index is $j=1+\lfloor nU\rfloor$; for consecutive [integer](integer-split.md) values the output is $X=a+\lfloor nU\rfloor$. With the usual [quantile function](quantile-function.md) convention $Q(u)=\inf\{t:F_X(t)\geq u\}$, one instead writes $Q(u)=x_{\lceil nu\rceil}$ for $0<u\leq1$, using the [ceiling function](ceiling-function.md). The endpoint conventions differ only at a finite [set](set-split.md) of points with [probability](probability.md) zero under the ideal [continuous uniform distribution](continuous-uniform-distribution.md).

For $S=\{1,2,4,8\}$, the four [intervals](interval-mathematics.md) $[0,1/4)$, $[1/4,1/2)$, $[1/2,3/4)$, and $[3/4,1)$ select $1,2,4,8$, respectively. Thus $U=3/10$ selects $2$, while $U=9/10$ selects $8$. The upper half of the [interval](interval-mathematics.md) selects values at least four, recovering [probability](probability.md) $1/2$. Equal widths refer to the sampling [probability](probability.md) coordinate, not to distances between output values. This is an exact mathematical construction assuming an ideal [continuous uniform distribution](continuous-uniform-distribution.md); a finite computer random-number source needs its own justification of equal output chances.

## ↑ Ancestors (8)

1. [Discrete uniform distribution](discrete-uniform-distribution.md)
2. [Discrete probability distribution](discrete-probability-distribution-split.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
