<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $\binom{[n]}k$ for the $k$th [uniform layer of the Boolean cube](../../../../../uniform-layer-of-the-boolean-cube.md). For $\mathcal F\subseteq\binom{[n]}k$, $1\leq k\leq n$, its [lower shadow](../../../../../lower-shadow.md) is $\partial\mathcal F=\{B:|B|=k-1,\ B\subset A\text{ for some }A\in\mathcal F\}$. The [Local LYM inequality](../../../../../local-lym-inequality.md) states

$$
\boxed{\frac{|\partial\mathcal F|}{\binom n{k-1}}\geq\frac{|\mathcal F|}{\binom nk}.}
$$

To prove it, count pairs $(B,A)$ with $A\in\mathcal F$, $B\subset A$ and $|B|=k-1$. Each $A$ contributes $k$ pairs; each member of the [lower shadow](../../../../../lower-shadow.md) contributes at most $n-k+1$. Thus $k|\mathcal F|\leq(n-k+1)|\partial\mathcal F|$, which is exactly the displayed [Local LYM inequality](../../../../../local-lym-inequality.md). The corresponding [upper shadow](../../../../../upper-shadow.md) inequality follows either by taking [complements](../../../../../complement-of-a-set.md) or by counting upward inclusion pairs.

For an [antichain](../../../../../antichain.md) $\mathcal A\subseteq\mathcal P([n])$, put $\mathcal A_k=\mathcal A\cap\binom{[n]}k$. The [LYM inequality](../../../../../lubell-yamamoto-meshalkin-inequality.md) is

$$
\boxed{\sum_{k=0}^n\frac{|\mathcal A_k|}{\binom nk}\leq1.}
$$

For the first proof, set $\mathcal B_n=\mathcal A_n$ and recursively $\mathcal B_k=\mathcal A_k\cup\partial\mathcal B_{k+1}$. Every member of $\mathcal B_{k+1}$ is a subset of an original member of $\mathcal A$ of size at least $k+1$. Consequently $\mathcal A_k$ and $\partial\mathcal B_{k+1}$ are disjoint: otherwise one original member would properly contain another, contradicting the [antichain](../../../../../antichain.md) condition. The [Local LYM inequality](../../../../../local-lym-inequality.md) now gives

$$
\frac{|\mathcal B_k|}{\binom nk}
\geq\frac{|\mathcal A_k|}{\binom nk}
+\frac{|\mathcal B_{k+1}|}{\binom n{k+1}}.
$$

Iterating down to $k=0$ bounds the desired sum by $|\mathcal B_0|\leq1$, proving the [LYM inequality](../../../../../lubell-yamamoto-meshalkin-inequality.md).

For the second proof, a [permutation](../../../../../permutation.md) $(i_1,\ldots,i_n)$ determines a [maximal chain in a Boolean lattice](../../../../../maximal-chain-in-a-boolean-lattice.md) through the successive initial subsets $\varnothing,\{i_1\},\ldots,[n]$. A member $A$ of size $k$ lies on exactly $k!(n-k)!$ of these $n!$ [maximal chains in a Boolean lattice](../../../../../maximal-chain-in-a-boolean-lattice.md). An [antichain](../../../../../antichain.md) meets each such [chain in a partially ordered set](../../../../../chain-in-a-partially-ordered-set.md) at most once. Counting its incidences with the [maximal chains in a Boolean lattice](../../../../../maximal-chain-in-a-boolean-lattice.md) therefore yields $\sum_{A\in\mathcal A}|A|!(n-|A|)!\leq n!$. Division by $n!$ is the [LYM inequality](../../../../../lubell-yamamoto-meshalkin-inequality.md) again.

The [Sperner theorem](../../../../../sperner-s-theorem.md) says that an [antichain](../../../../../antichain.md) has at most $M=\binom n{\lfloor n/2\rfloor}$ members. Indeed $\binom nk\leq M$ for every $k$, so

$$
\frac{|\mathcal A|}{M}\leq\sum_k\frac{|\mathcal A_k|}{\binom nk}\leq1.
$$

The middle [uniform layer of the Boolean cube](../../../../../uniform-layer-of-the-boolean-cube.md) attains the bound. For [equality in Sperner theorem](../../../../../equality-in-sperner-theorem.md), equality throughout forces every member to lie in a layer of maximum size. If $n=2k$, this forces $\mathcal A=\binom{[n]}k$.

If $n=2k+1$, only ranks $k$ and $k+1$ are possible. Let $\mathcal L=\mathcal A_k$, $\mathcal U=\mathcal A_{k+1}$, and $\mathcal S=\nabla\mathcal L$ be the [upper shadow](../../../../../upper-shadow.md). The [antichain](../../../../../antichain.md) condition gives $\mathcal U\cap\mathcal S=\varnothing$. The [Local LYM inequality](../../../../../local-lym-inequality.md) for the two equally sized middle layers gives $|\mathcal S|\geq|\mathcal L|$, while $|\mathcal L|+|\mathcal U|=M$ forces $|\mathcal S|=|\mathcal L|$ and $\mathcal U=\binom{[n]}{k+1}\setminus\mathcal S$.

Consider the inclusion [bipartite graph](../../../../../bipartite-graph.md) between these two middle layers. It is a $(k+1)$-[regular graph](../../../../../regular-graph.md). Since $|\mathcal S|=|\mathcal L|$, all $(k+1)|\mathcal S|$ edges incident to $\mathcal S$ must come from $\mathcal L$; there are no edges from its complement on the lower side into $\mathcal S$. This [bipartite graph](../../../../../bipartite-graph.md) is a [connected graph](../../../../../connected-graph.md): any two $k$-subsets can be joined by single-element exchanges, and each exchange passes through their common $(k+1)$-superset; every upper vertex has a lower neighbour. For $k=0$ it is just one edge. Hence either $\mathcal L=\varnothing$ or $\mathcal L$ is the whole lower layer. We have proved the complete classification:

$$
\boxed{\mathcal A=\binom{[n]}{\lfloor n/2\rfloor}\quad\text{or}\quad\mathcal A=\binom{[n]}{\lceil n/2\rceil}.}
$$

The two possibilities coincide for even $n$; for $n=0$ the unique maximum [antichain](../../../../../antichain.md) is $\{\varnothing\}$.

Finally enumerate the members of the [separating set system](../../../../../separating-set-system.md) as $A_1,\ldots,A_m$ and encode each point $i\in[n]$ by $T_i=\{a\in[m]:i\in A_a\}$. Separation of the ordered pair $(i,j)$ means $T_i\setminus T_j\ne\varnothing$. Applying the hypothesis also to $(j,i)$ shows that the $n$ [sets](../../../../../set-split.md) $T_i$ are distinct and pairwise incomparable. They form an [antichain](../../../../../antichain.md) in $\mathcal P([m])$, so the [Sperner theorem](../../../../../sperner-s-theorem.md) immediately gives

$$
\boxed{n\leq\binom m{\lfloor m/2\rfloor}.}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
