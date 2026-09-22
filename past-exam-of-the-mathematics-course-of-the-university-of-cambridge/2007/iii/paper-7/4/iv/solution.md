<h1 id="4/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

A [Steiner system](../../../../../../steiner-system.md) $S(5,6,12)$ consists of 12 points and a collection of six-element blocks such that every five-element subset lies in exactly one block. The blocks are often called hexads. Necessarily their number is $\binom{12}{5}/\binom65=132$. We give the [synthematic construction of the small Witt design](../../../../../../synthematic-construction-of-the-small-witt-design.md) explicitly and prove this defining property.

Write $X=\{1,\ldots,6\}$ and $Y=\{T_1,\ldots,T_6\}$. For an unordered pair $P=\{T_i,T_j\}\subset Y$, let $S(P)$ denote the unique [syntheme](../../../../../../syntheme.md) shared by its two [synthematic totals](../../../../../../total-of-synthemes.md). A [duad](../../../../../../duad.md) $D\subset X$ belongs to three [synthemes](../../../../../../syntheme.md). The corresponding three pairs $P$ partition $Y$: every [synthematic total](../../../../../../total-of-synthemes.md) contains $D$ in exactly one of its [synthemes](../../../../../../syntheme.md), and each [syntheme](../../../../../../syntheme.md) lies in exactly two [synthematic totals](../../../../../../total-of-synthemes.md). Thus the incidence $D\in S(P)$ gives a perfect matching of the six [synthematic totals](../../../../../../total-of-synthemes.md) for each [duad](../../../../../../duad.md).

To describe the blocks with three points in each half, take an unordered partition $X=A\sqcup A^c$ into triples. A [syntheme](../../../../../../syntheme.md) is cross if each of its three [duads](../../../../../../duad.md) joins $A$ to $A^c$. Form a graph on $Y$ by declaring $P$ an edge exactly when $S(P)$ is cross. This graph is the union of two disjoint triangles. Indeed a [synthematic total](../../../../../../total-of-synthemes.md) partitions the nine cross [duads](../../../../../../duad.md); every [syntheme](../../../../../../syntheme.md) has either one or three cross [duads](../../../../../../duad.md), so if $k$ of its five [synthemes](../../../../../../syntheme.md) are cross, then $3k+(5-k)=9$, giving $k=2$. Each vertex therefore has degree two. The stronger assertion about its components follows directly for $A=\{1,2,3\}$, when the two triangles are

$$
\{T_1,T_4,T_5\}\quad\text{and}\quad\{T_2,T_3,T_6\};
$$

any other triple partition is obtained by relabelling $X$, which also permutes the [synthematic totals](../../../../../../total-of-synthemes.md). Denote the two components by $B,B^c$.

The complete block collection is given by the following three rules:

- Include $X$ and $Y$.
- For each $P\subset Y$ of size two and each [duad](../../../../../../duad.md) $D\in S(P)$, include $D\cup(Y\setminus P)$ and its complement $(X\setminus D)\cup P$.
- For each unordered triple partition $A\sqcup A^c$ and its two components $B,B^c$, include $A\cup B$, $A\cup B^c$, $A^c\cup B$, and $A^c\cup B^c$.

There are $2+15\cdot3\cdot2+10\cdot4=132$ distinct blocks. The first two rules have different intersection sizes with $X$ from the third; within the third, a block determines its triple $A$ and its component. We next verify the [Steiner system](../../../../../../steiner-system.md) property, rather than relying solely on this count.

We need one further consequence of the triangle construction. The three [synthemes](../../../../../../syntheme.md) attached to the three pairs within $B$ are pairwise disjoint, since any two belong to their common [synthematic total](../../../../../../total-of-synthemes.md), and together they are all nine cross [duads](../../../../../../duad.md) of the [complete bipartite graph](../../../../../../complete-bipartite-graph.md) between $A$ and $A^c$. Thus $B$ determines the unordered partition $A\sqcup A^c$ uniquely: it is the bipartition of this connected graph. There are 10 such partitions, each giving two different components, hence 20 different triples in $Y$. Since $\binom63=20$, **each triple in $Y$ corresponds to exactly one triple partition of $X$**. The same reasoning applies to $B^c$.

Let $F$ be any five-point set and put $r=|F\cap X|$. If $r=5$, only $X$ can contain it; if $r=0$, only $Y$ can contain it, because no other block has five points in either half.

If $r=4$, set $D=X\setminus F$ and write $F\cap Y=\{T\}$. The three pairs attached to $D$ partition $Y$, so exactly one contains $T$; its block $(X\setminus D)\cup P$ is the unique block through $F$. If $r=1$, put $P=Y\setminus F$ and write $F\cap X=\{x\}$. The three [duads](../../../../../../duad.md) of $S(P)$ partition $X$, so exactly one contains $x$; this gives the unique block $D\cup(Y\setminus P)$.

If $r=3$, write $A=F\cap X$ and $P=F\cap Y$. A [syntheme](../../../../../../syntheme.md) has either one or three [duads](../../../../../../duad.md) crossing $A\sqcup A^c$. In the one-cross case, $S(P)$ has exactly one [duad](../../../../../../duad.md) $D$ internal to $A^c$, and the unique block is $(X\setminus D)\cup P$. No block with three points in each half is possible, since $P$ is then not an edge of either triangle. In the three-cross case, $P$ is an edge of exactly one triangle $B$, giving the unique block $A\cup B$; no [duad](../../../../../../duad.md) of $S(P)$ is internal to $A^c$, so a block with four points in $X$ is impossible.

Finally let $r=2$, write $D=F\cap X$ and $B=F\cap Y$, and use the uniquely associated partition $X=A\sqcup A^c$ just proved. If $D$ crosses this partition, the three [synthemes](../../../../../../syntheme.md) belonging to the pairs inside $B$ contain each cross [duad](../../../../../../duad.md) exactly once. Thus the matching of $Y$ attached to $D$ has exactly one pair internal to $B$. It has exactly one pair $P$ internal to $B^c$ as well, since a matching must leave equal numbers of vertices in the two halves for cross pairs. The unique block containing $F$ is then $D\cup(Y\setminus P)$; $D$ is not contained in either $A$ or $A^c$, so no block of the third rule applies. If $D$ is internal to $A$ or $A^c$, none of its attached pairs lies inside $B$ or $B^c$, since the [synthemes](../../../../../../syntheme.md) attached to these internal pairs are cross. Thus the second rule gives no block. The third rule gives exactly one, namely $A\cup B$ or $A^c\cup B$, according to which part contains $D$.

All possibilities have now been exhausted, proving

$$
\boxed{\text{These 132 hexads form an }S(5,6,12)\text{ on }X\sqcup Y.}
$$

This is the [small Witt design](../../../../../../small-witt-design.md); the construction uses only [duads](../../../../../../duad.md), [synthemes](../../../../../../syntheme.md), their [synthematic totals](../../../../../../total-of-synthemes.md), and the induced action on those [synthematic totals](../../../../../../total-of-synthemes.md).

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [4](../../4.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
