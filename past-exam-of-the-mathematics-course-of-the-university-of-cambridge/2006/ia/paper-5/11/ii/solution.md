<h1 id="11/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

If $T$ is [transitive](../../../../../../transitive-relation.md), then $T\circ T\subseteq T$. Since $S,R\subseteq T$, monotonicity of [composition of relations](../../../../../../composition-of-relations.md) gives

$$
S\circ R\subseteq T\circ T\subseteq T,
$$

which is condition (iii).

Conversely, condition (iii), associativity of [composition of relations](../../../../../../composition-of-relations.md), and the identities $R\circ R=R$, $S\circ S=S$ give

$$
\begin{aligned}
T\circ T&=R\circ S\circ R\circ S\\
&\subseteq R\circ R\circ S\circ S
=R\circ S=T.
\end{aligned}
$$

For a direct chain description, start with $xRaSbRcSz$. Replace its middle $aSbRc$ by $aRdSc$ using condition (iii), then use [transitivity](../../../../../../transitive-relation.md) inside $R$ and $S$ to obtain $xRdSz$. Hence $T$ is [transitive](../../../../../../transitive-relation.md). **Conditions (ii) and (iii) are equivalent.**

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [11](../../11.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Ia](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
