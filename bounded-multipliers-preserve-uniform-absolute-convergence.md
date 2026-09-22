# Bounded multipliers preserve uniform absolute convergence

↑ **Parent:** [Uniform absolute convergence](uniform-absolute-convergence.md)

Suppose a [series](series-mathematics.md) of [functions](function-split.md) $\sum f_n$ has [uniform absolute convergence](uniform-absolute-convergence.md) on $E$ and $(g_n)$ is a [uniformly bounded family of functions](uniformly-bounded-family-of-functions.md) there, with common bound $M$. The [triangle inequality](triangle-inequality.md) gives

$$
\left|\sum_{n=p+1}^qf_n(x)g_n(x)\right|\leq M\sum_{n=p+1}^q|f_n(x)|.
$$

The right-hand side tends uniformly to zero as $q>p\to\infty$. The [Uniform Cauchy criterion](uniform-cauchy-criterion.md) proves [uniform convergence](uniform-convergence.md) of $\sum f_ng_n$. Applying the same estimate to $\sum|f_ng_n|$ proves [uniform absolute convergence](uniform-absolute-convergence.md) too.

The shared bound over both $n$ and $x$ matters: separate bounds for each $g_n$ can grow too fast. For example, the constant [functions](function-split.md) $f_n(x)=2^{-n}$ and $g_n(x)=2^n$ have a summable original [series](series-mathematics.md) but products identically one.

## ↑ Ancestors (8)

1. [Uniform absolute convergence](uniform-absolute-convergence.md)
2. [Absolute convergence](absolute-convergence.md)
3. [Sequence and series](sequence-and-series-split.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
