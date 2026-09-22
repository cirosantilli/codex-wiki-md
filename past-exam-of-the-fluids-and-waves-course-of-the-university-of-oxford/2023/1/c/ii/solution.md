<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $P=p_\infty/\rho>0$. Multiplying the radius [ordinary differential equation](../../../../../ordinary-differential-equation.md) by $2R^2\dot R$ gives an exact derivative:

$$
\frac d{dt}(R^3\dot R^2)
=2R^2\dot R\left(R\ddot R+\frac32\dot R^2\right)
=-2PR^2\dot R=-\frac{2P}{3}\frac d{dt}(R^3).
$$

The [initial conditions](../../../../../initial-condition.md) therefore give the [first integral](../../../../../first-integral.md)

$$
R^3\dot R^2=\frac{2P}{3}(a^3-R^3),\qquad
\boxed{\dot R=-\sqrt{\frac{2p_\infty}{3\rho}
\left(\frac{a^3}{R^3}-1\right)}}.
$$

Choose the negative square root because the cavity starts accelerating inward. It cannot turn around while $0<R<a$, since the squared speed is then strictly positive. Separating variables, with $s=R/a$, proves the [collapse time of a spherical cavity](../../../../../collapse-time-of-a-spherical-cavity.md) is

$$
t_{\rm collapse}
=\sqrt{\frac{3\rho}{2p_\infty}}
\int_0^a\frac{R^{3/2}}{\sqrt{a^3-R^3}}\,dR
=a\sqrt{\frac\rho{p_\infty}}
\sqrt{\frac32}\int_0^1\frac{s^{3/2}}{\sqrt{1-s^3}}\,ds.
$$

Hence

$$
\boxed{t_{\rm collapse}=k\sqrt{\frac{\rho a^2}{p_\infty}},\qquad
k=\sqrt{\frac32}\int_0^1\frac{s^{3/2}}{\sqrt{1-s^3}}\,ds}.
$$

The [improper integral](../../../../../improper-integral.md) is finite: its integrand behaves as $s^{3/2}$ near zero and as $[3(1-s)]^{-1/2}$ near one. The divergent inward speed as $R\to0$ signals a singular endpoint of this ideal [incompressible flow](../../../../../incompressible-flow.md) model; the finite collapse time follows within that model.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the fluids and waves course of the University of Oxford](../../../../split.md)
6. [Fluids and waves course of the University of Oxford](../../../../../fluids-and-waves-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
