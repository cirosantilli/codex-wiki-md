<h1 id="a/2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For $n\geq1$, $\phi_n$ is [orthogonal](../../../../../orthogonal-vectors.md) to every [polynomial](../../../../../polynomial-split.md) in $P_{n-1}$, so $(u,\phi_n)=(u-p_{n-1}^*,\phi_n)$. The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives

$$
|(u,\phi_n)|\leq E_{n-1}\int_0^1x^2|\phi_n|\,dx
\leq E_{n-1}\left(\int_0^1x^2\,dx\right)^{1/2}\|\phi_n\|_2
=\boxed{E_{n-1}/\sqrt3}.
$$

Using the tail identity from part (b) and shifting the index,

$$
\boxed{\|u-p_n\|_2^2\leq\frac13\sum_{r=n}^\infty E_r^2.}
$$

For the stated power law and $n>1$, the decreasing-function [integral test](../../../../../integral-test-for-convergence.md) gives

$$
\sum_{r=n}^\infty r^{-2a}\leq\int_{n-1}^\infty x^{-2a}\,dx=\frac{(n-1)^{1-2a}}{2a-1}.
$$

Consequently

$$
\boxed{\|u-p_n\|_2\leq\frac K{\sqrt3}\frac{(n-1)^{-a+1/2}}{\sqrt{2a-1}}.}
$$

The assumption $a>1$ is sufficient; this summation estimate itself only needs $a>1/2$.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
