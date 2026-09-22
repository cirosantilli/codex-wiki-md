<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the two [Pauli matrices](../../../../pauli-matrices.md) as

$$
A=\begin{pmatrix}0&1\\1&0\end{pmatrix},\qquad
B=\begin{pmatrix}1&0\\0&-1\end{pmatrix},\qquad
C=AB=\begin{pmatrix}0&-1\\1&0\end{pmatrix}.
$$

They satisfy $A^2=B^2=I$, $BA=-AB$ and $C^2=-I$. Moving every $A$ to the left of every $B$ reduces each word to one of eight distinct [matrices](../../../../matrix.md). Consequently

$$
\boxed{G=\{I,-I,A,-A,B,-B,C,-C\},\qquad |G|=8.}
$$

Taking $r=C$, $s=A$ gives $r^4=s^2=I$ and $srs=r^{-1}$, identifying the [group](../../../../group-split.md) with the [dihedral group](../../../../dihedral-group.md) of a square.

The elements $\pm I$ are central. Conjugating $A$ by $B$ changes its sign, and similarly for $B$ and $C$. No conjugation mixes these pairs: modulo the central [subgroup](../../../../subgroup.md) $\{\pm I\}$ the [quotient group](../../../../quotient-group.md) is the [Klein four-group](../../../../klein-four-group.md) and hence [Abelian](../../../../abelian-group.md). Thus the [conjugacy classes](../../../../conjugacy-class.md) are precisely

$$
\boxed{\{I\},\quad\{-I\},\quad\{A,-A\},\quad\{B,-B\},\quad\{C,-C\}.}
$$

There are five complex [irreducible representations](../../../../irreducible-representation.md), one for each [conjugacy class](../../../../conjugacy-class.md). In a [one-dimensional representation](../../../../one-dimensional-representation.md), the images of $A,B$ are signs $s,t\in\{1,-1\}$. Since they commute, $-I$ maps to $1$, and all four choices of $s,t$ satisfy the relations. These are four inequivalent [one-dimensional representations](../../../../one-dimensional-representation.md). The [sum of squares of irreducible representation dimensions](../../../../sum-of-squares-of-irreducible-representation-dimensions.md) leaves $8-4=4$ for the fifth, so the [dimensions](../../../../dimension-vector-space.md) are

$$
\boxed{1,1,1,1,2.}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2021](../../../2021-split.md)
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

- [Solution](../c/solution.md)
