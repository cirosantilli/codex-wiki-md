<h1 id="a/2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

With $d=\Delta x$, define the [semidiscrete Fourier transform](../../../../../semidiscrete-fourier-transform.md) by

$$
\widehat U(k)=d\sum_{j\in\mathbb Z}U_j e^{-ikjd},\qquad -\pi/d\leq k\leq\pi/d.
$$

For finite-support sequences, expand the squared modulus and use [orthogonality](../../../../../orthogonal-vectors.md):

$$
\int_{-\pi/d}^{\pi/d}e^{-ik(j-\ell)d}dk=\frac{2\pi}d\mathbf1_{\{j=\ell\}}.
$$

Consequently

$$
\int_{-\pi/d}^{\pi/d}|\widehat U(k)|^2dk
=2\pi d\sum_j|U_j|^2.
$$

For a general square-summable sequence, truncate it to $|j|\leq N$. The identity makes the transformed truncations Cauchy in $L^2$, and [completeness](../../../../../completeness.md) defines the transform as their $L^2$ limit. Passing to the limit proves the [Parseval identity](../../../../../parseval-identity.md)

$$
\boxed{\|U\|_{\ell^2}^2=(2\pi)^{-1}\|\widehat U\|_{L^2}^2.}
$$

The infinite series need not converge absolutely pointwise; the $L^2$ interpretation is sufficient for the stability analysis.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the numerical solution of differential equations course of the University of Oxford](../../../../split.md)
6. [Numerical solution of differential equations course of the University of Oxford](../../../../../numerical-solution-of-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
