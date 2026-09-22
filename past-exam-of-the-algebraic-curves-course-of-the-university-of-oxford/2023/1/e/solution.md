<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Take a union of $d$ distinct lines in [general position for projective lines](../../../../general-position-for-projective-lines.md), meaning that no three pass through one point. Each pair contributes one distinct [singular point](../../../../singular-point-of-an-algebraic-variety.md), and every other point lies on just one nonsingular line. Thus the union has [degree of a projective curve](../../../../degree-of-a-projective-curve.md) $d$ and exactly

$$
\boxed{\binom d2=\frac{d(d-1)}2}
$$

distinct [singular points](../../../../singular-point-of-an-algebraic-variety.md). For $d=1$, this gives a line with zero [singular points](../../../../singular-point-of-an-algebraic-variety.md), as required.

For a concrete construction, choose distinct $t_1,\ldots,t_d\in\mathbb C$ and set

$$
L_i:\quad y=t_i x+t_i^2z,
\qquad
C:\quad\prod_{i=1}^d(y-t_ix-t_i^2z)=0.
$$

For $i\ne j$, the intersection is $[-(t_i+t_j):-t_it_j:1]$. Substitution into the equation of $L_k$ gives $-(t_k-t_i)(t_k-t_j)$, which is nonzero when $k$ is distinct from $i,j$. Thus there are no triple intersections, including at infinity.

## ↑ Ancestors (12)

1. [E](../e.md)
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
