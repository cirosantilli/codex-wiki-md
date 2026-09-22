<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Choose one representative from $A$ above each point of $\pi(A)$ and collect them in $X$. Part (c) gives $|X|\leq K^{O(1)}$. If $a\in A$ has the same image as $x\in X$, then $x^{-1}a\in A^2\cap N$, so

$$
A\subseteq X(A^2\cap N).
$$

This is the required covering of $A$ by at most $K^{O(1)}$ left cosets of the abelian translation subgroup $N$.

The set $B=A^2\cap N$ is a $K^{O(1)}$-approximate group by the [intersection of an approximate group power with a subgroup](../../../../../../intersection-of-an-approximate-group-power-with-a-subgroup.md). Apply the [Freiman-Green-Ruzsa theorem](../../../../../../freiman-ruzsa-theorem.md) inside $N\cong(\mathbb C,+)$. Because the additive group of the [complex numbers](../../../../../../complex-number.md) is a [torsion-free group](../../../../../../torsion-free-group.md), the finite subgroup part is trivial, so there is an [abelian progression](../../../../../../abelian-progression.md) $P$ with

$$
B\subseteq P,\qquad
\operatorname{rank}P\leq K^{O(1)},\qquad
|P|\leq\exp(K^{O(1)})|B|.
$$

Since $|B|\leq|A^2|\leq K|A|$, enlarging the implicit constant gives

$$
\boxed{A\subseteq XP,\qquad |X|\leq K^{O(1)},\qquad
\operatorname{rank}P\leq K^{O(1)},\qquad
|P|\leq\exp(K^{O(1)})|A|.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 149](../../../paper-149-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
