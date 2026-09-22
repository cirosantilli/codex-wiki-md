<h1 id="10/solution">Solution</h1>

↑ **Parent:** [10](../10.md)

Write the [symmetry group of a square](../../../../symmetry-group-of-a-square.md) as $D_4=\langle r,s\mid r^4=s^2=e,\ srs=r^{-1}\rangle$, with $r$ a counterclockwise quarter-turn and $s$ [reflection](../../../../reflection-mathematics.md) across the horizontal axis. The [conjugacy classes of the symmetry group of a square](../../../../conjugacy-classes-of-the-symmetry-group-of-a-square.md) are

$$
\boxed{\{e\},\qquad\{r^2\},\qquad\{r,r^3\},\qquad\{s,r^2s\},\qquad\{rs,r^3s\}.}
$$

Here $r^2$ is the half-turn and $r^3$ the clockwise quarter-turn. The two members of the fourth class reflect across the horizontal and vertical axes. Those of the fifth reflect across $y=x$ and $y=-x$. The identity and half-turn are [central elements](../../../../central-element-of-a-group.md), giving singleton classes. The relations $srs=r^3$, $rsr^{-1}=r^2s$, and $r(rs)r^{-1}=r^3s$ show that each displayed pair consists of conjugate elements. More generally, conjugating $r^ks$ by $r$ changes $k$ to $k+2$, and conjugating by $s$ changes $k$ to $-k$; parity is preserved, so the two [reflection](../../../../reflection-mathematics.md) pairs cannot merge.

In a [one-dimensional representation](../../../../one-dimensional-representation.md), the relation $srs=r^{-1}$ forces the image of $r$ to equal its inverse. Thus $r$ and $s$ can be assigned independent signs $\alpha,\beta\in\{1,-1\}$. These four choices give four [irreducible characters](../../../../irreducible-character.md). The ordinary two-dimensional action on the plane gives one more [character](../../../../character-of-a-representation.md): a [rotation](../../../../rotation-mathematics.md) through $\theta$ has [trace](../../../../matrix-trace.md) $2\cos\theta$, and a [reflection](../../../../reflection-mathematics.md) has [trace](../../../../matrix-trace.md) zero. Therefore the [character table of the symmetry group of a square](../../../../character-table-of-the-symmetry-group-of-a-square.md) is

$$
\begin{array}{c|rrrrr}
&e&r^2&\{r,r^3\}&\{s,r^2s\}&\{rs,r^3s\}\\\hline
\text{class size}&1&1&2&2&2\\\hline
A_1&1&1&1&1&1\\A_2&1&1&1&-1&-1\\B_1&1&1&-1&1&-1\\B_2&1&1&-1&-1&1\\E&2&-2&0&0&0
\end{array}.
$$

For instance the last row has squared character norm $(4+4)/8=1$, so the planar [representation](../../../../group-representation.md) is [irreducible](../../../../irreducible-representation.md); its inner product with each one-dimensional row is zero. All five rows obey [character orthogonality](../../../../character-orthogonality.md). Their squared dimensions sum to $1+1+1+1+4=8$, so they exhaust the [irreducible representations](../../../../irreducible-representation.md) of this order-eight [group](../../../../group-split.md).

## ↑ Ancestors (12)

1. [10](../10.md)
2. [Paper 2](../../paper-2-split.md)
3. [2003](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
