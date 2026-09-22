<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use positive strikes, the natural real-power domain of this price curve. For any such $K$, the stock-minus-call payoff is

$$
S_1-(S_1-K)^+=\min(S_1,K)>0
$$

almost surely, since $S_1>0$. Therefore the call price must be strictly below the [stock](../../../../../../stock.md) price $S_0=1$: if $C(K)\geq1$, buying [stock](../../../../../../stock.md) and selling the call has nonpositive initial cost and strictly positive terminal payoff. Also a negative call price is an immediate [arbitrage](../../../../../../arbitrage.md) by buying the call.

For $p<0$, $1+K^p>K^p$ and raising to the negative power $1/p$ reverses the inequality, giving $(1+K^p)^{1/p}<K$ and $C(K)<0$. The expression is undefined at $p=0$. For $0<p<1$, strict [concavity](../../../../../../concave-function.md) of the power implies $(1+K)^p<1+K^p$, whence

$$
C(K)=(1+K^p)^{1/p}-K>1.
$$

At $p=1$, $C(K)=1$. Every defined case with $p\leq1$ therefore violates the necessary no-arbitrage bounds. Consequently

$$
\boxed{p>1.}
$$

This argument does not require a dense family of strikes; even one positive-strike call gives the contradiction. The strict stock-minus-call payoff explains why the borderline $p=1$ is also excluded.

## ↑ Ancestors (11)

1. [C](../c.md)
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
