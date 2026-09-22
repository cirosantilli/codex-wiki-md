<h1 id="a/2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose the nodes as the $n+1$ roots of the [Chebyshev polynomial](../../../../../chebyshev-polynomial.md) $T_{n+1}$. Its leading coefficient is $2^n$, so the monic nodal product is $\omega=2^{-n}T_{n+1}$. Since $|T_{n+1}|\leq1$ on $[-1,1]$, part (b) bounds this particular interpolant by

$$
\|u-p_n\|_\infty\leq
\frac{\|u^{(n+1)}\|_\infty}{2^n(n+1)!}.
$$

The best error cannot exceed the error of a particular member of $P_n$. Therefore

$$
\boxed{E_n\leq
\frac{\|u^{(n+1)}\|_\infty}{2^n(n+1)!}.}
$$

The choice of Chebyshev roots controls the maximum of the nodal product, not the size of any individual [interpolation](../../../../../interpolation-split.md) coefficient.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
