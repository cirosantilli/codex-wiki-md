<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Lagrange interpolation polynomial](../../../../lagrange-polynomial.md) is

$$
p(x)=\sum_{r=0}^n u_r\frac{\pi_{n,r}(x)}{\pi_{n,r}(x_r)},\qquad
\boxed{w_r=\frac1{\pi_{n,r}(x_r)}=\frac1{\pi_n'(x_r)}=\prod_{s\ne r}(x_r-x_s)^{-1}.}
$$

The [interpolation nodes](../../../../interpolation-node.md) are distinct, so these weights are well defined. Applying the same [Lagrange interpolation](../../../../lagrange-polynomial.md) to the constant [polynomial](../../../../polynomial-split.md) one gives $1=\sum_r w_r\pi_{n,r}(x)$. Dividing this identity and the formula for $p$ by $\pi_n(x)$ gives the [barycentric interpolation formula](../../../../barycentric-interpolation-formula.md)

$$
\boxed{p(x)=\frac{\sum_{r=0}^n w_ru_r/(x-x_r)}{\sum_{r=0}^n w_r/(x-x_r)}.}
$$

This displayed quotient is used away from the [interpolation nodes](../../../../interpolation-node.md); at $x=x_r$ its removable singularity is evaluated by setting $p(x_r)=u_r$. Multiplying every weight by the same nonzero constant leaves the quotient unchanged.

**Chebyshev points are generally more reliable at high degree.** The [Chebyshev-Lobatto nodes](../../../../chebyshev-lobatto-node.md), or the affine images of the roots of a [Chebyshev polynomial](../../../../chebyshev-polynomial.md), cluster near the interval endpoints and control the amplification measured by the [Lebesgue constant of interpolation](../../../../lebesgue-constant-of-interpolation.md). Equally spaced [interpolation nodes](../../../../interpolation-node.md) can produce large endpoint oscillations and the [Runge phenomenon](../../../../runge-s-phenomenon.md). This is a comparison of numerical robustness and general approximation behaviour, not a claim that one set minimizes the error for every individual [function](../../../../function-split.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the approximation of functions course of the University of Oxford](../../../split.md)
5. [Approximation of functions course of the University of Oxford](../../../../approximation-of-functions-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
