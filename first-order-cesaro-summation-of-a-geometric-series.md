<h1 id="first-order-cesaro-summation-of-a-geometric-series">First-order Cesàro summation of a geometric series</h1>

↑ **Parent:** [Cesàro summation](cesaro-summation.md)

For the [geometric series](geometric-series.md) with terms $z^n$, $z\neq1$, the [partial sums](partial-sum.md) are $(1-z^{n+1})/(1-z)$. Averaging the finite expressions gives

$$
\sigma_N=\frac1{1-z}-\frac{z(1-z^{N+1})}{(N+1)(1-z)^2}.
$$

If $|z|\leq1$ and $z\neq1$, the second term has [absolute value](absolute-value.md) at most $2/((N+1)|1-z|^2)$, and therefore tends to zero. On the [unit circle](complex-unit-circle.md), except at $z=1$, this yields a first-order [Cesàro sum](cesaro-sum.md) even though the terms do not tend to zero. For $z=1$, instead $s_n=n+1$ and $\sigma_N=(N+2)/2$, so there is no finite [Cesàro sum](cesaro-sum.md).[Example 2, geometric-series calculation](cesaro-summation-mathematica-tutorial-by-vladimir-dobrushkin.md)

## ↑ Ancestors (9)

1. [Cesàro summation](cesaro-summation.md)
2. [Summation method](summation-method.md)
3. [Series (mathematics)](series-mathematics.md)
4. [Sequence and series](sequence-and-series-split.md)
5. [Real analysis](real-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)
