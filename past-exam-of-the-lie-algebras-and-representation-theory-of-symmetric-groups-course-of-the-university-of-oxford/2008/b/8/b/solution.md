<h1 id="b/8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose the two [standard tableaux](../../../../../standard-young-tableau.md)

$$
t_1=\begin{array}{ll}1&2\\3&4\end{array},\qquad t_2=\begin{array}{ll}1&3\\2&4\end{array},
$$

and use their [polytabloids](../../../../../polytabloid.md) $e_1,e_2$, with column-vector coordinates. Writing $[ab\mid cd]$ for the [tabloid](../../../../../tabloid.md) with those two row sets gives

$$
\begin{aligned}
e_1&=[12\mid34]-[23\mid14]-[14\mid23]+[34\mid12],\\
e_2&=[13\mid24]-[23\mid14]-[14\mid23]+[24\mid13].
\end{aligned}
$$

The coefficients at $[12\mid34]$ and $[13\mid24]$ prove independence over every [field](../../../../../field.md). Applying the generators directly gives

$$
(12)e_1=e_1-e_2,\quad(12)e_2=-e_2,\qquad(23)e_1=e_2,\quad(23)e_2=e_1,
$$

and $(34)$ acts in the same way as $(12)$. Their span is invariant under the generators, contains $e_1$, and contains its whole orbit, hence is the [Specht module](../../../../../specht-module.md). Thus it is a [basis](../../../../../basis.md) without needing a characteristic-zero argument. The [matrices](../../../../../matrix.md) are

$$
\boxed{\rho(12)=\rho(34)=\begin{pmatrix}1&0\\-1&-1\end{pmatrix},\qquad\rho(23)=\begin{pmatrix}0&1\\1&0\end{pmatrix}.}
$$

These integral [matrices](../../../../../matrix.md) may be reduced in the chosen characteristic.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [8](../../8.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../split.md)
6. [Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../../lie-algebras-and-representation-theory-of-symmetric-groups-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
