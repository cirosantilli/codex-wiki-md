<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let the common [vertex](../../../../../vertex-graph-theory.md) degree be $r>0$. For each unordered [edge](../../../../../edge-of-a-graph.md) place an independent [Poisson process](../../../../../poisson-process.md) of rate $1/r$, and at a mark interchange the two endpoint occupations. If exactly one endpoint is occupied, this moves its particle across that [edge](../../../../../edge-of-a-graph.md) at rate $1/r$; if both or neither are occupied, the occupied set stays unchanged. Thus each particle proposes jumps at total rate one, uniformly among its neighbours, with occupied-target proposals suppressed. This is the stated [symmetric simple exclusion process](../../../../../symmetric-simple-exclusion-process.md). An edgeless [graph](../../../../../graph-split.md) has the identity dynamics and both conclusions below hold trivially.

In the [stirring representation of symmetric exclusion](../../../../../stirring-representation-of-symmetric-exclusion.md), put a distinct label at every [vertex](../../../../../vertex-graph-theory.md) and interchange labels at every [edge](../../../../../edge-of-a-graph.md) mark, even when the occupations agree. There are finitely many marks on every finite time interval. Their chronological composition is a random [permutation](../../../../../permutation.md) $\pi_t$ of the [vertex](../../../../../vertex-graph-theory.md) set, and simultaneously for every initial set,

$$
\eta_t^A=\pi_t(A).
$$

Each [edge](../../../../../edge-of-a-graph.md) swap is its own inverse. Reflecting the [edge](../../../../../edge-of-a-graph.md)-mark times in $[0,t]$ preserves their joint [Poisson process](../../../../../poisson-process.md) law and reverses the order of the swaps. Hence $\pi_t^{-1}$ and $\pi_t$ have the same distribution. Pathwise,

$$
\pi_t(A)\supseteq B\quad\Longleftrightarrow\quad\pi_t^{-1}(B)\subseteq A.
$$

Taking [probabilities](../../../../../probability.md) and then using the inverse-[permutation](../../../../../permutation.md) distribution proves the [product self-duality of symmetric exclusion](../../../../../product-self-duality-of-symmetric-exclusion.md) in set form:

$$
\boxed{\mathbb P(\eta_t^A\supseteq B)=\mathbb P(\eta_t^B\subseteq A)}.
$$

No assumption about disjointness or equal cardinality of $A$ and $B$ is required; impossible inclusions have [probability](../../../../../probability.md) zero on both sides.

For invariance, independently choose the initial occupied set $A$ under the [product measure](../../../../../product-measure.md) $\mu_\rho$. The occupations are independent identically distributed [Bernoulli distribution](../../../../../bernoulli-distribution.md) variables, so permuting their sites by any deterministic [permutation](../../../../../permutation.md) preserves their joint law. Conditional on the independent stirring [permutation](../../../../../permutation.md) $\pi_t$, the output therefore still has law $\mu_\rho$. Averaging proves the [Bernoulli invariant laws of finite symmetric exclusion](../../../../../bernoulli-invariant-laws-of-finite-symmetric-exclusion.md):

$$
\boxed{\mu_\rho P_t=\mu_\rho\qquad(0\le\rho\le1)}.
$$

There is also a direct check from the duality. For every $B\subseteq V$,

$$
\int\mathbb P(\eta_t^A\supseteq B)\,\mu_\rho(dA)
=\mathbb E\left[\mu_\rho\{A:A\supseteq\eta_t^B\}\right]
=\mathbb E\rho^{|\eta_t^B|}=\rho^{|B|},
$$

because the [exclusion process](../../../../../exclusion-process.md) conserves particle number. These are exactly the joint occupation moments of $\mu_\rho$; on a finite set they determine the law by the [inclusion-exclusion principle](../../../../../inclusion-exclusion-principle.md). The endpoint densities give the absorbing empty and fully occupied configurations, and the empty-set moment is one also at $\rho=0$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 28](../../paper-28-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
