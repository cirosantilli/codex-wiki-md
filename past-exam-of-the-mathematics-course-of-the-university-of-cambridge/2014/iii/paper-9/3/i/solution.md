<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A proper [filter on a set](../../../../../../filter-set-theory.md) $\mathcal F$ on $\mathbb N$ contains $\mathbb N$, excludes the empty set, is closed under finite intersections and is upward closed under inclusion. An [ultrafilter](../../../../../../ultrafilter.md) is a maximal proper filter. Equivalently, for every $A\subseteq\mathbb N$ it contains exactly one of $A,A^c$. To see maximality implies this dichotomy, if $A$ is absent then adjoining it must make the generated filter improper; hence some filter member is disjoint from $A$, forcing $A^c$ into the filter. Conversely, a filter with this dichotomy cannot be properly enlarged without acquiring disjoint members.

Extend the [cofinite filter](../../../../../../cofinite-filter.md) to a maximal proper filter using [Zorn's lemma](../../../../../../zorn-s-lemma.md). Every chain of proper extensions has its union as a proper filter upper bound: any finite collection of its members lies in one member of the chain, and the empty set never enters. The resulting ultrafilter contains no finite set, because it already contains that set's cofinite complement. It is therefore a [free ultrafilter](../../../../../../nonprincipal-ultrafilter.md), or [nonprincipal ultrafilter](../../../../../../nonprincipal-ultrafilter.md). This proves the required existence with the usual choice principle explicit.

Define the [Stone-Čech compactification of the natural numbers](../../../../../../stone-cech-compactification-of-the-natural-numbers.md) as the set of all ultrafilters, with basic open sets

$$
\widehat A=\{\mathcal U:A\in\mathcal U\}\qquad(A\subseteq\mathbb N).
$$

They form a basis because $\widehat{\mathbb N}$ is the whole space and $\widehat A\cap\widehat B=\widehat{A\cap B}$. Also $(\widehat A)^c=\widehat{A^c}$, so each basic set is [clopen](../../../../../../clopen-set.md). Distinct ultrafilters disagree on some $A$, putting them in the disjoint open sets $\widehat A$ and $\widehat{A^c}$. Thus this space is [Hausdorff](../../../../../../hausdorff-space.md).

To prove compactness, suppose an open cover has no finite subcover and refine it by basic sets $\widehat{A_i}$. Their complements $B_i=\mathbb N\setminus A_i$ have the [finite intersection property](../../../../../../finite-intersection-property.md): otherwise finitely many $\widehat{A_i}$ would cover every ultrafilter. Here a nonempty finite intersection of the $B_i$ has a principal ultrafilter containing it, whereas an empty intersection cannot belong to any proper filter. The $B_i$ therefore generate a proper filter, which extends to an ultrafilter by the same Zorn argument. That ultrafilter lies outside every $\widehat{A_i}$, contradicting the cover. Hence **$\beta\mathbb N$ is compact and Hausdorff**. Natural number $n$ is identified with its [principal ultrafilter](../../../../../../principal-ultrafilter.md).

[Hindman's theorem](../../../../../../hindman-theorem.md) asserts that every finite colouring of the positive integers has an increasing sequence $x_1<x_2<\cdots$ for which all nonempty finite sums of distinct terms have one colour. Let $\mathcal U+\mathcal U=\mathcal U$ be the given [idempotent ultrafilter](../../../../../../idempotent-ultrafilter.md). Since $\mathbb N$ is positive, a principal ultrafilter cannot be idempotent: its sum with itself is principal at $2n$, not $n$. Thus $\mathcal U$ is nonprincipal and contains every cofinite tail. In a convention including zero, one instead uses an idempotent in the nonprincipal part, excluding the trivial principal idempotent at zero.

For $A\subseteq\mathbb N$ define $A-n=\{m:n+m\in A\}$. [Addition on the Stone-Čech compactification of the natural numbers](../../../../../../addition-on-the-stone-cech-compactification-of-the-natural-numbers.md) is characterized by

$$
A\in\mathcal U+\mathcal V\quad\Longleftrightarrow\quad\{n:A-n\in\mathcal V\}\in\mathcal U.
$$

One cell $A$ of the finite colour partition belongs to $\mathcal U$. Put

$$
A^*=\{n\in A:A-n\in\mathcal U\}.
$$

Idempotence makes $A^*\in\mathcal U$. Moreover, if $n\in A^*$, then $A^*-n\in\mathcal U$. Indeed, write $B=\{y:A-y\in\mathcal U\}$ so $A^*=A\cap B$. We have $A-n\in\mathcal U$, and idempotence applied to that set gives

$$
B-n=\{y:(A-n)-y\in\mathcal U\}\in\mathcal U.
$$

Their intersection is $A^*-n$. This is the [idempotent-ultrafilter star-set lemma](../../../../../../idempotent-ultrafilter-star-set-lemma.md).

Choose $x_1\in A^*$. If the finite-sums set $F_k$ of the first $k$ choices lies in $A^*$, select

$$
x_{k+1}\in A^*\cap\bigcap_{s\in F_k}(A^*-s)\cap\{n:n>x_k\}.
$$

Every factor belongs to $\mathcal U$, so this finite intersection is nonempty. Its choice preserves $F_{k+1}\subseteq A^*$. Therefore

$$
\boxed{\operatorname{FS}(x_1,x_2,\ldots)\subseteq A^*\subseteq A.}
$$

This proves the requested [Idempotent-ultrafilter proof of Hindman's theorem](../../../../../../idempotent-ultrafilter-proof-of-hindman-s-theorem.md), without assuming an idempotent-existence proof.

Finally, for the first logical assertion put $P=\{x:p(x)\}$ and $Q=\{x:q(x)\}$. A proper filter contains $P\cap Q$ if and only if it contains both $P$ and $Q$: one direction is finite-intersection closure and the other is upward closure. Thus **(i) is always true**. This is the [conjunction law for filter quantifiers](../../../../../../conjunction-law-for-filter-quantifiers.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
