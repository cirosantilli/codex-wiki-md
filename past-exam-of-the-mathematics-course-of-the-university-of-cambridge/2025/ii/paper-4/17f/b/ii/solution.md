<h1 id="17f/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Part (i) gives $R(K_{1,t})\leq2t$ for every $t$.

Suppose first that $t$ is odd. On $2t-1$ vertices, take a red $(t-1)$-regular graph; for example, label the vertices cyclically and join each vertex to the $(t-1)/2$ nearest vertices in each direction. Its blue complement is also $(t-1)$-regular. Neither colour contains a vertex of degree $t$, so there is no monochromatic $K_{1,t}$. Therefore

$$
R(K_{1,t})=2t
\qquad(t\text{ odd}).
$$

Now let $t$ be even. If a colouring of $K_{2t-1}$ had no monochromatic $K_{1,t}$, every vertex would have red and blue degree at most $t-1$. Since the two degrees sum to $2t-2$, each would equal $t-1$. The red graph would then be $(t-1)$-regular on $2t-1$ vertices, impossible because both numbers are odd and the sum of degrees must be even. Hence $R(K_{1,t})\leq2t-1$.

For the matching lower bound, colour a copy of $K_{t-1,t-1}$ red on $2t-2$ vertices and colour all remaining edges blue. Red degree is $t-1$ and the blue graph is two disjoint copies of $K_{t-1}$, of degree $t-2$. Again neither colour contains $K_{1,t}$. Thus the [Ramsey number of a star](../../../../../../../ramsey-number-of-a-star.md) is

$$
\boxed{R(K_{1,t})=
\begin{cases}
2t,&t\text{ odd},\\
2t-1,&t\text{ even}.
\end{cases}}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [17F](../../../17f.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
