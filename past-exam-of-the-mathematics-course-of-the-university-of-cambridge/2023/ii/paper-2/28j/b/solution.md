<h1 id="28j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $i\geq1$, the total holding rate is $(\lambda+1)2^i$, and the [jump chain](../../../../../../jump-chain.md) moves upward and downward with probabilities

$$
p=\frac{\lambda}{\lambda+1},
\qquad
q=\frac1{\lambda+1},
$$

while it moves from zero to one with probability one. Thus it is a [reflected nearest-neighbour random walk](../../../../../../reflected-nearest-neighbour-random-walk.md). Recurrence is unaffected by the holding times, so it is recurrent exactly when $p\leq q$. In the given range,

$$
\boxed{X\text{ is recurrent exactly when }\lambda=1.}
$$

For $\lambda>1$ the jump chain is transient.

The [detailed-balance equations](../../../../../../detailed-balance-for-a-birth-death-process.md) are

$$
\pi_i\lambda2^i=\pi_{i+1}2^{i+1}
\qquad(i\geq0),
$$

where the formula also covers the boundary $i=0$. Hence every candidate invariant measure has

$$
\pi_i=\pi_0\left(\frac\lambda2\right)^i.
$$

At $\lambda=1$ this is summable and the chain is nonexplosive, giving

$$
\pi_i=2^{-i-1},
\qquad i\geq0.
$$

For $\lambda=2$ it is not summable. When $1<\lambda<2$, it is a summable formal solution of $\pi Q=0$, but the chain explodes, so it is not an invariant probability for the minimal process; this is precisely the caveat in [invariant distribution of an explosive chain](../../../../../../invariant-distribution-of-an-explosive-chain.md). Consequently

$$
\boxed{X\text{ has an invariant distribution exactly when }\lambda=1.}
$$

It remains to classify explosion. At $\lambda=1$, the recurrent jump chain visits zero infinitely often. The holding time at zero has rate one, so [nonexplosion from recurrent visits to a slow state](../../../../../../nonexplosion-from-recurrent-visits-to-a-slow-state.md) shows that the accumulated time is infinite almost surely.

For $\lambda>1$, let $V_i$ be the total number of visits of the transient jump chain to $i$. Using the stated uniform visit bound and writing $q_i=(\lambda+1)2^i$ for $i\geq1$,

$$
\mathbb E\!\left[\sum_{n\geq0}\frac1{q_{Y_n}}\right]
=\sum_{i\geq0}\frac{\mathbb E V_i}{q_i}
<\infty,
$$

because $\sum_i2^{-i}<\infty$. Conditional on the jump path, this is the expected sum of all holding times, so the total lifetime is finite almost surely. This is [explosion of an upward-biased walk with geometrically increasing rates](../../../../../../explosion-of-an-upward-biased-walk-with-geometrically-increasing-rates.md). Therefore

$$
\boxed{X\text{ is explosive exactly when }1<\lambda\leq2.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [28J](../../28j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
