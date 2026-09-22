<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $A=g_1$, $B=g_2$ and $C=AB$. Direct multiplication gives

$$
A^2=B^2=I_2,\qquad BA=-AB,\qquad
C=\begin{pmatrix}0&1\\-1&0\end{pmatrix},\qquad C^2=-I_2.
$$

The relation $BA=-AB$ moves all occurrences of $A$ to the left of all occurrences of $B$. Removing even powers reduces every product of the generators to $\pm A^aB^b$ with $a,b\in\{0,1\}$. The resulting eight [matrices](../../../../matrix.md) are distinct, so

$$
\boxed{G=\{\pm I_2,\ \pm A,\ \pm B,\ \pm C\},\qquad |G|=8.}
$$

Explicitly, the four pairs are

$$
\pm\begin{pmatrix}1&0\\0&1\end{pmatrix},\quad
\pm\begin{pmatrix}1&0\\0&-1\end{pmatrix},\quad
\pm\begin{pmatrix}0&1\\1&0\end{pmatrix},\quad
\pm\begin{pmatrix}0&1\\-1&0\end{pmatrix}.
$$

Since $AB=-BA$ and $AB\ne0$, the [group](../../../../group-split.md) is noncommutative. More precisely, $C$ has order four, $A$ has order two and $ACA=C^{-1}$, identifying $G$ with the [dihedral group](../../../../dihedral-group.md) of a square. This fixes the convention unambiguously: it is the [dihedral group](../../../../dihedral-group.md) of [group order](../../../../order-of-a-finite-group.md) eight, irrespective of whether it is denoted $D_4$ or $D_8$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

## ← Incoming links (1)

- [Solution](../d/solution.md)
