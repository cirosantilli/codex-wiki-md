<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [Newton-Cotes quadrature](../../../../newton-cotes-quadrature.md) integrates a [Lagrange interpolation polynomial](../../../../lagrange-polynomial.md) at equally spaced [quadrature nodes](../../../../quadrature-node.md). For the [Newton-Cotes closed quadrature](../../../../newton-cotes-closed-quadrature.md), the endpoints are included: write $x_j=a+jh$, $h=(b-a)/n$, and use

$$
\int_a^bf(x)\,dx\ \approx\ \int_a^bp_n(x)\,dx
=\sum_{j=0}^n W_jf(x_j),\qquad W_j=\int_a^b\ell_j(x)\,dx.
$$

These [quadrature weights](../../../../quadrature-weight.md) depend on the [quadrature nodes](../../../../quadrature-node.md), not on the sampled [function](../../../../function-split.md). Open [Newton-Cotes quadrature](../../../../newton-cotes-quadrature.md) uses equally spaced interior [quadrature nodes](../../../../quadrature-node.md) instead.

For [Simpson's rule](../../../../simpson-s-rule.md), use $n=2$ and set $x=a+ht$, so $0\leq t\leq2$. The [Lagrange cardinal polynomials](../../../../lagrange-cardinal-polynomial.md) become

$$
L_0(t)=\frac{(t-1)(t-2)}2,\qquad L_1(t)=t(2-t),\qquad L_2(t)=\frac{t(t-1)}2.
$$

Integrating these [quadratic polynomials](../../../../quadratic-polynomial.md) gives $1/3$, $4/3$, $1/3$, respectively. The change of variable contributes $h$, so

$$
\boxed{\int_a^bf(x)\,dx\ \approx\ \frac h3\bigl[f(a)+4f(a+h)+f(b)\bigr]
=\frac{b-a}{6}\left[f(a)+4f\!\left(\frac{a+b}{2}\right)+f(b)\right].}
$$

Its [degree of precision of a quadrature rule](../../../../degree-of-precision-of-a-quadrature-rule.md) is three: it integrates every [quadratic polynomial](../../../../quadratic-polynomial.md) by construction, and also the cubic nodal [polynomial](../../../../polynomial-split.md) $(x-a)(x-a-h)(x-b)$, whose [integral](../../../../integral-split.md) vanishes by odd symmetry about $a+h$. Any [cubic polynomial](../../../../cubic-polynomial.md) differs from its [quadratic polynomial](../../../../quadratic-polynomial.md) [interpolant](../../../../interpolant.md) by a constant multiple of this nodal [polynomial](../../../../polynomial-split.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the numerical analysis course of the University of Oxford](../../../split.md)
5. [Numerical analysis course of the University of Oxford](../../../../numerical-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
