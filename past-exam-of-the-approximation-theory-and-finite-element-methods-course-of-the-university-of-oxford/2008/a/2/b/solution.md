<h1 id="a/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The displayed recurrence requires monic normalization, which is not explicitly stated in the preamble. Arbitrary independent rescaling of [orthogonal polynomials](../../../../../orthogonal-polynomial-split.md) preserves orthogonality but changes the recurrence coefficients. Choose their monic representatives for this and the following calculations.

Expand $x\phi_n$ in the orthogonal [polynomial](../../../../../polynomial-split.md) basis:

$$
x\phi_n=\phi_{n+1}+\sum_{j=0}^na_j\phi_j.
$$

The leading coefficient of $\phi_{n+1}$ is one. For $j\leq n-2$, $(x\phi_n,\phi_j)=(\phi_n,x\phi_j)=0$, because the second factor has degree below $n$. Thus only $j=n,n-1$ remain. Inner products give

$$
a_n=\frac{(\phi_n,x\phi_n)}{\|\phi_n\|^2},\qquad
a_{n-1}=\frac{(\phi_n,x\phi_{n-1})}{\|\phi_{n-1}\|^2}
=\frac{\|\phi_n\|^2}{\|\phi_{n-1}\|^2}.
$$

The last equality uses $x\phi_{n-1}-\phi_n\in P_{n-1}$. Rearranging yields exactly the [three-term recurrence for monic orthogonal polynomials](../../../../../three-term-recurrence-for-monic-orthogonal-polynomials.md)

$$
\boxed{\phi_{n+1}=(x-a_n)\phi_n-
\frac{\|\phi_n\|^2}{\|\phi_{n-1}\|^2}\phi_{n-1}.}
$$

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
