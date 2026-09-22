<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $C=V(P)$, where $P\in\mathbb C[x,y,z]$ is a [squarefree polynomial](../../../../square-free-polynomial.md) and a [homogeneous polynomial](../../../../homogeneous-polynomial.md) of degree $d$. A [projective point](../../../../projective-point.md) $p\in C$ is a [singular point](../../../../singular-point-of-an-algebraic-variety.md) precisely when

$$
P_x(p)=P_y(p)=P_z(p)=0.
$$

If $p=[p_0:p_1:p_2]$ is a [nonsingular point of an algebraic curve](../../../../nonsingular-point-of-an-algebraic-curve.md), its [projective tangent line](../../../../tangent-line-to-a-projective-plane-curve.md) is

$$
\boxed{T_pC=\{[x:y:z]:P_x(p)x+P_y(p)y+P_z(p)z=0\}.}
$$

The coefficients are not all zero, and the [Euler theorem for homogeneous functions](../../../../euler-theorem-for-homogeneous-functions.md) gives $p_0P_x(p)+p_1P_y(p)+p_2P_z(p)=dP(p)=0$, so the line passes through $p$. Changing the representative of the [projective point](../../../../projective-point.md) only rescales the equation.

The strong form of [Bézout's theorem](../../../../bezout-s-theorem.md) says that two [projective plane curves](../../../../projective-plane-curve.md) $C,D$ of degrees $d,e$, with no common [irreducible component](../../../../irreducible-component.md), have finitely many intersections and

$$
\boxed{\sum_{p\in C\cap D}I_p(C,D)=de.}
$$

Each [intersection multiplicity](../../../../intersection-multiplicity.md) is a positive integer. At $p\in C\cap D$,

$$
\boxed{I_p(C,D)=1\iff p\text{ is nonsingular on both curves and }T_pC\ne T_pD.}
$$

This is the criterion for a [transverse intersection of plane curves](../../../../transverse-intersection-of-plane-curves.md). In particular, an intersection at a [singular point](../../../../singular-point-of-an-algebraic-variety.md) of either curve contributes at least two.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the algebraic curves course of the University of Oxford](../../../split.md)
5. [Algebraic curves course of the University of Oxford](../../../../algebraic-curves-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
