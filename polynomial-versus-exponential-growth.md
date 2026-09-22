# Polynomial versus exponential growth

↑ **Parent:** [Big O notation](big-o-notation.md)

Every fixed power is eventually smaller than an [exponential function](exponential-function.md) with base $a>1$: for a fixed nonnegative integer $k$, $n^k/a^n\to0$. To prove this, the ratio of successive terms is $(1+1/n)^k/a\to1/a<1$, so after finitely many terms the ratio is bounded by a fixed $q<1$. A [geometric series](geometric-series.md) bound then proves the limit. In particular $n^k=O(a^n)$ in [big O notation](big-o-notation.md).

## ↑ Ancestors (6)

1. [Big O notation](big-o-notation.md)
2. [Real analysis](real-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/discrete-mathematics-continuous-mathematics-and-probability/discrete-mathematics/2/c/solution.md)
