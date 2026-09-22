<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

An [ultrafilter](../../../../../ultrafilter.md) on $\mathbb N=\{1,2,\ldots\}$ is a family $p\subseteq\mathcal P(\mathbb N)$ satisfying the proper [filter](../../../../../filter-set-theory.md) axioms: $\mathbb N\in p$, $\varnothing\notin p$, [closure](../../../../../closure-topology.md) under finite [intersections](../../../../../set-intersection.md), and upward [closure](../../../../../closure-topology.md) under inclusion. In addition, for every $A\subseteq\mathbb N$, exactly one of $A$ and $A^c$ belongs to $p$. Equivalently, an [ultrafilter](../../../../../ultrafilter.md) is a maximal proper [filter](../../../../../filter-set-theory.md). The [principal ultrafilter](../../../../../principal-ultrafilter.md) at $n$ consists of all [subsets](../../../../../subset.md) containing $n$; an [ultrafilter](../../../../../ultrafilter.md) not of this form is a [nonprincipal ultrafilter](../../../../../nonprincipal-ultrafilter.md).

To prove existence, start with the [cofinite filter](../../../../../cofinite-filter.md) and order the proper [filters](../../../../../filter-set-theory.md) containing it by inclusion. The [union](../../../../../set-union.md) of a chain is still a proper [filter](../../../../../filter-set-theory.md): finitely many of its members lie in one [filter](../../../../../filter-set-theory.md) of the chain, and no constituent contains the empty [set](../../../../../set-split.md). Thus [Zorn lemma](../../../../../zorn-s-lemma.md) supplies a maximal such [filter](../../../../../filter-set-theory.md) $p$. If $A\notin p$, adjoining $A$ cannot generate a proper [filter](../../../../../filter-set-theory.md); otherwise maximality fails. Consequently some $B\in p$ has $B\cap A=\varnothing$, so $A^c\in p$ by upward [closure](../../../../../closure-topology.md). This proves the [ultrafilter](../../../../../ultrafilter.md) alternative. No finite $A$ can belong to $p$, because $A^c$ is [cofinite](../../../../../cofinite-set.md) and already belongs to $p$. In particular $p$ contains no singleton and is a **[nonprincipal ultrafilter](../../../../../nonprincipal-ultrafilter.md)**. The same argument, starting from any proper [filter](../../../../../filter-set-theory.md), proves the [ultrafilter lemma](../../../../../ultrafilter-lemma.md) used below.

Define $\beta\mathbb N$ to be the [set](../../../../../set-split.md) of all [ultrafilters](../../../../../ultrafilter.md) on $\mathbb N$, with basic [open sets](../../../../../open-set.md)

$$
\widehat A=\{p\in\beta\mathbb N:A\in p\},\qquad A\subseteq\mathbb N.
$$

They form a [topological basis](../../../../../basis-of-a-topology.md) because $\widehat{\mathbb N}=\beta\mathbb N$ and $\widehat A\cap\widehat B=\widehat{A\cap B}$. Moreover $(\widehat A)^c=\widehat{A^c}$, so they are [clopen sets](../../../../../clopen-set.md). This is the [compact Hausdorff topology on ultrafilters](../../../../../compact-hausdorff-topology-on-ultrafilters.md). If $p\ne q$, some $A$ belongs to $p$ but not $q$, and then $\widehat A$ and $\widehat{A^c}$ are disjoint open [neighbourhoods](../../../../../neighbourhood-mathematics.md) of the two points. Thus $\beta\mathbb N$ is [Hausdorff](../../../../../hausdorff-space.md).

For [compactness](../../../../../compact-space.md), take an [open cover](../../../../../open-cover.md) and refine it by basic [open sets](../../../../../open-set.md) $\widehat{A_\lambda}$. If no finite subfamily covers, then for every finite collection of indices the [intersection](../../../../../set-intersection.md) $\bigcap A_\lambda^c$ is nonempty. Indeed, if that [intersection](../../../../../set-intersection.md) were empty, the corresponding $A_\lambda$ would cover $\mathbb N$, and every [ultrafilter](../../../../../ultrafilter.md) would contain at least one of them by the finite [ultrafilter](../../../../../ultrafilter.md) alternative. The complements therefore have the [finite intersection property](../../../../../finite-intersection-property.md) and generate a proper [filter](../../../../../filter-set-theory.md). Extend it to an [ultrafilter](../../../../../ultrafilter.md) $q$ by the proved [ultrafilter lemma](../../../../../ultrafilter-lemma.md). Then $A_\lambda^c\in q$ for every $\lambda$, so $q$ belongs to none of the covering $\widehat{A_\lambda}$, a contradiction. A finite basic subcover lies inside a finite subcover of the original cover. Hence

$$
\boxed{\beta\mathbb N\text{ is compact and Hausdorff}.}
$$

The map $n\mapsto p_n$, where $p_n$ is the [principal ultrafilter](../../../../../principal-ultrafilter.md) at $n$, identifies the discrete natural numbers with a [dense subset](../../../../../dense-set.md): any nonempty $\widehat A$ has $A\ne\varnothing$ and contains $p_n$ for $n\in A$.

[Hindman theorem](../../../../../hindman-theorem.md) states that every [finite colouring](../../../../../finite-coloring.md) of the positive [integers](../../../../../integer.md) admits an increasing [sequence](../../../../../sequence.md) $x_1<x_2<\cdots$ whose [finite-sums set](../../../../../finite-sums-set.md)

$$
FS(x_1,x_2,\ldots)=\left\{\sum_{i\in F}x_i:\varnothing\ne F\subseteq\mathbb N\text{ finite}\right\}
$$

is [monochromatic](../../../../../monochromatic-set.md). We now give the [Idempotent-ultrafilter proof of Hindman's theorem](../../../../../idempotent-ultrafilter-proof-of-hindman-s-theorem.md). For $A\subseteq\mathbb N$, write $A-x=\{y\in\mathbb N:x+y\in A\}$. The addition on $\beta\mathbb N$ is defined by

$$
A\in p+q\quad\Longleftrightarrow\quad\{x\in\mathbb N:A-x\in q\}\in p.
$$

Take an [idempotent ultrafilter on the natural numbers](../../../../../idempotent-ultrafilter-on-the-natural-numbers.md) $p$, whose existence is allowed, so $p+p=p$. It is a [nonprincipal ultrafilter](../../../../../nonprincipal-ultrafilter.md): addition of principal points is $p_m+p_n=p_{m+n}$, whereas no positive [integer](../../../../../integer.md) satisfies $2m=m$.

Exactly one [colour class](../../../../../colour-class.md) $A$ belongs to $p$. Define

$$
A^*=A\cap\{x:A-x\in p\}.
$$

By idempotence, $A^*\in p$. The [idempotent-ultrafilter star-set lemma](../../../../../idempotent-ultrafilter-star-set-lemma.md) needed for the recursion is that $A^*-x\in p$ whenever $x\in A^*$. To prove it, put $D=A-x\in p$. Idempotence again gives

$$
D^*=D\cap\{y:D-y\in p\}\in p.
$$

For $y\in D^*$, we have $x+y\in A$ and $A-(x+y)=D-y\in p$, hence $x+y\in A^*$. Thus $D^*\subseteq A^*-x$, proving the lemma by upward [closure](../../../../../closure-topology.md).

Choose $x_1\in A^*$. Suppose $F_n=FS(x_1,\ldots,x_n)\subseteq A^*$ has been constructed. Every factor of

$$
A^*\cap\bigcap_{s\in F_n}(A^*-s)\cap\left\{z:z>\sum_{i=1}^nx_i\right\}
$$

belongs to $p$: the translate factors do by the just-proved lemma, and the last factor does because it is [cofinite](../../../../../cofinite-set.md) and $p$ is a [nonprincipal ultrafilter](../../../../../nonprincipal-ultrafilter.md). The finite [intersection](../../../../../set-intersection.md) is therefore nonempty. Choose $x_{n+1}$ in it. Then $x_{n+1}$ and every $s+x_{n+1}$ with $s\in F_n$ lie in $A^*$, so $F_{n+1}\subseteq A^*$. This constructs a strictly increasing [sequence](../../../../../sequence.md), indeed $x_{n+1}>\sum_{i\le n}x_i$, and proves [Hindman theorem](../../../../../hindman-theorem.md).

Finally apply [Hindman theorem](../../../../../hindman-theorem.md) to obtain a [monochromatic](../../../../../monochromatic-set.md) [finite-sums set](../../../../../finite-sums-set.md) $FS(y_1,y_2,\ldots)$. We construct a [divisibility chain inside a finite-sums set](../../../../../divisibility-chain-inside-a-finite-sums-set.md) using disjoint successive blocks of indices. Start with $x_1=y_1$. If $x_i=m$, take $2m$ unused terms after all indices used so far, and split them into two groups of $m$ consecutive terms. In each group its $m+1$ [partial sums](../../../../../partial-sum.md), including $0$, contain two in the same [congruence class](../../../../../congruence-class.md) modulo $m$ by the [pigeonhole principle](../../../../../pigeonhole-principle.md). Their difference is a nonempty consecutive sum divisible by $m$, and positivity makes it at least $m$. Let $x_{i+1}$ be the sum of these two selected sums. Then $m\mid x_{i+1}$ and $x_{i+1}\ge2m>m$.

The index [set](../../../../../set-split.md) defining $x_{i+1}$ lies strictly after all previous index [sets](../../../../../set-split.md). Discard the other terms in these two groups before continuing. Because the chosen index [sets](../../../../../set-split.md) are disjoint, every finite sum of distinct $x_i$ is a finite sum of distinct $y_j$, retaining the same colour. Therefore

$$
\boxed{x_1<x_2<\cdots,\qquad x_i\mid x_{i+1}\ \text{for every }i,\qquad FS(x_1,x_2,\ldots)\text{ is monochromatic}.}
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
