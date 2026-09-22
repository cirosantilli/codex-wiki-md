# Capped geometric waiting time

↑ **Parent:** [Geometric distribution](geometric-distribution.md)

For a positive-integer [geometric distribution](geometric-distribution.md) $P(N=j)=pq^{j-1}$ with $q=1-p$, the capped time has masses $pq^{j-1}$ for $1\leq j<k$ and $q^{k-1}$ at $k$. The last mass includes all later arrivals, not only $N=k$. Its [probability generating function](probability-generating-function.md) and [expected value](expected-value.md) are

$$
G_X(s)=p\sum_{j=1}^{k-1}q^{j-1}s^j+q^{k-1}s^k,\qquad \mathbb E X=\frac{1-q^k}{p}.
$$

The expectation follows either by differentiating the [PGF](probability-generating-function.md) or summing the tail [probabilities](probability.md) up to $k$.

## ↑ Ancestors (8)

1. [Geometric distribution](geometric-distribution.md)
2. [Discrete probability distribution](discrete-probability-distribution-split.md)
3. [Probability distribution](probability-distribution.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-2/4f/solution.md)
