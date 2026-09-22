<h1 id="9/solution">Solution</h1>

↑ **Parent:** [9](../9.md)

An [uncountable](../../../../../uncountable-set.md) cardinal $\kappa$ is a [measurable cardinal](../../../../../measurable-cardinal.md) if there is a nonprincipal $\kappa$-complete [ultrafilter](../../../../../ultrafilter.md) $U$ on $\kappa$: [intersections](../../../../../set-intersection.md) of fewer than $\kappa$ members of $U$ remain in $U$. Such an [ultrafilter](../../../../../ultrafilter.md) is uniform. No [singleton](../../../../../singleton-mathematics.md) belongs to it, and intersecting the complements of fewer than $\kappa$ [singletons](../../../../../singleton-mathematics.md) shows that no [set](../../../../../set-split.md) of [cardinality](../../../../../cardinality.md) below $\kappa$ belongs to it.

Form the [ultrapower](../../../../../ultrapower.md) of the universe by $U$, with classes $[f]$ of [functions](../../../../../function-split.md) $f:\kappa\to V$, and $[f]\in_U[g]$ exactly when $\{\xi:f(\xi)\in g(\xi)\}\in U$. The [Łoś theorem](../../../../../los-theorem.md) proves that the map taking $x$ to the constant [function](../../../../../function-split.md) with value $x$ is elementary. The [ultrapower](../../../../../ultrapower.md) relation is well-founded: from an infinite descending [sequence](../../../../../sequence.md) $[f_0]\ni_U[f_1]\ni_U\cdots$, [countable](../../../../../countable-set.md) completeness gives a coordinate satisfying all the membership relations, producing an actual infinite descending membership [sequence](../../../../../sequence.md) and contradicting [foundation](../../../../../axiom-of-regularity.md). It is also set-like. Predecessors of $[g]$ can be represented by [functions](../../../../../function-split.md) whose value at $\xi$ lies in $g(\xi)\cup\{\varnothing\}$; these [functions](../../../../../function-split.md) form a [set](../../../../../set-split.md). The [Mostowski collapse theorem](../../../../../mostowski-collapse-theorem.md) therefore gives a [transitive class](../../../../../transitive-class.md) $N$ and an [elementary embedding](../../../../../elementary-embedding.md)

$$
j:V\longrightarrow N.
$$

The usual class-ultrapower notation is understood via set-sized representatives and this set-like collapse.

For $\alpha<\kappa$, any [function](../../../../../function-split.md) into $\alpha$ is constant on a $U$-large [set](../../../../../set-split.md): if none of its fewer-than-$\kappa$ fibers belonged to $U$, intersect their complements to get the [empty set](../../../../../empty-set.md) in $U$. Consequently every member of the [ultrapower](../../../../../ultrapower.md) [ordinal](../../../../../ordinal.md) represented by the constant $\alpha$ is represented by a constant [ordinal](../../../../../ordinal.md) below $\alpha$. Induction on $\alpha$ now gives $j(\alpha)=\alpha$.

On the other hand the identity [function](../../../../../function-split.md) $d(\xi)=\xi$ represents an [ordinal](../../../../../ordinal.md) below $j(\kappa)$. For every $\alpha<\kappa$, the tail $\{\xi:\xi>\alpha\}$ belongs to $U$, so the collapsed [ordinal](../../../../../ordinal.md) $[d]$ is above $j(\alpha)=\alpha$. Hence

$$
\boxed{\operatorname{crit}(j)=\kappa,\qquad j(\kappa)>\kappa.}
$$

This proves nonidentity explicitly. The collapsed identity class is at least $\kappa$; it need not equal $\kappa$ unless an additional normality convention is imposed on $U$.

Conversely, an [elementary embedding](../../../../../elementary-embedding.md) $j:V\to N$ into a [transitive class](../../../../../transitive-class.md) with critical point $\kappa$ yields

$$
U=\{X\subseteq\kappa:\kappa\in j(X)\}.
$$

For the converse use the usual amenability assumption on the class embedding, so this collection is a [set](../../../../../set-split.md). Since $j(\kappa)>\kappa$, exactly one of $j(X)$ and $j(\kappa\setminus X)$ contains $\kappa$, proving the [ultrafilter](../../../../../ultrafilter.md) condition. [Singletons](../../../../../singleton-mathematics.md) are excluded because $j(\alpha)=\alpha<\kappa$. If $\lambda<\kappa$ and $X_i\in U$ for $i<\lambda$, then $j$ fixes $\lambda$ and every index below it, giving $j(\bigcap_{i<\lambda}X_i)=\bigcap_{i<\lambda}j(X_i)$; the [intersection](../../../../../set-intersection.md) still contains $\kappa$. Thus $U$ is $\kappa$-complete and $\kappa$ is measurable.

In particular the first moved [ordinal](../../../../../ordinal.md) is a [strongly inaccessible cardinal](../../../../../strongly-inaccessible-cardinal.md). If $\operatorname{cf}(\kappa)<\kappa$, partition $\kappa$ into fewer than $\kappa$ bounded intervals. Each is too small to lie in $U$, contradicting completeness. Thus $\kappa$ is regular. If $2^\lambda\ge\kappa$ for some $\lambda<\kappa$, choose distinct [subsets](../../../../../subset.md) $A_\xi\subseteq\lambda$ for $\xi<\kappa$. For each $\eta<\lambda$, choose the $U$-large side of the question $\eta\in A_\xi$. Intersect these fewer-than-$\kappa$ large sides. The [intersection](../../../../../set-intersection.md) belongs to $U$, but all its indices have identical $A_\xi$, so it contains at most one index, contradicting nonprincipality. Therefore $2^\lambda<\kappa$ for every $\lambda<\kappa$, as required.

## ↑ Ancestors (10)

1. [9](../9.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
