<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Trying $y=x^m$ in the [Cauchy-Euler equation](../../../../cauchy-euler-equation.md) gives

$$
m(m-1)+4m-4=(m-1)(m+4)=0,
$$

so the [homogeneous solution](../../../../homogeneous-solution.md) is

$$
\boxed{y=C_1x+C_2x^{-4}.}
$$

Continuity with zero value at the singular endpoint excludes the second branch. Use the left and right adapted solutions $\ell(x)=x$, $r(x)=x^{-4}-x$, whose [Wronskian](../../../../wronskian.md) is

$$
W(x)=\ell r'-\ell'r=-5x^{-4}.
$$

The [Dirichlet Green kernel for an Euler operator with exponents one and minus four](../../../../dirichlet-green-kernel-for-an-euler-operator-with-exponents-one-and-minus-four.md) is therefore

$$
\boxed{G(x,\xi)=\frac15\begin{cases}x(\xi^5-1),&x\leq\xi,\\\xi^5(x-x^{-4}),&x\geq\xi.\end{cases}}
$$

It vanishes at both endpoints, is continuous at $x=\xi$, and has first-derivative jump

$$
G_x(\xi^+,\xi)-G_x(\xi^-,\xi)=\frac{\ell(\xi)r'(\xi)-\ell'(\xi)r(\xi)}{W(\xi)}=1.
$$

Thus $L_xG=\delta(x-\xi)$ with ordinary source measure $d\xi$. For bounded forcing the [Green function](../../../../green-s-function-split.md) representation is

$$
\boxed{u(x)=\frac{x-x^{-4}}5\int_0^x\xi^5f(\xi)d\xi+\frac x5\int_x^1(\xi^5-1)f(\xi)d\xi.}
$$

The apparent singular prefactor in the first term is canceled by the integral's decay at zero. The only regular homogeneous solution vanishing at $1$ is zero, so this solution is unique in the stated regular class.

For the piecewise source, split the integrals at $1/2$. If $x<1/2$, the needed integrals are $\int_0^x\xi^6d\xi=x^7/7$ and $\int_x^{1/2}(\xi^6-\xi)d\xi$. If $x>1/2$, only $\int_0^{1/2}\xi^6d\xi=1/896$ remains. Simplification yields

$$
\boxed{u(x)=\begin{cases}\displaystyle\frac{x^3}{14}-\frac{111x}{4480},&0\leq x\leq\frac12,\\\displaystyle\frac{x-x^{-4}}{4480},&\frac12\leq x\leq1.\end{cases}}
$$

At the interface both expressions have value $-31/8960$ and derivative $129/4480$, so no unintended [Dirac delta](../../../../dirac-delta-function.md) source appears. Their second derivatives have the allowed jump associated with the discontinuous forcing.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [2011](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
