<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Take $z$ upward along the straight rod. The part above height $z$ has weight $\lambda g(L-z)$, so, with tensile force positive, the internal tension is compressive:

$$
\boxed{\sigma(z)=-\lambda g(L-z)}.
$$

For a small transverse displacement $X(z)$, the quadratic bending and gravitational energies are

$$
\mathcal E[X]
=\frac A2\int_0^L(X'')^2\,dz
-\frac{\lambda g}{2}\int_0^L(L-z)(X')^2\,dz.
$$

The [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) for this functional is

$$
AX''''+\bigl[\lambda g(L-z)X'\bigr]'=0,
$$

which is exactly

$$
\boxed{AX_{zzzz}-(\sigma X_z)_z=0}.
$$

Clamping at the bottom fixes displacement and slope:

$$
X(0)=0,\qquad X'(0)=0.
$$

At the free upper end, bending moment and transverse force vanish:

$$
AX''(L)=0,\qquad AX'''(L)-\sigma(L)X'(L)=0.
$$

Since $\sigma(L)=0$, the four boundary conditions are

$$
\boxed{X(0)=X'(0)=0,\qquad X''(L)=X'''(L)=0}.
$$

Set $u=X'$. Integrating the field equation once and using the free-end shear condition gives

$$
Au''-\sigma u=0,
$$

or, with $s=L-z$,

$$
u_{ss}+\frac{\lambda g}{A}s\,u=0.
$$

Introduce the dimensionless similarity coordinate

$$
\eta=\frac23\left(\frac{\lambda g}{A}s^3\right)^{1/2}
$$

and write $u=\eta^{1/3}F(\eta)$. Direct substitution reduces the equation to

$$
\eta^2F''+\eta F'
+\left(\eta^2-\frac19\right)F=0.
$$

This is the [Bessel differential equation](../../../../../bessel-differential-equation.md) of order $1/3$, so

$$
\boxed{
u=\eta^{1/3}\left[aJ_{-1/3}(\eta)+bJ_{1/3}(\eta)\right]}.
$$

The free-moment condition is $u'(L)=0$. As $\eta\to0$,

$$
\eta^{1/3}J_{-1/3}(\eta)\sim\text{constant},
\qquad
\eta^{1/3}J_{1/3}(\eta)\sim\eta^{2/3}\propto s.
$$

The second term has nonzero limiting $z$ derivative, so the free-end condition forces $b=0$. The free-shear condition $u''(L)=0$ then follows from the differential equation. At the clamp, $u(0)=0$, giving

$$
J_{-1/3}(\eta_0)=0,\qquad
\eta_0=\frac23\left(\frac{\lambda gL^3}{A}\right)^{1/2}.
$$

Let $j_{-1/3,1}$ be the smallest positive zero of this [Bessel function](../../../../../bessel-function.md). The first [self-buckling threshold](../../../../../self-buckling-of-a-vertical-rod.md) is

$$
\boxed{
\frac23\left(\frac{\lambda gL^3}{A}\right)^{1/2}
=j_{-1/3,1}},
$$

or equivalently

$$
\boxed{\frac{\lambda gL^3}{A}
=\frac94j_{-1/3,1}^2}.
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 355](../../paper-355-split.md)
3. [Iii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
