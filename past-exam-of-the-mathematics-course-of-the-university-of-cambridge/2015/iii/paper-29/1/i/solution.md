<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $z^- =\max(-z,0)$. For $a<b$, let $U_N[a,b]$ be the [upcrossing count](../../../../../../upcrossing-count.md) obtained by successively buying at an observation at or below $a$ and selling at an observation at or above $b$, with the first purchase allowed at time zero. The [Doob upcrossings lemma](../../../../../../doob-upcrossing-inequality.md) for an integrable discrete-time [martingale](../../../../../../martingale-split.md) is

$$
\boxed{(b-a)\mathbb E U_N[a,b]\leq\mathbb E(X_N-a)^--\mathbb E(X_0-a)^-\leq\mathbb E(X_N-a)^-.}
$$

The weaker last bound is also the usual [Doob upcrossing inequality](../../../../../../doob-upcrossing-inequality.md).

To prove it, hold one unit between each purchase and sale, and zero units otherwise. If $H_k$ records the holding over $(k,k+1]$, the decision is $\mathcal F_k$-[measurable](../../../../../../measurability.md), with $H_k\in\{0,1\}$. The resulting [martingale transform](../../../../../../martingale-transform.md) has gain

$$
G_N=\sum_{k=0}^{N-1}H_k(X_{k+1}-X_k),\qquad \mathbb E G_N=0.
$$

Each completed [upcrossing](../../../../../../upcrossing.md) earns at least $b-a$. An unfinished holding loses at most $(X_N-a)^-$. If a purchase occurs at zero, its price is $X_0\leq a$, giving the additional discount $(X_0-a)^-$, whether that holding has been sold or remains open. If no purchase occurs at zero, this extra term is zero. Therefore, path by path,

$$
G_N\geq(b-a)U_N[a,b]-(X_N-a)^-+(X_0-a)^-.
$$

Taking [expectations](../../../../../../expected-value.md) proves the bound.

The [martingale convergence theorem](../../../../../../martingale-convergence-theorem.md), stated without proof, says that a discrete-time [martingale](../../../../../../martingale-split.md) satisfying $\sup_n\mathbb E|X_n|<\infty$ converges [almost surely](../../../../../../almost-sure-convergence.md) to a finite [integrable random variable](../../../../../../integrable-random-variable.md) $X_\infty$. In particular every nonnegative [martingale](../../../../../../martingale-split.md) converges [almost surely](../../../../../../almost-sure-convergence.md) to a finite limit. Under [uniform integrability](../../../../../../uniform-integrability.md), the [uniformly integrable martingale convergence theorem](../../../../../../uniformly-integrable-martingale-convergence-theorem.md) additionally gives [convergence in L1](../../../../../../convergence-in-l1.md) and $X_n=\mathbb E[X_\infty\mid\mathcal F_n]$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
