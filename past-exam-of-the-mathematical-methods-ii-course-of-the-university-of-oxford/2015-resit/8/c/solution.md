<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A one-form $A(x,y)\,dx+B(x,y)\,dy$ is an [exact differential](../../../../exact-differential.md) if a single-valued differentiable [potential of a conservative vector field](../../../../potential-of-a-conservative-vector-field.md) $f$ satisfies $A=f_x$ and $B=f_y$ on the domain. Then it equals $df$, and its integral along a path is the endpoint difference of $f$.

Integrate $f_x=10x^4-2xy^3$ with respect to $x$:

$$
f(x,y)=2x^5-x^2y^3+g(y).
$$

Its $y$ derivative is $-3x^2y^2+g'(y)$. Matching the required second component [forces](../../../../force-split.md) $g'(y)=0$, so the additive constant is arbitrary and

$$
df=(10x^4-2xy^3)\,dx-3x^2y^2\,dy.
$$

The [fundamental theorem for line integrals](../../../../fundamental-theorem-for-line-integrals.md) now gives

$$
\boxed{I=f(2,1)-f(0,0)=2(2^5)-2^2=60},
$$

independently of the convenient segmented path used before. Merely checking equality of mixed partial derivatives on an unspecified domain would not by itself construct this globally defined potential.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [8](../../8.md)
3. [2015 resit](../../../2015-resit-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
