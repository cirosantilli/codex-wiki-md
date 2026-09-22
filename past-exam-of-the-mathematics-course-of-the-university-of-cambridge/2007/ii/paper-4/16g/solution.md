<h1 id="16g/solution">Solution</h1>

↑ **Parent:** [16G](../16g.md)

A binary relation $R$ on a set is a [well-founded relation](../../../../../well-founded-relation.md) if every nonempty subset has an $R$-minimal member, that is, a member with no predecessor inside that subset. Here write $xRy$ when $x\in f(y)$.

Suppose $R$ is well-founded and fix any $g:\mathcal P(b)\to b$. Call a partial function $h:D\to b$ consistent if $D$ is downward closed under $R$ and $h(y)=g(\{h(x):x\in f(y)\})$ for $y\in D$. Two consistent partial functions agree on their common domain: otherwise the set of points where they disagree has a minimal member, all of whose predecessors are in both domains and agree, so applying $g$ gives agreement at that member as well, a contradiction. Thus the union of all consistent partial functions is itself a function $h:D\to b$, on a downward-closed domain, and remains consistent. This union is a set, because every such graph is a subset of $a\times b$.

If $D\ne a$, choose a minimal member $y$ of $a\setminus D$. All predecessors of $y$ lie in $D$, so extend $h$ to $y$ by the prescribed value $g(\{h(x):x\in f(y)\})$. The enlarged domain remains downward closed and consistent, contradicting the union's maximality. Hence $D=a$. The same minimal-disagreement argument proves uniqueness. This establishes the required recursion directly, without invoking an unproved [well-founded recursion](../../../../../well-founded-recursion.md) theorem.

Conversely, if $R$ is not well-founded, choose a nonempty $S\subset a$ such that each $y\in S$ has a predecessor in $S$. Let $T$ be all points reachable from $S$ by a finite chain of upward $R$ steps, including $S$. Then

$$
y\in T\quad\Longleftrightarrow\quad f(y)\cap T\ne\varnothing.
$$

For a point reached by a nonempty chain, its preceding point is in $T$; for a point of $S$, use its predecessor in $S$. The converse follows by appending the final step to a chain. Choose $b=\{0,1\}$ and $g(B)=1$ if $1\in B$, zero otherwise. Both $h_0\equiv0$ and $h_1=\mathbf1_T$ satisfy the required recursion, and they differ because $S\ne\varnothing$. This contradicts recursiveness. Therefore **$f$ is recursive exactly when its predecessor relation is well-founded**, the characterization of a [recursive powerset mapping](../../../../../recursive-powerset-mapping.md).

## ↑ Ancestors (10)

1. [16G](../16g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
