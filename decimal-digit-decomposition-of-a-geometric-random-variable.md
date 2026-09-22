# Decimal digit decomposition of a geometric random variable

↑ **Parent:** [Geometric distribution](geometric-distribution.md)

The same argument works for any integer base $b\ge2$. Suppose $N$ has [geometric distribution](geometric-distribution.md) $\mathbb P(N=n)=(1-q)q^n$, $n\ge0$, with $0<q<1$. Its [Euclidean division](euclidean-division.md) $N=bY+X$ gives $0\le X<b$ and $Y\ge0$. Their [joint probability mass function](joint-probability-mass-function.md) is

$$
p_{X,Y}(x,y)=(1-q)q^{x+by}
=\frac{(1-q)q^x}{1-q^b}(1-q^b)q^{by}.
$$

The factors are normalized [probability mass functions](probability-mass-function.md), so the final digit $X$ and quotient $Y$ are [independent](independent-random-variables.md). The quotient again has [geometric distribution](geometric-distribution.md), with success [probability](probability.md) $1-q^b$. If $N$ is the integer part of an [exponential random variable](exponential-distribution.md) of rate $\lambda$, take $q=e^{-\lambda}$.

## ↑ Ancestors (8)

1. [Geometric distribution](geometric-distribution.md)
2. [Discrete probability distribution](discrete-probability-distribution-split.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/undated/prelims/mathematics-iii-resit/4/c/i/solution.md)
