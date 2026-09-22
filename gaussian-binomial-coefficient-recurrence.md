# Gaussian binomial coefficient recurrence

↑ **Parent:** [Gaussian binomial coefficient](gaussian-binomial-coefficient.md)

For $n\geq1$ and $1\leq k\leq n$, the displayed [recurrence relation](recurrence-relation.md) uses $G_{n,0}(t)=1$ and $G_{n,k}(t)=0$ when $k<0$ or $k>n$. At $t=1$ it becomes [Pascal's identity](pascal-s-rule.md).

An exact weighted-[subset](subset.md) formula is

$$
G_{n,k}(t)=\sum_{0\leq j_1<\cdots<j_k<n}t^{\sum_{i=1}^k(j_i-(i-1))}.
$$

The [exponent](exponent.md) measures how far the selected positions lie beyond the earliest possible choices $0,\ldots,k-1$. Split the [subsets](subset.md) according to whether they contain $n-1$. Those without it give $G_{n-1,k}(t)$; deleting it from those with it removes exactly $n-k$ from their [exponent](exponent.md). This gives the displayed [recurrence relation](recurrence-relation.md), explaining why it builds [polynomials](polynomial-split.md) with nonnegative [integer](integer-split.md) [coefficients](coefficient.md).

## ↑ Ancestors (6)

1. [Gaussian binomial coefficient](gaussian-binomial-coefficient.md)
2. [Binomial coefficient](binomial-coefficient-split.md)
3. [Combinatorics](combinatorics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Gaussian binomial coefficient](gaussian-binomial-coefficient.md)
- [Lattice-path interpretation of Gaussian binomial coefficients](lattice-path-interpretation-of-gaussian-binomial-coefficients.md)
