<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For [fair division](../../../../../fair-division.md), let $J=\{1,\ldots,m\}$ and let the [additive valuation](../../../../../additive-valuation.md) of agent $i$ be $v_i(S)=\sum_{j\in S}v_{ij}$. Use one variable $X_i$ per agent, with [constraint domain](../../../../../constraint-domain.md) $\mathcal P(J)$, the [power set](../../../../../power-set.md) of the items. Empty bundles are permitted in this original formulation.

Require pairwise [disjoint sets](../../../../../disjoint-sets.md):

$$
X_i\cap X_\ell=\varnothing\qquad(1\le i<\ell\le n).
$$

Each such [binary constraint](../../../../../binary-constraint.md) involves exactly $X_i,X_\ell$. Require complete allocation by the single all-variable constraint

$$
\bigcup_{i=1}^{n}X_i=J.
$$

Finally impose the [envy-free allocation](../../../../../envy-free-allocation.md) [binary constraints](../../../../../binary-constraint.md)

$$
v_i(X_i)\ge v_i(X_\ell)\qquad(i\ne\ell),
$$

each on $X_i,X_\ell$. The two directions for a pair use different agents' [additive valuations](../../../../../additive-valuation.md) and must both hold. These conditions give precisely an ordered [set partition](../../../../../set-partition.md) of the items that is an [envy-free allocation](../../../../../envy-free-allocation.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2023](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
