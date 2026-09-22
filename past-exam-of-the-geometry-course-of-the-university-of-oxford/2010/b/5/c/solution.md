<h1 id="b/5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write the irreducible curve as $F=0$, with $F$ homogeneous of degree $n$. For $n=1$ there are no singular points. Otherwise choose a nonzero partial derivative, say $F_x$, which has degree $n-1$. Such a derivative exists in [characteristic zero](../../../../../characteristic-zero.md). Irreducibility and its smaller degree show that $F$ and $F_x$ have no common component.

At every [singular point](../../../../../singular-point-of-an-algebraic-variety.md) $p$ of $C$, $F_x(p)=0$ and the curve multiplicity of $F$ is at least two. The standard local lower bound for [intersection multiplicity](../../../../../intersection-multiplicity.md) gives $I_p(F,F_x)\geq2$. Applying the [Bézout theorem](../../../../../bezout-s-theorem.md),

$$
2\#\operatorname{Sing}(C)\leq\sum_{p\in C\cap\{F_x=0\}}I_p(F,F_x)=n(n-1).
$$

Therefore

$$
\boxed{\#\operatorname{Sing}(C)\leq\tfrac12n(n-1).}
$$

This is the [polar bound for singular points of a plane curve](../../../../../polar-bound-for-singular-points-of-a-plane-curve.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the geometry course of the University of Oxford](../../../../split.md)
6. [Geometry course of the University of Oxford](../../../../../geometry-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
