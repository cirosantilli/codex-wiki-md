<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The required condition is [uniform integrability](../../../../../../uniform-integrability.md), written entirely in terms of the given [probability laws](../../../../../../probability-distribution.md):

$$
\boxed{\lim_{R\to\infty}\sup_n\int_{\{|x|>R\}}|x|\,\mu_n(dx)=0.}
$$

Together with the given [almost sure convergence](../../../../../../almost-sure-convergence.md), this implies [L1 convergence](../../../../../../convergence-in-l1.md) to an integrable $M_\infty$. Passing to the limit in $\mathbb E[M_m\mid\mathcal F_n]=M_n$, using the contraction property of [conditional expectation](../../../../../../conditional-expectation.md) in [L1 space](../../../../../../l1-space.md), gives $M_n=\mathbb E[M_\infty\mid\mathcal F_n]$.

For every bounded [stopping time](../../../../../../stopping-time.md) $S$, the same identity holds with $\mathcal F_S$: split an event of its [stopping-time sigma-algebra](../../../../../../stopping-time-sigma-algebra.md) according to $\{S=k\}$ and use the deterministic-time identity. In particular $M_{T\wedge n}=\mathbb E[M_\infty\mid\mathcal F_{T\wedge n}]$. These [conditional expectations](../../../../../../conditional-expectation.md) are [uniformly integrable](../../../../../../uniform-integrability.md): for an integrable $Y$ and $Z=\mathbb E[Y\mid\mathcal G]$, the event $A=\{|Z|>K\}$ satisfies $\mathbb P(A)\leq\mathbb E|Y|/K$, and

$$
\mathbb E[|Z|;A]\leq\mathbb E[|Y|;|Y|>R]+R\mathbb E|Y|/K.
$$

First choose $R$, then $K$, uniformly in $\mathcal G$. Define $M_T=M_\infty$ on $\{T=\infty\}$. Now $M_{T\wedge n}\to M_T$ [almost surely](../../../../../../almost-sure-convergence.md) and in [L1 space](../../../../../../l1-space.md), so the bounded-time mean identities imply **$\mathbb E M_T=\mathbb E M_0$ even when $T$ can be infinite**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
