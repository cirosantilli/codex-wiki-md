<h1 id="a/1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $x=\cos\theta$. The trigonometric identity

$$
\cos((n+1)\theta)+\cos((n-1)\theta)=2\cos\theta\cos(n\theta)
$$

gives the [Chebyshev polynomial](../../../../../chebyshev-polynomial.md) recurrence $T_{n+1}=2xT_n-T_{n-1}$. Starting from $T_0=1$ and $T_1=x$, successive substitution yields

$$
\boxed{T_0=1,\quad T_1=x,\quad T_2=2x^2-1,\quad
T_3=4x^3-3x,\quad T_4=8x^4-8x^2+1.}
$$

The recurrence also proves by induction that $T_n$ is a [polynomial](../../../../../polynomial-split.md) of degree $n$, with leading coefficient $2^{n-1}$ for $n\geq1$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
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
