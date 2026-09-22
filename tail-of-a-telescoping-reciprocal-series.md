# Tail of a telescoping reciprocal series

↑ **Parent:** [Telescoping series](telescoping-series.md)

For the [telescoping series](telescoping-series.md) $\sum_{n=1}^{\infty}1/[n(n+1)]=1$, the remainder after the first $N$ terms is exactly

$$
1-S_N=\sum_{n=N+1}^{\infty}\frac1{n(n+1)}=\frac1{N+1}.
$$

Thus $S_9=0.9$, $S_{99}=0.99$, and $S_{999}=0.999$. This supplies an exact stopping rule: to make the [absolute error](absolute-error.md) at most $10^{-3}$, **999 terms suffice**. Requiring strictly less than $10^{-3}$ instead needs at least 1000 terms.

The next term, $a_{N+1}=1/[(N+1)(N+2)]$, is smaller than the full remaining [sum](sum.md) by a factor of $N+2$. For example, after 99 terms the next term is $1/10100$, while the remainder is $1/100$. The [term test for divergence](term-test-for-divergence.md) concerns individual terms; a reliable numerical approximation needs a bound on the whole remaining [sum](sum.md).

## ↑ Ancestors (8)

1. [Telescoping series](telescoping-series.md)
2. [Series (mathematics)](series-mathematics.md)
3. [Sequence and series](sequence-and-series.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Partial sum](partial-sum.md)
