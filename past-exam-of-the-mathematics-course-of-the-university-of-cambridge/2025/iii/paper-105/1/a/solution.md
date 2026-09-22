<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The scalar [Cauchy-Kovalevskaya theorem](../../../../../../cauchy-kovalevskaya-theorem.md) says that a [partial differential equation](../../../../../../partial-differential-equation-split.md) solved for its highest derivative normal to a [real-analytic](../../../../../../real-analytic-function.md) [non-characteristic hypersurface](../../../../../../non-characteristic-hypersurface.md), with real-analytic coefficients and [Cauchy data](../../../../../../cauchy-data.md), has a unique local real-analytic solution. In coordinates, an equation

$$
\partial_t^m\phi=F\bigl(t,x,(\partial_t^j\partial_x^\alpha\phi)_{j<m}\bigr)
$$

has such a solution near the origin when $F$ and the prescribed values of $\partial_t^j\phi(0,x)$ for $0\leq j<m$ are real analytic.

Choose a real-analytic primitive $F_0$ of $f$ near zero and apply the theorem to the scalar [Laplace equation](../../../../../../laplace-equation.md)

$$
\phi_{tt}=-\phi_{xx},
\qquad
\phi(0,x)=F_0(x),
\qquad
\phi_t(0,x)=-g(x).
$$

The line $t=0$ is [non-characteristic](../../../../../../non-characteristic-hypersurface.md) because the coefficient of $\phi_{tt}$ is one. Define

$$
u=\phi_x,
\qquad
v=-\phi_t.
$$

Then $u(0,x)=f(x)$ and $v(0,x)=g(x)$, while equality of mixed derivatives and the Laplace equation give

$$
u_t=\phi_{xt}=-v_x,
\qquad
v_t=-\phi_{tt}=\phi_{xx}=u_x.
$$

**Thus $(u,v)$ is the required local real-analytic solution.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
