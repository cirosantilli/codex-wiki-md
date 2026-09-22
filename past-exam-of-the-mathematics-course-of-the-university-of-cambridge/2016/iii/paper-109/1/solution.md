<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a family $\mathcal F\subseteq\binom{[n]}r$, let its [lower shadow](../../../../../lower-shadow.md) $\partial\mathcal F$ consist of all $(r-1)$-sets contained in members of $\mathcal F$. The **local LYM inequality** is

$$
\boxed{\frac{|\partial\mathcal F|}{\binom n{r-1}}\geq\frac{|\mathcal F|}{\binom nr}\qquad(1\leq r\leq n).}
$$

To prove it, use [double counting](../../../../../double-counting-proof-technique.md) on the pairs $(T,S)$ with $S\in\mathcal F$, $T\subset S$ and $|T|=r-1$. Each $S$ contributes $r$ pairs; each $T\in\partial\mathcal F$ contributes at most $n-r+1$. Hence $r|\mathcal F|\leq(n-r+1)|\partial\mathcal F|$, exactly the displayed [Local LYM inequality](../../../../../local-lym-inequality.md) after using $r\binom nr=(n-r+1)\binom n{r-1}$.

To deduce the [LYM inequality](../../../../../lubell-yamamoto-meshalkin-inequality.md), start with an [antichain](../../../../../antichain.md) $\mathcal A$ in the [Boolean lattice](../../../../../boolean-lattice.md) and assign it weight $\sum_{S\in\mathcal A}\binom n{|S|}^{-1}$. If its largest occupied rank is $r>0$, replace that whole rank by its [lower shadow](../../../../../lower-shadow.md). The result remains an [antichain](../../../../../antichain.md): if an old lower-rank member were contained in a new shadow member, it would also be contained in an original rank-$r$ member, contradicting the original [antichain](../../../../../antichain.md) property. Nor can a new member be contained in an old one, since every old member has size at most $r-1$ and equality would give the same contradiction. The [Local LYM inequality](../../../../../local-lym-inequality.md) shows that this replacement does not decrease the weight. Repeating eventually leaves an [antichain](../../../../../antichain.md) on rank zero, whose weight is at most one. Therefore

$$
\boxed{\sum_{S\in\mathcal A}\frac1{\binom n{|S|}}\leq1.}
$$

For the empty family the conclusion is immediate; the same argument includes the singleton family containing the empty set.

**The [antichains](../../../../../antichain.md) of maximum size are exactly the full middle levels.** More precisely, for even $n$ only $\binom{[n]}{n/2}$ attains the bound in [Sperner theorem](../../../../../sperner-s-theorem.md); for odd $n$ either $\binom{[n]}{(n-1)/2}$ or $\binom{[n]}{(n+1)/2}$ does. To prove that there are no others, put $M=\binom n{\lfloor n/2\rfloor}$. If $|\mathcal A|=M$, the [LYM inequality](../../../../../lubell-yamamoto-meshalkin-inequality.md) and $\binom nr\leq M$ imply equality in every term's bound $1/\binom nr\geq1/M$. Thus every member lies on a middle level. For even $n$, there is only one such level, so it must be full.

For odd $n=2r+1$, let $X$ be the rank-$r$ members and $Y$ the rank-$(r+1)$ members. Consider the [bipartite graph](../../../../../bipartite-graph.md) of inclusions between those levels. Both parts have size $M$, and the [degree of a vertex](../../../../../degree-graph-theory.md) is $r+1$. If $N(X)$ is the [neighbourhood](../../../../../neighbourhood-mathematics.md) of $X$, [double counting](../../../../../double-counting-proof-technique.md) gives $|N(X)|\geq|X|$. Since the family is an [antichain](../../../../../antichain.md), $Y$ avoids $N(X)$; equality $|X|+|Y|=M$ forces $|N(X)|=|X|$ and $Y$ to be the full complement of $N(X)$. Equality in the degree count means that every edge into $N(X)$ comes from $X$, so there are no edges between $X\cup N(X)$ and its complement.

This inclusion [graph](../../../../../graph-split.md) is [connected](../../../../../connected-space.md): any two $r$-sets can be joined by successively exchanging one element, and each exchange passes through their $(r+1)$-set union. Every upper vertex has a lower neighbour. Thus $X$ must be empty or the whole lower level, proving the classification. For $n=1$ the graph is just one edge, and for $n=0$ the unique maximum family is $\{\varnothing\}$. This establishes [equality in Sperner theorem](../../../../../equality-in-sperner-theorem.md) without assuming that equality in the [LYM inequality](../../../../../lubell-yamamoto-meshalkin-inequality.md) alone always forces a middle level.

For the set-pair bound, choose a uniformly random [permutation](../../../../../permutation.md) of $[n]$, and let $E_i$ be the [event](../../../../../event.md) that every element of $A_i$ appears before every element of $B_i$. Since $A_i\cap B_i=\varnothing$, their relative order is uniform, and

$$
\mathbb P(E_i)=\frac{|A_i|!\,|B_i|!}{(|A_i|+|B_i|)!}=\binom{|A_i|+|B_i|}{|A_i|}^{-1}.
$$

For distinct $i,j$, choose $a\in A_i\cap B_j$ and $b\in A_j\cap B_i$. These are distinct because $A_i\cap B_i$ is empty. On $E_i$, $a$ precedes $b$; on $E_j$, $b$ precedes $a$. Thus the events are pairwise [disjoint events](../../../../../disjoint-events.md), giving **the Bollobas set-pairs inequality**

$$
\boxed{\sum_i\binom{|A_i|+|B_i|}{|A_i|}^{-1}=\mathbb P\left(\bigcup_iE_i\right)\leq1.}
$$

This [Bollobas set-pairs inequality](../../../../../bollobas-set-pairs-inequality.md) immediately gives another proof of the [LYM inequality](../../../../../lubell-yamamoto-meshalkin-inequality.md): enumerate the members $S_i$ of an [antichain](../../../../../antichain.md), and take $A_i=S_i$, $B_i=[n]\setminus S_i$. For $i\ne j$, incomparability means $S_i\setminus S_j\ne\varnothing$, while $A_i\cap B_i=\varnothing$. The set-pair hypotheses therefore hold, and $|A_i|+|B_i|=n$ makes the resulting sum exactly the [LYM inequality](../../../../../lubell-yamamoto-meshalkin-inequality.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 109](../../paper-109-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
