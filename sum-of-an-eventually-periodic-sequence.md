# Sum of an eventually periodic sequence

↑ **Parent:** [Eventually periodic sequence](eventually-periodic-sequence.md)

Suppose a numerical [sequence](sequence.md) has period $T$ from index $N$, and let $C=\sum_{j=0}^{T-1}u_{N+j}$. For $L=qT+r$ with $0\leq r<T$, split the required [sum](sum.md) into $q$ complete periods and a tail of length $r$. Every complete period contributes $C$, proving the formula in the title. Precomputed [prefix sums](prefix-sum.md) of one period make the tail lookup constant time. If this periodic [sequence](sequence.md) consists of the [first differences](first-difference.md) of another [sequence](sequence.md), the same formula extrapolates that original [sequence](sequence.md) by adding the initial value at $N$.

## ↑ Ancestors (8)

1. [Eventually periodic sequence](eventually-periodic-sequence.md)
2. [Sequence](sequence.md)
3. [Sequence and series](sequence-and-series-split.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
