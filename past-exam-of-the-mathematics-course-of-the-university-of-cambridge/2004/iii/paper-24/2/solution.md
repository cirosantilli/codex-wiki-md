<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [partition relation](../../../../../partition-relation.md) $\lambda\to(\mu)^r_\nu$ says that every [colouring](../../../../../colouring-of-a-set.md) of the $r$-element [subsets](../../../../../subset.md) of a [set](../../../../../set-split.md) of [cardinality](../../../../../cardinality.md) $\lambda$ into $\nu$ colours has a [homogeneous set](../../../../../homogeneous-set-for-a-colouring.md) of [cardinality](../../../../../cardinality.md) $\mu$. Define the [beth numbers](../../../../../beth-number.md) over an infinite [cardinal](../../../../../cardinal-number.md) $\kappa$ by $\beth_0(\kappa)=\kappa$ and $\beth_{n+1}(\kappa)=2^{\beth_n(\kappa)}$. The [Erdős-Rado theorem for finite arities](../../../../../erdos-rado-theorem-for-finite-arities.md) gives the precise bound

$$
\boxed{\beth_n(\kappa)^+\longrightarrow(\kappa^+)^{n+1}_\kappa\qquad(n<\omega).}
$$

Thus any fixed finite arity and any fixed infinite number of colours admit arbitrarily large infinite [monochromatic sets](../../../../../monochromatic-set.md) once the starting [cardinal](../../../../../cardinal-number.md) is sufficiently large. For pairs, the especially useful case is $(2^\kappa)^+\to(\kappa^+)^2_\kappa$. The successor in this bound matters: a binary first-difference colouring on a suitably ordered [set](../../../../../set-split.md) of binary [sequences](../../../../../sequence.md) supplies the familiar obstruction at $2^\kappa$. Also, a theorem for every fixed finite arity is not a theorem homogenizing all arities simultaneously.

The mechanism is to build an [end-homogeneous routing tree](../../../../../end-homogeneous-routing-tree.md): each new vertex is routed according to its colours to earlier vertices on its branch. A long branch is end-homogeneous, meaning the colour from a fixed earlier vertex is independent of the later vertex. There are at most $\kappa^\alpha\leq2^\kappa$ routes of length $\alpha<\kappa^+$, and the whole collection of short routes has size at most $2^\kappa$. Inserting $(2^\kappa)^+$ vertices therefore forces a branch of length $\kappa^+$. One colour occurs at $\kappa^+$ earlier vertices on that branch, giving the pair theorem. Iterating the higher-arity version of this routing construction explains the successive powers in the [Erdős-Rado theorem for finite arities](../../../../../erdos-rado-theorem-for-finite-arities.md).

A [weakly compact cardinal](../../../../../weakly-compact-cardinal.md) is an uncountable [strongly inaccessible cardinal](../../../../../strongly-inaccessible-cardinal.md) $\kappa$ with

$$
\kappa\longrightarrow(\kappa)^2_2.
$$

Equivalent formulations include the [tree property](../../../../../tree-property.md) at the inaccessible [cardinal](../../../../../cardinal-number.md) and compactness for theories of size at most $\kappa$ in the infinitary language $L_{\kappa,\kappa}$: if every subtheory of size $<\kappa$ has a [first-order model](../../../../../model-of-a-first-order-theory.md), so does the theory.

A [measurable cardinal](../../../../../measurable-cardinal.md) is an uncountable $\kappa$ carrying a [nonprincipal ultrafilter](../../../../../nonprincipal-ultrafilter.md) [closed](../../../../../closed-set.md) under intersections of fewer than $\kappa$ members. Such an [ultrafilter](../../../../../ultrafilter.md) contains no [set](../../../../../set-split.md) of size $<\kappa$, since all singletons have complements in it and it is [kappa-complete](../../../../../kappa-complete-filter.md). Consequently a cofinal [sequence](../../../../../sequence.md) of length $<\kappa$ would partition $\kappa$ into too few small pieces, so $\kappa$ is [regular cardinal](../../../../../regular-cardinal.md). If $\lambda<\kappa$ and $\kappa$ distinct [subsets](../../../../../subset.md) of $\lambda$ existed, choose, for each coordinate of $\lambda$, the bit selected by the [ultrafilter](../../../../../ultrafilter.md). [Kappa-completeness](../../../../../kappa-complete-filter.md) would make all those bits simultaneously constant on a large [set](../../../../../set-split.md) of indices; only one distinct [subset](../../../../../subset.md) could have that bit pattern, a contradiction. Hence $2^\lambda<\kappa$: $\kappa$ is also a [strong limit cardinal](../../../../../strong-limit-cardinal.md).

A [supercompact cardinal](../../../../../supercompact-cardinal.md) $\kappa$ has, for every $\lambda\geq\kappa$, a [fine ultrafilter](../../../../../fine-ultrafilter.md) that is a [normal ultrafilter on small subsets](../../../../../normal-ultrafilter-on-small-subsets.md) and is [kappa-complete](../../../../../kappa-complete-filter.md) on

$$
P_\kappa(\lambda)=\{x\subseteq\lambda:|x|<\kappa\}.
$$

Fine means $\{x:\alpha\in x\}$ is large for every $\alpha<\lambda$. Normal means that a [function](../../../../../function-split.md) $f$ with $f(x)\in x$ on a large [set](../../../../../set-split.md) is constant on some large [set](../../../../../set-split.md). Equivalently, for every such $\lambda$ there is an [elementary embedding](../../../../../elementary-embedding.md) $j:V\to M$ with [critical point](../../../../../critical-point.md) $\kappa$, $j(\kappa)>\lambda$, and $M$ [closed](../../../../../closed-set.md) under $\lambda$-sequences from the universe.

These notions form the implication chain **supercompact $\Rightarrow$ measurable $\Rightarrow$ weakly compact**. For the first implication, an embedding as above gives the measure $U=\{X\subseteq\kappa:\kappa\in j(X)\}$. For the second, use a [normal ultrafilter on a cardinal](../../../../../normal-ultrafilter-on-a-cardinal.md) obtained by normalizing its measure. Indeed the [ultrapower embedding](../../../../../ultrapower-embedding.md) gives the measure $U=\{X\subseteq\kappa:\kappa\in j(X)\}$; for a regressive $f$, $j(f)(\kappa)<\kappa$ is a fixed [ordinal](../../../../../ordinal.md), yielding the required constant large fibre. Given a pair-colouring, select for each $\alpha$ the measure-one colour on the tail above $\alpha$. One selected colour occurs on a measure-one [set](../../../../../set-split.md) of $\alpha$'s. Normality makes the diagonal intersection of their selected tails measure one; any two members of that intersection have the selected colour. This gives the required [partition relation](../../../../../partition-relation.md), and the preceding regularity and strong-limit argument gives inaccessibility.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 24](../../paper-24-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
