<h1 id="17f/solution">Solution</h1>

↑ **Parent:** [17F](../17f.md)

Work with finite graphs, as in the usual matching theorem. Hall's condition is $|N(A)|\ge|A|$ for every $A\subseteq X$. It is necessary because a matching injects $A$ into its neighbours.

For sufficiency, induct on $|X|$. If a nonempty proper subset $A$ has $|N(A)|=|A|$, induction matches $A$ to $N(A)$. For $B\subseteq X\setminus A$, Hall's inequality for $A\cup B$ gives $|N(B)\setminus N(A)|\ge|B|$, so induction matches the complement to unused neighbours. Combining the matchings finishes this case. Otherwise every nonempty proper $A$ has $|N(A)|\ge|A|+1$. Choose an edge $xy$, delete its endpoints, and observe that every subset of the remaining $X$ still has at least its own number of neighbours. Induction matches the remainder, and adjoining $xy$ finishes. The one-vertex case and the empty case are immediate.

For $0\le d\le|X|$, the defect version is

$$
\boxed{G\text{ has at least }|X|-d\text{ independent edges}\iff |N(A)|\ge|A|-d\text{ for all }A\subseteq X.}
$$

Necessity follows because at most $d$ vertices of $X$ can be unmatched. For sufficiency add $d$ new vertices to $Y$, each joined to every vertex of $X$. The displayed inequality makes Hall's condition hold in the enlarged graph. Its full matching uses at most $d$ new vertices, giving the required original edges.

To prove the matching-cover equality, let $M$ be a maximum matching and $U$ its unmatched vertices in $X$. Follow alternating paths from $U$, using nonmatching edges from $X$ to $Y$ and matching edges back. Let $Z_X,Z_Y$ be the [reachable sets](../../../../../reachable-set.md). No reachable $Y$ is unmatched, since that would give an [augmenting path](../../../../../augmenting-path.md) and a larger matching. Matching edges give a bijection $Z_Y\leftrightarrow Z_X\setminus U$. The set $C=(X\setminus Z_X)\cup Z_Y$ covers every edge: an edge from a reachable $X$ to an unreachable $Y$ cannot be a nonmatching edge, and its matching edge, if present, is already reachable. Its size is

$$
|C|=|X|-|Z_X|+|Z_Y|=|X|-|U|=|M|.
$$

Every [vertex cover](../../../../../vertex-cover.md) has at least $|M|$ vertices, because the matching edges are disjoint. Therefore **maximum matching size equals minimum vertex-cover size**, as required.

## ↑ Ancestors (10)

1. [17F](../17f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
