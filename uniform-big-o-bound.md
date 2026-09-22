# Uniform big O bound

↑ **Parent:** [Big O notation](big-o-notation.md)

A uniform big O bound for a family of [functions](function-split.md) uses one multiplier and one threshold for every allowed parameter:

$$
\exists C>0,\ N\quad\forall\alpha\in A\quad\forall n\ge N:
\quad |f_\alpha(n)|\le C|g(n)|.
$$

The order of the quantifiers matters. For $f_\alpha(n)=\alpha n$, $0\le\alpha\le10$ admits $C=10$ and $N=1$, while the unbounded family $\alpha>0$ admits no such constant. Each individual member nevertheless satisfies $f_\alpha=O(n)$. A uniform bound is useful when an approximation must work across a whole parameter range, rather than separately for each fixed parameter.

## ↑ Ancestors (6)

1. [Big O notation](big-o-notation.md)
2. [Real analysis](real-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Big O notation](big-o-notation.md)
