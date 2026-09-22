# Polylogarithm series remainder bound

↑ **Parent:** [Polylogarithm](polylogarithm.md)

For $|z|<1$, $a\geq0$ and integer $N\geq0$, truncating the defining [polylogarithm](polylogarithm.md) [power series](power-series.md) after $N$ terms has remainder

$$
\left|\sum_{k>N}\frac{z^k}{k^a}\right|
\leq\sum_{k>N}\frac{|z|^k}{(N+1)^a}
=\frac{|z|^{N+1}}{(N+1)^a(1-|z|)}.
$$

The inequality uses monotonicity of $k^a$ and then the [geometric series](geometric-series.md). The bound applies to negative real $z$ as well as positive real $z$, and gives a rigorous absolute truncation tolerance independently of cancellation. It does not bound floating-point rounding error.

## ↑ Ancestors (6)

1. [Polylogarithm](polylogarithm.md)
2. [Complex analysis](complex-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-simulation-and-statistical-programming-course-of-the-university-of-oxford/2021/3/b/i/solution.md)
