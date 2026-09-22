# Intersection-preserving lexicographic UV-compression

↑ **Parent:** [UV-compression](uv-compression.md)

Let $U,V$ be disjoint, equally sized, nonempty [sets](set-split.md), with $\min U<\min V$. Suppose an [intersecting family](intersecting-family.md) is unchanged by all such [UV-compressions](uv-compression.md) of smaller size. Then its $(U,V)$-[UV-compression](uv-compression.md) is still an [intersecting family](intersecting-family.md). Indeed, a newly moved member $A'=(A\setminus V)\cup U$ can only be disjoint from a retained old member $B$, since two newly moved members share $U$. Here $B\cap U=\varnothing$ and $V'=B\cap V\ne\varnothing$. If $V'=V$, retaining $B$ forces $(B\setminus V)\cup U$ to have been present, contradicting the old [intersection](set-intersection.md) property with $A$. Otherwise choose $U'\subset U$ with $|U'|=|V'|$ and $\min U\in U'$. Stability under the smaller $(U',V')$-[UV-compression](uv-compression.md) forces $(A\setminus V')\cup U'$ to be present; this member is disjoint from $B$, again a contradiction. Repeatedly applying a changing [UV-compression](uv-compression.md) of smallest size terminates, since the sum of [lexicographic order](lexicographic-order.md) positions decreases. A terminal [set family](set-family.md) is a [lexicographic](lexicographic-order.md) initial segment: a missing earlier member $X$ and present later member $Y$ would be moved by $U=X\setminus Y$, $V=Y\setminus X$.

## ↑ Ancestors (9)

1. [UV-compression](uv-compression.md)
2. [Kruskal-Katona theorem](kruskal-katona-theorem.md)
3. [Lower shadow](lower-shadow.md)
4. [Set family shadow](set-family-shadow.md)
5. [Extremal set theory](extremal-set-theory-split.md)
6. [Combinatorics](combinatorics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-14/2/solution.md)
