<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $n=4$, the lower bound is four pairs. On $X=\{1,2,3,4\}$ use

$$
(A_1,B_1)=(\{1,2\},\{3,4\}),\quad
(A_2,B_2)=(\{1\},\{2\}),\quad
(A_3,B_3)=(\{3\},\{4\}),\quad
(A_4,B_4)=(\varnothing,\varnothing).
$$

The first pair separates points in different halves, and the next two separate points within each half. The four pairs are distinct and have total incidence $4+2+2+0=8=(1/2)\cdot4\cdot4$. They are therefore a valid [separating family of disjoint set pairs](../../../../../../separating-family-of-disjoint-set-pairs.md) attaining the bound.

For $n=8$, label points by triples $(u,v,w)\in\{0,1\}^3$. The following six pairs attain the bound of six. Coordinates not mentioned in a row are unrestricted:

$$
\begin{array}{c|c|c|c}
i&A_i&B_i&|A_i|+|B_i|\\\hline
1&u=0&u=1&8\\
2&u=0,\ v=0&u=0,\ v=1&4\\
3&u=1,\ v=0&u=1,\ v=1&4\\
4&u=0,\ w=0&u=0,\ w=1&4\\
5&u=1,\ v=0,\ w=0&u=1,\ v=0,\ w=1&2\\
6&u=1,\ v=1,\ w=0&u=1,\ v=1,\ w=1&2
\end{array}
$$

If two triples first differ in $u$, row 1 separates them. If they agree in $u$ and differ in $v$, row 2 or 3 does. If they agree in both and differ in $w$, row 4, 5, or 6 does. The total incidence is $24=(1/2)\cdot6\cdot8$, and each point belongs to exactly three pairs. Thus

$$
\boxed{\text{As written, the bound is sharp for both }n=4\text{ and }n=8.}
$$

The empty fourth pair matters for $n=4$. The original PDF requires disjoint subsets but does not require either side to be nonempty, so the construction is permitted. Under the additional convention that both sides of every pair must be nonempty, the $n=4$ answer would be no: four pairs of total incidence at most eight would each have two singleton sides and could separate at most four of the six unordered pairs of points. The $n=8$ construction already has both sides nonempty.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 109](../../../paper-109-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
