<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Order configurations coordinatewise. The [FKG lattice condition](../../../../../fkg-lattice-condition.md) on the masses of a finite Boolean lattice is

$$
P(\omega\wedge\eta)P(\omega\vee\eta)\geq P(\omega)P(\eta)\quad\text{for every }\omega,\eta.
$$

The [FKG inequality](../../../../../fkg-inequality.md) states that under this condition, increasing real-valued functions $f,g$ satisfy $\mathbb E[fg]\geq\mathbb E[f]\mathbb E[g]$. In particular [increasing events](../../../../../increasing-event.md) satisfy $P(A\cap B)\geq P(A)P(B)$. For a [product measure](../../../../../product-measure.md) with coordinate weights $w_e(0),w_e(1)$, the pair $(\min(\omega_e,\eta_e),\max(\omega_e,\eta_e))$ has the same two entries as $(\omega_e,\eta_e)$. Multiplying over coordinates gives equality in the lattice condition, including degenerate Bernoulli parameters without division by zero.

For independent [bond percolation](../../../../../bond-percolation-split.md) on the nearest-neighbor [cubic lattice](../../../../../cubic-lattice.md), write $\theta_d(p)=\mathbb P_p(|C(0)|=\infty)$. Define the [percolation critical probability](../../../../../percolation-critical-probability.md) and the [connective constant](../../../../../connective-constant.md) by

$$
\boxed{p_c(d)=\inf\{p\in[0,1]:\theta_d(p)>0\},\qquad\mu(d)=\lim_{n\to\infty}c_n(d)^{1/n}},
$$

where $c_n(d)$ counts rooted $n$-step [self-avoiding walks](../../../../../self-avoiding-walk.md). [Translation invariance](../../../../../translation-invariance.md) makes the root irrelevant, and part (i) proves existence of the latter limit.

First work on the [square lattice](../../../../../square-lattice.md), whose dual is another translated [square lattice](../../../../../square-lattice.md). Put $q=1-p$ and assume $q\mu(2)<1$. If the open cluster at the origin is finite, its exterior [edge](../../../../../edge-of-a-graph.md) boundary contains a closed dual simple circuit surrounding the origin. To see this planar fact, surround its finitely many vertices by their unit square cells and follow the exterior boundary: its crossing primal [edges](../../../../../edge-of-a-graph.md) are closed. Resolving repeated boundary vertices into simple circuits leaves a circuit separating the origin from infinity.

Let $a_n$ count such dual circuits of length $n$. Every one crosses the positive horizontal ray at distance at most $n$, because it surrounds the origin and its horizontal span is at most its length. Choosing a ray-crossing [edge](../../../../../edge-of-a-graph.md), an orientation and all but the last [edge](../../../../../edge-of-a-graph.md) encodes it by one of at most $Cn$ rooted length-$n-1$ [self-avoiding walks](../../../../../self-avoiding-walk.md). Thus $a_n\leq Cn c_{n-1}(2)$. Choose $b>\mu(2)$ with $qb<1$. The root-count limit gives $c_{n-1}(2)\leq C_b b^n$, so

$$
\mathbb P_p(\text{some enclosing closed dual circuit of length at least }N)
\leq CC_b\sum_{n\geq N}n(qb)^n\longrightarrow0.
$$

This summable tail alone need not make the probability of every enclosing circuit less than one. Choose a large $R$ and let $A_R$ be the absence of enclosing closed dual circuits of length at least $R$, with $P(A_R)>1/2$. Let $B_R$ require every primal [edge](../../../../../edge-of-a-graph.md) inside $[-R,R]^2$ to be open. It has positive probability. Both events are increasing. The finite-measure [Harris-FKG inequality](../../../../../harris-fkg-inequality.md) extends to $A_R$ by decreasing limits over finitely many circuit exclusions, so $P(A_R\cap B_R)\geq P(A_R)P(B_R)>0$.

On $B_R$ the origin is connected to every [graph vertex](../../../../../vertex-graph-theory.md) of that box. Any closed dual circuit enclosing the origin must then enclose the whole box, hence have length at least $R$. On $A_R\cap B_R$ no such circuit exists, so the origin cluster is infinite. This proves the [connective-constant Peierls bound](../../../../../connective-constant-peierls-bound.md), $p_c(2)\leq1-1/\mu(2)$. Finally the lattice in dimension $d\geq2$ contains a coordinate copy of the [square lattice](../../../../../square-lattice.md), whose [edge](../../../../../edge-of-a-graph.md) law is unchanged. Percolation in that subgraph implies percolation in the full [graph](../../../../../graph-split.md), and hence

$$
\boxed{p_c(d)\leq p_c(2)\leq1-\frac1{\mu(2)}}.
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 26](../../paper-26-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
