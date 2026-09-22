<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For an axisymmetric surface $r=a(z,t)$, twice the [mean curvature](../../../../../../mean-curvature.md) with the outward-normal convention is

$$
\kappa=\frac1{a\sqrt{1+a_z^2}}
-\frac{a_{zz}}{(1+a_z^2)^{3/2}}.
$$

Writing $a=a_0+\eta$ and retaining linear terms gives

$$
\boxed{\kappa=\frac1{a_0}
-\frac{\eta}{a_0^2}-\eta_{zz}},
\qquad
\kappa'= -\frac{\eta}{a_0^2}-\eta_{zz}.
$$

At the unperturbed boundary $r=a_0$, the linearized [kinematic boundary condition](../../../../../../kinematic-boundary-condition.md), tangential-stress condition, and [Young–Laplace equation](../../../../../../young-laplace-equation.md) are

$$
u=\eta_t,
\qquad
\sigma_{rz}=\mu(u_z+w_r)=0,
\qquad
p'-2\mu u_r=\gamma\kappa'.
$$

For a normal mode $e^{ikz+st}$ these become $u(a_0)=s\eta$, $\sigma_{rz}(a_0)=0$, and

$$
p'(a_0)-2\mu u_r(a_0)
=\gamma(k^2-a_0^{-2})\eta.
$$

The [Papkovich–Neuber representation](../../../../../../papkovich-neuber-representation.md) of body-force-free [Stokes flow](../../../../../../stokes-flow-split.md) is

$$
2\mu\mathbf u=\nabla(\mathbf x\mathbin\cdot\boldsymbol\Phi+\chi)-2\boldsymbol\Phi,
\qquad
p=\nabla\mathbin\cdot\boldsymbol\Phi,
$$

where $\boldsymbol\Phi$ and $\chi$ are harmonic.

Let $x=kr$ and $E=e^{ikz+st}$. Substitution of the given radial vector potential and scalar potential gives

$$
\boxed{
u=\frac{E}{2\mu}
\left[P(xI_1'(x)-I_1(x))+QI_0'(x)\right]},
$$



$$
\boxed{
w=\frac{iE}{2\mu}
\left[PxI_1(x)+QI_0(x)\right]},
\qquad
p=PkI_0(x)E.
$$

Using the [modified Bessel function](../../../../../../modified-bessel-function.md) identity $(xI_1)'=xI_0$, the tangential stress simplifies to

$$
\boxed{
\sigma_{rz}=ikE
\left[PxI_1'(x)+QI_0'(x)\right]}.
$$

The stress-free condition at $r=a$ therefore yields

$$
\boxed{PxI_1'(x)+QI_0'(x)=0
\quad\text{at }x=ka}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
