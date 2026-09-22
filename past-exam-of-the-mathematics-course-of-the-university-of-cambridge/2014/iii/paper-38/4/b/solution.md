<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Buy half a call at each neighboring strike and sell one call at the middle strike. Its cost is

$$
\frac12C(K_{i-1})+\frac12C(K_{i+1})-C(K_i)<0.
$$

For fixed terminal [stock](../../../../../../stock.md) price $s$, the function $K\mapsto(s-K)^+$ is [convex](../../../../../../convex-function.md). Since $K_i$ is the midpoint, the payoff

$$
\frac12(s-K_{i-1})^++\frac12(s-K_{i+1})^+-(s-K_i)^+
$$

is nonnegative for every $s$. More explicitly, it is zero outside $[K_{i-1},K_{i+1}]$, equals $(s-K_{i-1})/2$ on $[K_{i-1},K_i]$, and equals $(K_{i+1}-s)/2$ on $[K_i,K_{i+1}]$. The negative cost and nonnegative payoff produce an [arbitrage](../../../../../../arbitrage.md). This is the [butterfly-spread arbitrage for nonconvex call prices](../../../../../../butterfly-spread-arbitrage-for-nonconvex-call-prices.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
