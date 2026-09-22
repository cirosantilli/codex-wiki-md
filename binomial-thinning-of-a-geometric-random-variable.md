# Binomial thinning of a geometric random variable

↑ **Parent:** [Binomial thinning](binomial-thinning.md)

Use the zero-based [geometric distribution](geometric-distribution.md), with $\mathbb P(N=k)=p(1-p)^k$ for $k\geq0$ and $0<p<1$. After [binomial thinning](binomial-thinning.md) with retention [probability](probability.md) $0\leq r\leq1$, the retained count is again zero-based [geometrically distributed](geometric-distribution.md), with the displayed success [probability](probability.md). Indeed, writing $q=1-p$, its [probability generating function](probability-generating-function.md) is

$$
G_Y(s)=\frac{p}{1-q(1-r+rs)}=\frac{p'}{1-(1-p')s}.
$$

For $r=0$ this includes the degenerate success parameter $p'=1$ and retained count zero.

## ↑ Ancestors (8)

1. [Binomial thinning](binomial-thinning.md)
2. [Random sum](random-sum.md)
3. [Random variable](random-variable-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/discrete-mathematics-continuous-mathematics-and-probability/8/b/ii/solution.md)
