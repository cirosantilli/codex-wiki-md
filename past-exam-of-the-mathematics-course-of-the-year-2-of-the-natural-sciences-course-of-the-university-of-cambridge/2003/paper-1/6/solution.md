<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

For the normalized second-order [linear differential equation](../../../../linear-differential-equation.md) $y''+P(z)y'+Q(z)y=0$, an [ordinary point](../../../../ordinary-point-criterion-for-a-second-order-equation.md) $z_0$ has analytic $P,Q$ near $z_0$. At a [regular singular point](../../../../regular-singular-point.md), which is not ordinary, $(z-z_0)P(z)$ and $(z-z_0)^2Q(z)$ are analytic. Ordinary points admit two independent convergent [power series](../../../../power-series.md) solutions. Regular singular points instead call for the [Frobenius method](../../../../frobenius-method.md), which permits leading powers and, in some cases, [logarithms](../../../../logarithm.md).

Here zero is an [ordinary point](../../../../ordinary-point-criterion-for-a-second-order-equation.md). Substitute $y=\sum_{n\geq0}a_nz^n$ into the [Hermite differential equation](../../../../hermite-differential-equation.md) and equate coefficients:

$$
(n+2)(n+1)a_{n+2}+(\lambda-2n)a_n=0,\qquad\boxed{a_{n+2}=\frac{2n-\lambda}{(n+2)(n+1)}a_n.}
$$

The even and odd initial coefficients are independent, giving

$$
y=a_0\left[1-\frac\lambda2z^2+\frac{\lambda(\lambda-4)}{24}z^4+\cdots\right]+a_1\left[z+\frac{2-\lambda}{6}z^3+\frac{(2-\lambda)(6-\lambda)}{120}z^5+\cdots\right].
$$

These are the [power series solutions of the Hermite differential equation](../../../../power-series-solutions-of-the-hermite-differential-equation.md), with the present parameter equal to twice the parameter in that article. The ratio of successive terms within each nonterminating parity is asymptotically $2|z|^2/n$, so both series have infinite [radius of convergence](../../../../radius-of-convergence.md).

For a nonzero [polynomial](../../../../polynomial-split.md) of degree $m$, its highest coefficient in $-2zy'+\lambda y$ forces $\lambda=2m$. Conversely at that value the matching parity terminates. Hence

$$
\boxed{\lambda=2m,\qquad m=0,1,2,\ldots.}
$$

The [polynomial](../../../../polynomial-split.md) solutions are [scalar multiples](../../../../scalar-multiple.md) of the [Hermite polynomials](../../../../hermite-polynomial.md). Two examples are $\boxed{\lambda=0:\ y=1;\qquad\lambda=2:\ y=z}$; direct substitution verifies both. The other independent solution generally remains nonpolynomial.

## ↑ Ancestors (12)

1. [6](../6.md)
2. [Paper 1](../../paper-1-split.md)
3. [2003](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
