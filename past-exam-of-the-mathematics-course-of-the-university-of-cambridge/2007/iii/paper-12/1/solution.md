<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a nonempty $r$-[uniform set family](../../../../../uniform-set-family.md) $\mathcal F$, write its [cardinality](../../../../../cardinality.md) in its unique greedy [binomial representation](../../../../../combinatorial-number-system.md)

$$
|\mathcal F|=\binom{a_r}r+\binom{a_{r-1}}{r-1}+\cdots+\binom{a_s}s,\qquad a_r>a_{r-1}>\cdots>a_s\geq s\geq1.
$$

The [Kruskal-Katona theorem](../../../../../kruskal-katona-theorem.md) gives the exact minimum size of its [lower shadow](../../../../../lower-shadow.md):

$$
\boxed{|\partial\mathcal F|\geq\binom{a_r}{r-1}+\binom{a_{r-1}}{r-2}+\cdots+\binom{a_s}{s-1}.}
$$

Equality is attained by the [colexicographic initial segment](../../../../../colexicographic-initial-segment.md) of the same [cardinality](../../../../../cardinality.md). The empty family has empty shadow. In [colexicographic order](../../../../../colexicographic-order.md), $A$ precedes $B$ exactly when the largest point of $A\mathbin\triangle B$ belongs to $B$. The greedy expansion exists by choosing each top argument as large as possible; [Pascal's identity](../../../../../pascal-s-rule.md) makes the next residual less than $\binom{a_j}{j-1}$, forcing the next top argument below $a_j$. This also proves uniqueness.

Here is a proof by [UV-compression](../../../../../uv-compression.md) of the theorem, including the step that controls the [lower shadow](../../../../../lower-shadow.md). For disjoint nonempty sets $U,V$ of equal size, let $C_{U,V}$ replace a member $A$ containing $V$ and avoiding $U$ by $A'=(A\setminus V)\cup U$ only when $A'$ is absent. Other members stay. This [UV-compression](../../../../../uv-compression.md) preserves [cardinality](../../../../../cardinality.md). Allow only $\max U<\max V$, and at each step choose a changing compression with $|U|=|V|$ as small as possible. Every smaller allowed [UV-compression](../../../../../uv-compression.md) then fixes the current family.

For such a chosen [UV-compression](../../../../../uv-compression.md), we prove

$$
\partial(C_{U,V}\mathcal F)\subseteq C_{U,V}(\partial\mathcal F).
$$

First let $S$ be a new shadow member, not in $\partial\mathcal F$. It has the form $A'\setminus\{x\}$ for a moved member $A$. If $x\in U$, choose $y\in V$ with $y\neq\max V$ when $|V|>1$. The smaller [UV-compression](../../../../../uv-compression.md) with sets $U\setminus\{x\},V\setminus\{y\}$ fixes $\mathcal F$, and therefore its target $S\cup\{y\}$ already belongs to $\mathcal F$. This would put $S$ in the old shadow, a contradiction. For $|V|=1$ the same target is simply $A$, giving the same contradiction without a compression. Hence $x\notin U$. Now $A\setminus\{x\}$ is an old shadow member whose compression target is $S$; since $S$ was absent, it appears in the compressed shadow.

It remains to check that a surviving old shadow member is not removed on the right side. Such a removal could occur only for $S$ containing $V$, avoiding $U$, with $S'=(S\setminus V)\cup U$ absent from the old shadow. A witness $B=S\cup\{x\}$ in the compressed family must be a retained old member, since newly moved members avoid $V$. If $x\notin U$, retention of the eligible member $B$ forces its target $S'\cup\{x\}$ to be in the old family, contrary to the absence of $S'$ from its shadow. If $x\in U$, the smaller fixed compression just used forces $S'\cup\{y\}$ into the old family; for $|U|=1$ this is $B$ itself. Again there is a contradiction. This proves the containment, and hence the chosen compression cannot increase [lower shadow](../../../../../lower-shadow.md) [cardinality](../../../../../cardinality.md).

Each change strictly decreases the integer potential $\sum_{A\in\mathcal F}\sum_{a\in A}2^a$. The procedure therefore terminates. Its terminal family is an initial segment of [colexicographic order](../../../../../colexicographic-order.md): otherwise take an absent earlier set $X$ and a present later set $Y$. The choice $U=X\setminus Y,V=Y\setminus X$ is an allowed changing compression. Thus [UV-compression](../../../../../uv-compression.md) transforms $\mathcal F$ into the [colexicographic initial segment](../../../../../colexicographic-initial-segment.md) of the same size without increasing its [lower shadow](../../../../../lower-shadow.md).

Finally compute that shadow. The first block comprises all $r$-subsets of $[a_r]$ and contributes $\binom{a_r}{r-1}$ shadow members. The next block has maximum point $a_r+1$ and its remaining $(r-1)$ points form a smaller [colexicographic initial segment](../../../../../colexicographic-initial-segment.md). Shadow members omitting $a_r+1$ are already in the first block's shadow; those containing it are counted by the [lower shadow](../../../../../lower-shadow.md) of that smaller initial segment. Recursion through the [binomial representation](../../../../../combinatorial-number-system.md) gives precisely the displayed sum. This completes the proof.

To deduce the [Erdős-Ko-Rado theorem](../../../../../erdos-ko-rado-theorem.md), let $1\leq r\leq n/2$ and let $\mathcal F$ be an [intersecting family](../../../../../intersecting-family.md). Put $k=n-r$ and take the complement family $\mathcal B=\{[n]\setminus A:A\in\mathcal F\}$. Its rank-$r$ [lower shadow](../../../../../lower-shadow.md), obtained by deleting $k-r$ points, is disjoint from $\mathcal F$: membership of $A$ in that shadow would give $A\cap C=\varnothing$ for some $C\in\mathcal F$. If $|\mathcal F|>\binom{n-1}{r-1}=\binom{n-1}k$, iterating the proved [Kruskal-Katona theorem](../../../../../kruskal-katona-theorem.md) gives this shadow at least as many members as the corresponding colex shadow. The colex family contains every $k$-set of $[n-1]$ and a further $k$-set containing $n$. Its rank-$r$ shadow therefore contains every $r$-set of $[n-1]$ and at least one more $r$-set containing $n$. This applies also when $k=r$, with no shadow operation. The two disjoint families would consequently have total size greater than

$$
\binom{n-1}{r-1}+\binom{n-1}r=\binom nr,
$$

a contradiction. Thus $\boxed{|\mathcal F|\leq\binom{n-1}{r-1}}$, attained by all $r$-sets containing a fixed point.

For [nonisomorphic colex shadow minimizers](../../../../../nonisomorphic-colex-shadow-minimizers.md) of rank two, take $n=4$ and $\mathcal F=\{12,23,34,14\}$. Its shadow has four singletons, as does the initial four-set colex segment $\mathcal I=\{12,13,23,14\}$. The first family is the edge set of a [cycle graph](../../../../../cycle-graph.md); its four point degrees are all two. The second has point degrees $3,2,2,1$, so no permutation makes them isomorphic.

For rank three, take $n=5$ and

$$
\mathcal F=\{124,125,134,135,234,235\},\qquad\mathcal I=\{123,124,134,234,125,135\}.
$$

The first [lower shadow](../../../../../lower-shadow.md) comprises the three pairs in $\{1,2,3\}$ and the six pairs joining that set to $\{4,5\}$. The second shadow comprises every pair on $[5]$ except $45$. Both therefore have size nine. Their point-degree multisets are respectively $\{4,4,4,3,3\}$ and $\{5,4,4,3,2\}$, so again the two families are not isomorphic. These examples can be embedded in larger ground sets by adding unused points.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
