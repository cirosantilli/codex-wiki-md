<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For an $r$-[uniform set family](../../../../../uniform-set-family.md) $\mathcal F$, its [lower shadow](../../../../../lower-shadow.md) is the [set family](../../../../../set-family.md) of all $(r-1)$-sets contained in a member. Write a positive integer $m$ in its unique [binomial representation](../../../../../combinatorial-number-system.md)

$$
m=\binom{a_r}{r}+\binom{a_{r-1}}{r-1}+\cdots+\binom{a_j}{j},\qquad
a_r>a_{r-1}>\cdots>a_j\geq j\geq1.
$$

The [Kruskal-Katona theorem](../../../../../kruskal-katona-theorem.md) states that

$$
\boxed{|\mathcal F|=m\quad\Longrightarrow\quad
|\partial\mathcal F|\geq\binom{a_r}{r-1}+\binom{a_{r-1}}{r-2}+\cdots+\binom{a_j}{j-1}.}
$$

For $m=0$ the bound is zero. Equality is attained by the first $m$ $r$-sets in [colexicographic order](../../../../../colexicographic-order.md). In that order $A$ precedes $B$ when the largest element of their [symmetric difference](../../../../../symmetric-difference.md) belongs to $B$.

Here is a complete [UV-compression proof of the Kruskal-Katona theorem](../../../../../uv-compression-proof-of-the-kruskal-katona-theorem.md). For disjoint equal-sized [sets](../../../../../set-split.md) $U,V$, put $C(A)=(A\setminus V)\cup U$ when $A$ contains every element of $V$ and no element of $U$, and put $C(A)=A$ otherwise. The [UV-compression](../../../../../uv-compression.md) of a [set family](../../../../../set-family.md) replaces an eligible $A$ only if its image is absent. It preserves [cardinality](../../../../../cardinality.md): a retained collision keeps both the original [set](../../../../../set-split.md) and its already present image.

We first prove the required [Shadow lemma for UV-compressions](../../../../../shadow-lemma-for-uv-compressions.md). Suppose that, for each $x\in U$, a $y\in V$ can be chosen so the [set family](../../../../../set-family.md) is fixed by $C_{U\setminus\{x\},V\setminus\{y\}}$. We claim

$$
\partial C_{U,V}(\mathcal F)\subseteq C_{U,V}(\partial\mathcal F).
$$

Consider a [lower shadow](../../../../../lower-shadow.md) member obtained by deleting $z$ from a moved [set](../../../../../set-split.md) $A'=(A\setminus V)\cup U$. If $z\notin U$, it is the compressed image of $A\setminus\{z\}$, an old [lower shadow](../../../../../lower-shadow.md) member. If $z=x\in U$, the smaller compression of $A$ produces $A'\setminus\{x\}\cup\{y\}$, which is in $\mathcal F$ by the assumed invariance. Thus $A'\setminus\{x\}$ already belongs to the old [lower shadow](../../../../../lower-shadow.md); it is not eligible to move since it lacks $x$.

It remains to consider a [lower shadow](../../../../../lower-shadow.md) member $B$ from a retained original member $A=B\cup\{z\}$. If $B$ is not eligible to move, it stays in the compressed [lower shadow](../../../../../lower-shadow.md). If it is eligible, let $B'=(B\setminus V)\cup U$. When $z\notin U$, retaining the eligible $A$ means its image already belongs to $\mathcal F$, and that image contains $B'$. When $z=x\in U$, the smaller compression of $A$ belongs to $\mathcal F$ and equals $B'\cup\{y\}$. In either case $B'$ is in the old [lower shadow](../../../../../lower-shadow.md) too. Consequently the collision rule retains $B$ as well. This proves the claimed containment in every case. Since compression preserves [cardinality](../../../../../cardinality.md), it cannot increase [lower shadow](../../../../../lower-shadow.md) size.

If $\mathcal F$ is not a [colexicographic initial segment](../../../../../colexicographic-initial-segment.md), an earlier absent [set](../../../../../set-split.md) $A$ and a later present [set](../../../../../set-split.md) $B$ give $U=A\setminus B$, $V=B\setminus A$ with $\max U<\max V$, and a nontrivial [UV-compression](../../../../../uv-compression.md). Choose such a compression with $|U|$ smallest. If $|U|>1$, choose $y\in V\setminus\{\max V\}$. For every $x\in U$, the smaller compression still has its largest differing element on the $V$ side and must fix $\mathcal F$ by minimality. If $|U|=1$, the smaller compression is the identity. Thus the [lower shadow](../../../../../lower-shadow.md) argument applies.

Each nontrivial step strictly decreases the positive integer weight

$$
w(\mathcal F)=\sum_{A\in\mathcal F}\sum_{i\in A}2^i,
$$

because the largest differing coordinate belongs to $V$. Iteration therefore terminates. A terminal [set family](../../../../../set-family.md) is a [colexicographic initial segment](../../../../../colexicographic-initial-segment.md), since an earlier gap and a later member would otherwise provide another nontrivial compression. The final [set family](../../../../../set-family.md) has $m$ members and no larger [lower shadow](../../../../../lower-shadow.md).

To compute its [lower shadow](../../../../../lower-shadow.md), take $a_r$ maximal with $\binom{a_r}{r}\leq m$. All $r$-sets of $[a_r]$ occur first. The next block consists of [sets](../../../../../set-split.md) containing $a_r+1$ whose remaining $(r-1)$-set runs through the initial segment of length $m-\binom{a_r}{r}$. By [Pascal's identity](../../../../../pascal-s-rule.md), the remainder is smaller than $\binom{a_r}{r-1}$, so its next leading top index is strictly less than $a_r$. Repeating gives the stated unique [binomial representation](../../../../../combinatorial-number-system.md). The first block contributes all $\binom{a_r}{r-1}$ $(r-1)$-sets in $[a_r]$ to the [lower shadow](../../../../../lower-shadow.md). Deleting $a_r+1$ from the next block contributes only [sets](../../../../../set-split.md) already counted; deleting another coordinate contributes $a_r+1$ joined to the [lower shadow](../../../../../lower-shadow.md) of the smaller initial segment. This recursive decomposition gives exactly the displayed sum. The base $r=1$ has [lower shadow](../../../../../lower-shadow.md) $\{\varnothing\}$ for every nonempty [set family](../../../../../set-family.md). This completes the proof and the sharpness assertion.

Now let $\mathcal C$ be the [set family](../../../../../set-family.md) of [vertex](../../../../../vertex-graph-theory.md) [sets](../../../../../set-split.md) of the [graph](../../../../../graph-split.md)'s [cliques](../../../../../clique-graph-theory.md) of order four. Its twice-iterated [lower shadow](../../../../../lower-shadow.md) consists of [edges](../../../../../edge-of-a-graph.md) of the [graph](../../../../../graph-split.md). If there were at least sixteen such copies, choose a sixteen-member subfamily. The relevant [binomial representation](../../../../../combinatorial-number-system.md) is

$$
16=\binom64+\binom33.
$$

The proved theorem gives at least $\binom63+\binom32=23$ triples in its first [lower shadow](../../../../../lower-shadow.md). Apply it again to any twenty-three of those triples, using $23=\binom63+\binom32$. Their [edge](../../../../../edge-of-a-graph.md) [lower shadow](../../../../../lower-shadow.md) has at least

$$
\binom62+\binom31=18
$$

members, contradicting the fifteen available [edges](../../../../../edge-of-a-graph.md). Conversely, the [complete graph](../../../../../complete-graph.md) $K_6$ has $\binom62=15$ [edges](../../../../../edge-of-a-graph.md) and $\binom64=15$ copies of $K_4$. Therefore **the maximum number of copies is exactly 15**.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
