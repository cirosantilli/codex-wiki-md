<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the given [exchangeable](../../../../../../exchangeable-random-variables.md) law $\mu$, put

$$
m_k=\mu(\eta\equiv1\text{ on }A)\quad\text{when }|A|=k,
$$

which is well-defined by the stated assumption. Integrate the [product self-duality of symmetric exclusion](../../../../../../product-self-duality-of-symmetric-exclusion.md) against $\mu$, and use boundedness to interchange [expectation](../../../../../../expected-value.md) and integration:

$$
\int\mathbb P^\eta(\eta_t\equiv1\text{ on }A)\,\mu(d\eta)
=\mathbb E^A\left[\mu(\eta\equiv1\text{ on }A_t)\right].
$$

The finite-particle process conserves its cardinality. Hence the right side is $\mathbb E^A m_{|A_t|}=m_{|A|}$. All occupation-product moments are therefore unchanged by evolution.

These moments determine the law, not merely its one-site marginals. For disjoint [finite sets](../../../../../../finite-set.md) $B,C$, the [inclusion-exclusion principle](../../../../../../inclusion-exclusion-principle.md) gives

$$
\mu(\eta\equiv1\text{ on }B,\ \eta\equiv0\text{ on }C)
=\sum_{D\subseteq C}(-1)^{|D|}\mu(\eta\equiv1\text{ on }B\cup D).
$$

Every term is unchanged, so every finite cylinder [probability](../../../../../../probability.md) is unchanged. Such cylinder events generate the [product sigma-algebra](../../../../../../product-sigma-algebra.md) on $\{0,1\}^{\mathbb Z}$, and [probability](../../../../../../probability.md) laws agreeing on them agree everywhere. Consequently

$$
\boxed{\mu P_t=\mu\quad(t\ge0).}
$$

Thus every [exchangeable](../../../../../../exchangeable-random-variables.md) [probability](../../../../../../probability.md) law is invariant for the [symmetric exclusion process](../../../../../../symmetric-simple-exclusion-process.md). This proof of [exchangeable invariant laws of symmetric exclusion](../../../../../../exchangeable-invariant-laws-of-symmetric-exclusion.md) needs only the given cardinality dependence and duality; no representation theorem for [exchangeable](../../../../../../exchangeable-random-variables.md) measures is required.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
