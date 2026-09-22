<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

A [measurable cardinal](../../../../../measurable-cardinal.md) is an uncountable cardinal $\kappa$ carrying a [nonprincipal ultrafilter](../../../../../nonprincipal-ultrafilter.md) $U$ on $\kappa$ that is $\kappa$-complete: intersections of fewer than $\kappa$ members of $U$ remain in $U$. An [elementary embedding](../../../../../elementary-embedding.md) $j:M\to N$ preserves truth of every [first-order formula](../../../../../first-order-formula.md), with its parameters carried along by $j$.

The identity is always an elementary embedding of the universe into itself. The substantive question concerns a nonidentity embedding. In [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md), the [Kunen inconsistency theorem](../../../../../kunen-inconsistency-theorem.md) gives

$$
\boxed{\text{There is no nontrivial elementary embedding }j:V\to V.}
$$

Here, as usual for class embeddings, restrictions to sets and the recursively defined critical sequence are available. We give the stationary-set proof, including its partition ingredient.

Suppose such a $j$ existed. It has a least moved [ordinal](../../../../../ordinal.md) $\kappa$, its [critical point of an elementary embedding](../../../../../critical-point-of-an-elementary-embedding.md). To see why some [ordinal](../../../../../ordinal.md) must move, if all [ordinals](../../../../../ordinal.md) were fixed, induction on rank would fix every set: membership of $z$ in $j(x)$ is equivalent to membership of $z$ in $x$ once every lower-rank $z$ is fixed. A rank segment containing a moved set would then be fixed pointwise, a contradiction. The critical point is an uncountable cardinal. All finite [ordinals](../../../../../ordinal.md) and $\omega$ are definable and fixed. If $\kappa$ had [cardinality](../../../../../cardinality.md) $\mu<\kappa$, a bijection $f:\mu\to\kappa$ would be carried to a surjection $j(f):\mu\to j(\kappa)$ whose range still consists exactly of the fixed [ordinals](../../../../../ordinal.md) below $\kappa$, impossible since $j(\kappa)>\kappa$.

Put $\kappa_0=\kappa$, $\kappa_{n+1}=j(\kappa_n)$ and $\lambda=\sup_{n<\omega}\kappa_n$. Applying $j$ to this [Kunen critical sequence](../../../../../kunen-critical-sequence.md) shifts it by one, so $j(\lambda)=\lambda$. Elementarity also gives $j(\lambda^+)=\lambda^+$; write $\theta=\lambda^+$.

We need a [stationary partition at a successor cardinal](../../../../../stationary-partition-at-a-successor-cardinal.md). If $S\subseteq\lambda^+$ is stationary, choose bijections $e_\beta:\lambda\to\beta$ for $\lambda\leq\beta<\lambda^+$. For each $\xi<\lambda^+$, on the stationary tail $\{\beta\in S:\beta>\max(\lambda,\xi)\}$ the function $\beta\mapsto e_\beta^{-1}(\xi)$ is regressive. The [Fodor lemma](../../../../../fodor-lemma.md) supplies a stationary fiber $E_\xi$ with constant value $i_\xi<\lambda$. Some value $i$ occurs for $\lambda^+$ many $\xi$, since a union of $\lambda$ sets each of size at most $\lambda$ cannot have size $\lambda^+$. For distinct such $\xi$, their fibers are disjoint: $e_\beta(i)$ cannot equal two different [ordinals](../../../../../ordinal.md). These fibers yield $\lambda^+$ disjoint stationary subsets; include any leftover points in one cell. Grouping cells also gives a partition into any nonzero number at most $\lambda^+$.

For completeness, the [Fodor lemma](../../../../../fodor-lemma.md) used here follows from diagonal intersections of clubs. If a regressive function $f:S\to\theta$ had no stationary fiber, choose a [club set](../../../../../club-set.md) $C_\xi$ disjoint from each fiber. The diagonal intersection $\{\beta<\theta:\forall\xi<\beta\ (\beta\in C_\xi)\}$ is club by regularity and closure. A point $\beta$ in its intersection with $S$ would belong to $C_{f(\beta)}$, contradicting the choice of that club.

The set $S=\{\beta<\theta:\operatorname{cf}(\beta)=\omega\}$ is stationary: inside any club choose a strictly increasing countable sequence, whose supremum still lies below the regular uncountable $\theta$ and belongs to the club. Partition it as $\langle S_\alpha:\alpha<\kappa\rangle$. Its image $\langle T_\alpha:\alpha<j(\kappa)\rangle$ is another stationary partition of the same $S$.

The set $C=\{\beta<\theta:j\mathbin{``}\beta\subseteq\beta\}$ is club. Closure is immediate. To get a member above any given [ordinal](../../../../../ordinal.md), repeatedly bound the images of all earlier [ordinals](../../../../../ordinal.md) and take a countable supremum; regularity of $\theta$ keeps each bound below $\theta$. Choose $\beta\in C\cap T_\kappa$. Since $\operatorname{cf}(\beta)=\omega$, a countable cofinal sequence in $\beta$ and $j(\omega)=\omega$ give $j(\beta)=\beta$: the image sequence remains below $\beta$ by closure under $j$, and $j(\beta)\geq\beta$.

But $\beta\in S_\alpha$ for some $\alpha<\kappa$. Applying $j$ and using $j(\alpha)=\alpha$ gives $\beta=j(\beta)\in T_\alpha$, contradicting its membership in the disjoint cell $T_\kappa$. This proves the assertion. The use of [axiom of choice](../../../../../axiom-of-choice.md) in the cardinal and stationary-partition arguments matters; the conclusion here is explicitly in ZFC.

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 26](../../paper-26-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
