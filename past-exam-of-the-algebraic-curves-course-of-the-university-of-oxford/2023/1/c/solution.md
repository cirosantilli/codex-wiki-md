<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

There is a [nonsingular point of an algebraic curve](../../../../nonsingular-point-of-an-algebraic-curve.md) on $C$, since part (b) makes its [singular locus](../../../../singular-locus.md) finite whereas a [projective curve](../../../../projective-curve.md) has infinitely many complex points. Apply a [projective transformation](../../../../projective-linear-transformation.md) taking one such point to $p=[1:0:0]$, and use $P$ for the transformed [homogeneous polynomial](../../../../homogeneous-polynomial.md). As in part (b), $P_x$ is nonzero and $D=V(P_x)$ has no common [irreducible component](../../../../irreducible-component.md) with $C$.

The [Euler theorem for homogeneous functions](../../../../euler-theorem-for-homogeneous-functions.md) and its differentiated identities give

$$
P_x(p)=dP(p)=0,
\qquad
P_{xx}(p)=(d-1)P_x(p)=0,
$$

and

$$
P_{xy}(p)=(d-1)P_y(p),
\qquad
P_{xz}(p)=(d-1)P_z(p).
$$

Since $p$ is nonsingular on $C$, at least one of $P_y(p),P_z(p)$ is nonzero. Because $d>1$, the [polar curve](../../../../polar-curve.md) $D$ is also nonsingular at $p$, and these identities show that $T_pD=T_pC$. Hence $I_p(C,D)\geq2$.

This additional intersection is separate from all the [singular points](../../../../singular-point-of-an-algebraic-variety.md) of $C$. Thus [Bézout's theorem](../../../../bezout-s-theorem.md) gives

$$
2s+2\leq\sum_{q\in C\cap D}I_q(C,D)\leq d(d-1),
\qquad
\boxed{s\leq\frac{d(d-1)}2-1.}
$$

The improvement comes from making the [polar curve](../../../../polar-curve.md) tangent at a chosen nonsingular point, thereby reserving at least two of the available intersections.

## ↑ Ancestors (12)

1. [C](../c.md)
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
