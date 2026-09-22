<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [measurable cardinal](../../../../../../measurable-cardinal.md) is an uncountable [cardinal](../../../../../../cardinal-number.md) $\kappa$ carrying a nonprincipal $\kappa$-complete [ultrafilter](../../../../../../ultrafilter.md) $U$: intersections of fewer than $\kappa$ members of $U$ remain in $U$. Such an [ultrafilter](../../../../../../ultrafilter.md) contains no set of size less than $\kappa$. Indeed each singleton is absent, and intersecting fewer than $\kappa$ singleton complements shows that every small set's complement is in $U$. In particular every tail of $\kappa$ is in $U$.

Form the [ultrapower](../../../../../../ultrapower.md) of the universe by functions $f:\kappa\to V$, identifying functions agreeing on a member of $U$, and interpreting membership coordinatewise modulo $U$. The [Łoś theorem](../../../../../../los-theorem.md), applied separately to each formula, makes the map $x\mapsto[c_x]$ elementary. Countable completeness makes the [ultrapower](../../../../../../ultrapower.md) well-founded: an infinite descending chain $[f_{n+1}]\in[f_n]$ would give $U$-large sets witnessing each step, whose countable intersection is nonempty; a coordinate in that intersection would give an infinite descending membership chain in the original universe. The relation is extensional and set-like, so the [Mostowski collapse theorem](../../../../../../mostowski-collapse-theorem.md) gives a transitive class $M$ and an elementary [ultrapower embedding](../../../../../../ultrapower-embedding.md) $j:V\to M$.

For each $\alpha<\kappa$, every function $\kappa\to\alpha$ is constant modulo $U$. If no fibre were in $U$, intersecting the fewer than $\kappa$ fibre complements would give the empty set in $U$. Induction on $\alpha$ therefore shows that the collapsed [ultrapower](../../../../../../ultrapower.md) [ordinal](../../../../../../ordinal.md) $j(\alpha)$ has precisely the elements $\beta<\alpha$, so

$$
j(\alpha)=\alpha\quad(\alpha<\kappa).
$$

The identity function $\operatorname{id}:\kappa\to\kappa$ represents an [ordinal](../../../../../../ordinal.md) below $j(\kappa)$, and every constant $\alpha<\kappa$ is below it modulo $U$, since a tail is large. Consequently

$$
\boxed{\kappa\leq[\operatorname{id}]^{\mathrm{collapse}}<j(\kappa),\qquad
\operatorname{crit}(j)=\kappa.}
$$

Thus **the canonical collapsed embedding is not the identity; its first moved [ordinal](../../../../../../ordinal.md) is $\kappa$**. For a general measure the identity-function class need not collapse to exactly $\kappa$; that stronger equality holds for a normal measure. The argument above needs only its lower bound.

Conversely, suppose $j:V\to M$ is elementary, $M$ is transitive, its critical point is $\kappa$, and its derived measure is a set, as for the usual definable or amenable class embeddings. Define

$$
U=\{A\subseteq\kappa:\kappa\in j(A)\}.
$$

Because $\kappa<j(\kappa)$, elementary preservation of complements and intersections makes this an [ultrafilter](../../../../../../ultrafilter.md). It is nonprincipal since $j(\{\alpha\})=\{\alpha\}$ for $\alpha<\kappa$. For a sequence of $\gamma<\kappa$ large sets, $j$ fixes the index [ordinal](../../../../../../ordinal.md) $\gamma$ and takes the intersection to the intersection of their images; $\kappa$ belongs to every image and hence to the intersection. Thus $U$ is $\kappa$-complete. The set-existence qualification excludes treating an arbitrary external class map as a set parameter without justification.

For context, measurability already implies regularity and the strong-limit property. A cofinal sequence of length below $\kappa$ partitions $\kappa$ into that many bounded, hence small, pieces; completeness and their absent fibres contradict covering all of $\kappa$. If there were $\kappa$ distinct subsets of some $\lambda<\kappa$, for each coordinate choose the $U$-large side deciding its membership bit. The intersection of these $\lambda$ large sets would still be large, but all its indices would label the same subset, so it would have at most one member. This contradiction gives $2^\lambda<\kappa$. Thus the first moved [ordinal](../../../../../../ordinal.md) is an uncountable [strongly inaccessible cardinal](../../../../../../strongly-inaccessible-cardinal.md), in addition to being measurable.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
