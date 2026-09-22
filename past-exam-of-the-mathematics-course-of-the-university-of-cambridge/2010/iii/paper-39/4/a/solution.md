<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

On a fixed horizon $T$, an [arbitrage](../../../../../../arbitrage.md) is an [admissible trading strategy](../../../../../../admissible-trading-strategy.md) that is [self-financing](../../../../../../self-financing-portfolio.md), has $X_0=0$, and satisfies $X_T\geq0$ almost surely with $\mathbb P(X_T>0)>0$. Here admissibility means that wealth in units of the strictly positive riskless [numéraire](../../../../../../numeraire.md) has a deterministic lower bound throughout the horizon. An [equivalent martingale measure](../../../../../../risk-neutral-measure.md) $Q$ is equivalent to the physical measure on $\mathcal F_T$ and makes each discounted risky price $\widetilde S^i=S^i/B$ a [martingale](../../../../../../martingale-split.md).

For a predictable, stochastically integrable risky holding vector $\pi$, the discounted self-financing identity is

$$
\widetilde X_t:=\frac{X_t}{B_t}
=\frac{X_0}{B_0}+\int_0^t\pi_s\cdot d\widetilde S_s.
$$

Indeed, since the riskless account is a [finite-variation process](../../../../../../finite-variation-process.md), its quadratic covariations vanish, and the [Itô formula](../../../../../../ito-s-lemma.md) for $X/B$, combined with $X=\phi B+\pi\cdot S$ and $dX=\phi\,dB+\pi\cdot dS$, gives $d(X/B)=\pi\cdot d(S/B)$.

Use two standard facts from [stochastic calculus](../../../../../../stochastic-calculus-split.md): a stochastic integral against a continuous local martingale is a [local martingale](../../../../../../local-martingale.md), and a local martingale bounded below by a deterministic constant is a [supermartingale](../../../../../../supermartingale.md). The latter follows by adding the constant to make the process nonnegative, stopping at a localizing sequence, and applying the conditional [Fatou lemma](../../../../../../fatou-s-lemma.md). Thus admissible discounted wealth is a $Q$-supermartingale, and an arbitrage would satisfy

$$
0\leq\mathbb E_Q[\widetilde X_T]\leq\widetilde X_0=0.
$$

It follows that $X_T=0$ $Q$-almost surely, hence also physically almost surely by equivalence, a contradiction. Therefore **an equivalent martingale measure rules out arbitrage among admissible self-financing strategies**. The lower-bound restriction is essential to this argument; stochastic integrals need not be true martingales for arbitrary unbounded holdings.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
