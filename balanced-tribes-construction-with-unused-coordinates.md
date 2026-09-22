# Balanced tribes construction with unused coordinates

↑ **Parent:** [Tribes function](tribes-function.md)

Choose $w\geq1$ maximal such that $wm\leq n$ for the displayed $m$, and take the OR of $m$ AND blocks of size $w$, ignoring unused coordinates. Its failure probability is $(1-2^{-w})^m$, between one quarter and three quarters. Active coordinates have [influence](influence-of-a-variable.md) $2^{1-w}(1-2^{-w})^{m-1}$ and unused ones have zero influence. Maximality gives $2^{1-w}<4(\log2)(w+1)/n$; for $n\geq2$, $w\leq\log_2n$, so every influence is below $8\log n/n$. The construction is therefore a [quite fair Boolean function](quite-fair-boolean-function.md) with small influences for every $n\geq2$. The logarithmic bound cannot hold at $n=1$, where every quite fair function has influence one.

## ↑ Ancestors (8)

1. [Tribes function](tribes-function.md)
2. [Boolean function](boolean-function.md)
3. [Boolean hypercube](boolean-hypercube.md)
4. [Analysis of Boolean functions](analysis-of-boolean-functions.md)
5. [Combinatorics](combinatorics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-7/5/i/solution.md)
