<h1 id="17g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $B=\{b_1,b_2,b_3\}$ be a blue triangle and $Y=\{y_1,y_2,y_3\}$ a vertex-disjoint yellow triangle. If some $b_i$ has two yellow neighbours in $Y$, those three vertices form a yellow triangle meeting $B$. Otherwise every $b_i$ has at least two blue neighbours in $Y$, giving at least six blue cross-edges. Some $y_j$ then has two blue neighbours in $B$, and these form a blue triangle meeting $Y$. This proves the overlap assertion.

The [triangle-packing Ramsey number](../../../../../../triangle-packing-ramsey-number.md) is

$$
R(tK_3,tK_3)=5t\qquad(t\geq2).
$$

For completeness, its induction starts from the stated $K_{10}$ result. At each step, remove two disjoint monochromatic triangles supplied on ten currently unused vertices. If their colour disagrees with the packing already constructed, apply the overlap assertion to an oppositely coloured pair; replacing that pair by the overlapping pair is the augmenting move that shifts the boundary between the two packings. Repeating the move either adds a triangle to the existing colour or converts all pairs needed for the opposite-colour packing. Thus $K_{5t}$ contains $t$ pairwise vertex-disjoint monochromatic triangles of one colour.

The bound is sharp. For $K_{5t-1}$, split the vertices into $A,B_1,B_2$ with

$$
|A|=3t-1,
\qquad |B_1|=1,
\qquad |B_2|=2t-1.
$$

Colour edges inside $A$ and between $B_1$ and $B_2$ yellow; colour all edges from $A$ to $B_1\cup B_2$ and all edges within each $B_i$ blue. Every yellow triangle lies wholly in $A$, so there are at most $t-1$ disjoint yellow triangles. Every blue triangle uses at least two vertices of $B_1\cup B_2$, and $t$ such triangles would require a blue perfect matching on those $2t$ vertices, impossible because the isolated one-vertex blue component $B_1$ and the odd component $B_2$ have no such matching. Hence there is no $t$-triangle packing of either colour for any $t\geq2$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [17G](../../17g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
