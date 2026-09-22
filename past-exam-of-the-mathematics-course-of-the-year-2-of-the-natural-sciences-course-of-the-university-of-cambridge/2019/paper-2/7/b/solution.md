<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Label the equal [masses](../../../../../mass.md) $1,2$ and the mass $2m$ by $3$, in cyclic order. Let their equilibrium angles be $0,2\pi/3,4\pi/3$, with angular displacements $q_1,q_2,q_3$. Because the hoop has unit radius, its three arc lengths are

$$
\ell_1=\frac{2\pi}{3}+q_2-q_1,\quad
\ell_2=\frac{2\pi}{3}+q_3-q_2,\quad
\ell_3=\frac{2\pi}{3}+q_1-q_3.
$$

The [springs](../../../../../spring.md) themselves are constrained to the hoop, so these are arc lengths. If their common natural length is $\ell_0$, [Hooke's law](../../../../../hooke-s-law.md) gives $V=\frac k2\sum_i(\ell_i-\ell_0)^2$. Since the arc lengths have fixed sum $2\pi$, all terms linear in the $q_i$ cancel. Dropping the constant,

$$
\boxed{T=\frac m2(\dot q_1^2+\dot q_2^2+2\dot q_3^2),\qquad
V-V_0=\frac k2\big[(q_2-q_1)^2+(q_3-q_2)^2+(q_1-q_3)^2\big]}.
$$

Thus the unspecified common natural length does not affect the motion. The mass and restoring matrices in the [generalized eigenvalue problem](../../../../../generalized-eigenvalue-problem.md) are

$$
M=m\begin{pmatrix}1&0&0\\0&1&0\\0&0&2\end{pmatrix},\qquad
K=k\begin{pmatrix}2&-1&-1\\-1&2&-1\\-1&-1&2\end{pmatrix}.
$$

Exchange of the two equal [masses](../../../../../mass.md) separates symmetric and antisymmetric [normal modes](../../../../../normal-mode.md). Direct multiplication gives the complete set

$$
\boxed{\begin{array}{c|c}
\text{mode shape}&\omega^2\\ \hline
(1,1,1)&0\\
(1,-1,0)&3k/m\\
(1,1,-1)&2k/m
\end{array}}.
$$

The first is rigid [rotation](../../../../../rotation-mathematics.md) of all three beads: every arc length stays fixed, giving a [zero mode](../../../../../zero-mode.md). In the second, the equal [masses](../../../../../mass.md) move oppositely while the heavy bead stays fixed; the net force on that bead cancels. In the third, the equal [masses](../../../../../mass.md) move together and the heavy bead moves oppositely with equal angular amplitude. Both nonzero [normal modes](../../../../../normal-mode.md) have zero total [angular momentum](../../../../../angular-momentum.md). These are the [normal modes of three beads connected by springs on a circular hoop](../../../../../normal-modes-of-three-beads-connected-by-springs-on-a-circular-hoop.md) with $M=2m$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [7](../../7.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
