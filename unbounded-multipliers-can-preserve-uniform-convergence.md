# Unbounded multipliers can preserve uniform convergence

↑ **Parent:** [Uniform convergence](uniform-convergence.md)

An unbounded [function](function-split.md) can multiply a [series](series-mathematics.md) while preserving [uniform convergence](uniform-convergence.md). On $E=(0,1/2]$, let $g(x)=1/x$. The [geometric series](geometric-series.md) gives

$$
\sum_{n=0}^{\infty}x^ng(x)=\frac1{x(1-x)},\qquad
\sup_{x\in E}\left|\frac1{x(1-x)}-\sum_{n=0}^Nx^{n-1}\right|=2^{1-N}\longrightarrow0.
$$

The equality follows because $x^N/(1-x)$ increases up to $x=1/2$. Both the first term and the sum are unbounded, while their difference after sufficiently many terms is uniformly small. [Uniform convergence](uniform-convergence.md) controls approximation errors; boundedness of each individual [function](function-split.md) is a separate property.

## ↑ Ancestors (7)

1. [Uniform convergence](uniform-convergence.md)
2. [Sequence and series](sequence-and-series-split.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
