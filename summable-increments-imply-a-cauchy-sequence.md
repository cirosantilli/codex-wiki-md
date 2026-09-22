# Summable increments imply a Cauchy sequence

↑ **Parent:** [Cauchy sequence](cauchy-sequence.md)

If a [sequence](sequence.md) in a [metric space](metric-space.md) has $\sum_{j=1}^\infty d(x_{j+1},x_j)<\infty$, the [triangle inequality](triangle-inequality.md) gives $d(x_m,x_n)\leq\sum_{j=n}^{m-1}d(x_{j+1},x_j)$ for $m>n$. The tail of this [convergent series](convergent-series.md) tends to zero and bounds every later pair, proving the [Cauchy sequence](cauchy-sequence.md) condition. In particular, an increment bound $d(x_{j+1},x_j)\leq C r^j$ with $C>0$ and $0<r<1$ gives $d(x_m,x_n)\leq C r^n/(1-r)$ by the [geometric series](geometric-series.md). Unlike checking a small latest step, this bounds all remaining movement.

This sufficient condition is not necessary. The real [sequence](sequence.md) $x_n=(-1)^n/n$ converges to zero and is therefore a [Cauchy sequence](cauchy-sequence.md), although $|x_{n+1}-x_n|=1/(n+1)+1/n$ has a divergent sum. Cancellation allows convergence despite infinite accumulated [absolute values](absolute-value.md) of the successive changes.

## ↑ Ancestors (7)

1. [Cauchy sequence](cauchy-sequence.md)
2. [Sequence and series](sequence-and-series-split.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
