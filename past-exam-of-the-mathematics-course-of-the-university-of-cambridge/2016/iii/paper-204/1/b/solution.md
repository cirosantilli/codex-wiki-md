<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Order configurations coordinatewise: $\omega\leq\omega'$ means $\omega_e\leq\omega'_e$ for every [edge](../../../../../../edge-of-a-graph.md). An [increasing event](../../../../../../increasing-event.md) $A$ is a measurable [set](../../../../../../set-split.md) such that $\omega\in A$ and $\omega\leq\omega'$ imply $\omega'\in A$. Opening additional [edges](../../../../../../edge-of-a-graph.md) cannot destroy an [increasing event](../../../../../../increasing-event.md). The [Harris-FKG inequality](../../../../../../harris-fkg-inequality.md), the [product measure](../../../../../../product-measure.md) version of the [FKG inequality](../../../../../../fkg-inequality.md), states

$$
\boxed{\mathbb P_p(A\cap B)\geq\mathbb P_p(A)\mathbb P_p(B)}
$$

for two [increasing events](../../../../../../increasing-event.md). Equivalently, bounded coordinatewise increasing [random variables](../../../../../../random-variable-split.md) $f,g$ satisfy $\mathbb E_p(fg)\geq\mathbb E_p f\,\mathbb E_p g$. The event inequality also holds for two [decreasing events](../../../../../../decreasing-event.md), by taking complements.

For [disjoint occurrence of increasing events](../../../../../../disjoint-occurrence-of-increasing-events.md), a finite open [edge](../../../../../../edge-of-a-graph.md) set $K$ witnesses $A$ in $\omega$ if every configuration agreeing with $\omega$ on $K$ belongs to $A$. Since $A$ is an [increasing event](../../../../../../increasing-event.md) and all [edges](../../../../../../edge-of-a-graph.md) of $K$ are open, this says that the configuration with exactly $K$ open already forces $A$. Define $A\mathbin\square B$ to consist of configurations admitting disjoint finite witnesses $K,L$ for $A,B$. For events depending on finitely many [edges](../../../../../../edge-of-a-graph.md), this is the usual disjoint-occurrence definition; it also applies to finite-connection events on the infinite [graph](../../../../../../graph-split.md). The [Van den Berg-Kesten inequality](../../../../../../van-den-berg-kesten-inequality.md) states

$$
\boxed{\mathbb P_p(A\mathbin\square B)\leq\mathbb P_p(A)\mathbb P_p(B)}.
$$

On a countable [graph](../../../../../../graph-split.md), its finite-witness version follows by taking increasing unions over finite [edge](../../../../../../edge-of-a-graph.md) sets. The [Harris-FKG inequality](../../../../../../harris-fkg-inequality.md) concerns simultaneous occurrence, whereas the [Van den Berg-Kesten inequality](../../../../../../van-den-berg-kesten-inequality.md) requires separate certificates using disjoint coordinates.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 204](../../../paper-204-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
