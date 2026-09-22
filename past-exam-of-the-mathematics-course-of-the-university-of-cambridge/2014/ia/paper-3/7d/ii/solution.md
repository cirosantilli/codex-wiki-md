<h1 id="7d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Möbius transformations](../../../../../../mobius-transformation.md) are bijections, so they preserve which coordinates of a triple are equal. Conversely, part (i) implies transitivity within each equality pattern. For a pattern with fewer than three distinct entries, extend the chosen distinct points to a triple before applying part (i); this works also for $p=2$, when the [projective line](../../../../../../projective-line.md) has exactly three points. There are therefore five [orbits of a group action](../../../../../../orbit-of-a-group-action.md).

We first count $|GL_2(\mathbb F_p)|$. Its first column can be any nonzero [vector](../../../../../../vector.md), giving $p^2-1$ choices. The second must be outside the first column's one-dimensional span, giving $p^2-p$ choices. Hence

$$
|G|=(p^2-1)(p^2-p)=p(p-1)^2(p+1).
$$

For the all-equal pattern take $(\infty,\infty,\infty)$. Its [stabilizer subgroup](../../../../../../stabilizer-subgroup.md) consists of upper triangular [matrices](../../../../../../matrix.md)

$$
\begin{pmatrix}a&b\\0&d\end{pmatrix},\qquad a,d\ne0,
$$

of order $p(p-1)^2$. Its [group orbit](../../../../../../orbit-of-a-group-action.md) has order $p+1$.

The three exactly-two-equal patterns have representatives $(\infty,\infty,0)$, $(\infty,0,\infty)$ and $(0,\infty,\infty)$. Each [stabilizer subgroup](../../../../../../stabilizer-subgroup.md) fixes $0$ and $\infty$ individually, so it is the diagonal [subgroup](../../../../../../subgroup.md) of order $(p-1)^2$. Each [group orbit](../../../../../../orbit-of-a-group-action.md) has order $p(p+1)$; their repeated-coordinate positions keep these three orbits distinct.

For the all-distinct pattern use $(0,1,\infty)$. Its [stabilizer subgroup](../../../../../../stabilizer-subgroup.md) is the scalar [subgroup](../../../../../../subgroup.md) of order $p-1$, and the [group orbit](../../../../../../orbit-of-a-group-action.md) has order $(p+1)p(p-1)$. Stabilizers of arbitrary triples are conjugates of the displayed representative stabilizers. In summary the [equality-pattern orbits of projective triples](../../../../../../equality-pattern-orbits-of-projective-triples.md) have

$$
\boxed{\begin{array}{c|c|c}
\text{pattern}&\text{orbit size}&\text{stabilizer order}\\\hline
\text{all equal}&p+1&p(p-1)^2\\
\text{each two-equal pattern}&p(p+1)&(p-1)^2\\
\text{all distinct}&p(p+1)(p-1)&p-1
\end{array}}
$$

The sizes add to $(p+1)^3$, and each orbit size times its stabilizer order is $|G|$, as in the [orbit-stabilizer theorem](../../../../../../orbit-stabilizer-theorem.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [7D](../../7d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
