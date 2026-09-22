<h1 id="a/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [monic orthogonal polynomials](../../../../../monic-orthogonal-polynomial.md) $\phi_0,\ldots,\phi_{r+1}$ form a basis of $P_{r+1}$, ordered by degree. Since $x\phi_r$ is monic of degree $r+1$,

$$
x\phi_r=\phi_{r+1}+\sum_{j=0}^ra_j\phi_j.
$$

For $j\leq r-2$, symmetry of multiplication by $x$ gives $(x\phi_r,\phi_j)=(\phi_r,x\phi_j)=0$, because $\deg(x\phi_j)<r$. Only $a_r$ and $a_{r-1}$ remain. Taking inner products with $\phi_r$ yields $a_r=(\phi_r,x\phi_r)/(\phi_r,\phi_r)$.

Similarly,

$$
a_{r-1}=\frac{(x\phi_r,\phi_{r-1})}{(\phi_{r-1},\phi_{r-1})}
=\frac{(\phi_r,x\phi_{r-1})}{(\phi_{r-1},\phi_{r-1})}
=\frac{(\phi_r,\phi_r)}{(\phi_{r-1},\phi_{r-1})},
$$

since $x\phi_{r-1}-\phi_r$ has degree at most $r-1$. Rearranging proves the [three-term recurrence for monic orthogonal polynomials](../../../../../three-term-recurrence-for-monic-orthogonal-polynomials.md):

$$
\boxed{\phi_{r+1}=(x-a_r)\phi_r-
\frac{\|\phi_r\|_2^2}{\|\phi_{r-1}\|_2^2}\phi_{r-1}.}
$$

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
