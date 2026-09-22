# Randomly shifted lattice point process

↑ **Parent:** [Constant intensity does not imply independence](constant-intensity-does-not-imply-independence.md)

Let $U$ have the [uniform distribution](continuous-uniform-distribution.md) on $[0,1)$ and place a point at every $k+U$, $k\in\mathbb Z$. This is a [simple point process](simple-point-process.md), locally finite, and a [stationary point process](stationary-point-process.md): a [translation](translation-geometry.md) only changes the phase modulo one, preserving its [uniform distribution](continuous-uniform-distribution.md). For every [Borel set](borel-set.md) $A$, the [Tonelli theorem](tonelli-theorem.md) gives

$$
\mathbb E[\Pi(A)]=\sum_{k\in\mathbb Z}\int_0^1\mathbf1_A(k+u)\,du=|A|.
$$

Its consecutive points are exactly one unit apart, despite having the same [intensity measure](intensity-measure-of-a-point-process.md) as a unit-rate [Poisson point process](poisson-point-process.md). This is the one-dimensional translated-grid construction.[Section 2.1, Example 2.3, printed pp. 26-27: randomly translated grids have constant intensity](stochastic-geometry-lectures-given-at-the-c-i-m-e-summer-school-held-in-martina-franca-italy-september-13-18-2004/spatial-point-processes-and-their-applications.md)

Every half-open interval of length one contains exactly one point. For $A=[0,1/2)$ and $B=[1/2,1)$, $\Pi(A)+\Pi(B)=1$, each count has the [Bernoulli distribution](bernoulli-distribution.md) with parameter $1/2$, and

$$
\operatorname{Cov}(\Pi(A),\Pi(B))=0-\frac12\frac12=-\frac14.
$$

More generally, an interval of length $L=m+r$, with $m$ a [nonnegative integer](natural-number.md) and $0\le r<1$, contains $m$ or $m+1$ points with [probabilities](probability.md) $1-r$ and $r$. Its count [variance](variance-split.md) is $r(1-r)$, while a unit-rate [Poisson point process](poisson-point-process.md) has count [variance](variance-split.md) $L$.

## ↑ Ancestors (8)

1. [Constant intensity does not imply independence](constant-intensity-does-not-imply-independence.md)
2. [Intensity measure of a point process](intensity-measure-of-a-point-process.md)
3. [Point process](point-process.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Constant intensity does not imply independence](constant-intensity-does-not-imply-independence.md)
