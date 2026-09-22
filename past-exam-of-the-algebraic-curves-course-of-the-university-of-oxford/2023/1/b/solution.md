<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

If $d=1$, $C$ is a line and has no [singular points](../../../../singular-point-of-an-algebraic-variety.md). Suppose $d>1$ and take $P$ to be an [irreducible polynomial](../../../../irreducible-polynomial.md). First, $P_x$ is not the zero [polynomial](../../../../polynomial-split.md): otherwise $P\in\mathbb C[y,z]$, and a [homogeneous polynomial](../../../../homogeneous-polynomial.md) in two variables of degree greater than one factors into linear factors over $\mathbb C$, contrary to irreducibility.

Let $D=V(P_x)$ be the [polar curve](../../../../polar-curve.md) in this coordinate direction. Since $\deg P_x=d-1<d$, the [irreducible polynomial](../../../../irreducible-polynomial.md) $P$ cannot divide $P_x$. Thus $C,D$ have no common [irreducible component](../../../../irreducible-component.md), and [Bézout's theorem](../../../../bezout-s-theorem.md) applies. One may count repeated factors of $P_x$ with their multiplicities; alternatively, passing to its reduced equation only decreases $\deg D$.

Every [singular point](../../../../singular-point-of-an-algebraic-variety.md) $p$ of $C$ satisfies $P_x(p)=0$ and has $I_p(C,D)\geq2$ by part (a). Consequently, if $s$ is the number of distinct [singular points](../../../../singular-point-of-an-algebraic-variety.md),

$$
2s\leq\sum_{p\in C\cap D}I_p(C,D)\leq d(d-1),
\qquad
\boxed{s\leq\frac{d(d-1)}2.}
$$

This argument also proves that the [singular locus](../../../../singular-locus.md) is finite.

## ↑ Ancestors (12)

1. [B](../b.md)
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
