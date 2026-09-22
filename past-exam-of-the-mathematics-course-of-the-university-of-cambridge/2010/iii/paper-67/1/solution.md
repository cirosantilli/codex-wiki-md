<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Put $B=EI_2$, the [filament bending modulus](../../../../../filament-bending-modulus.md) in the easier bending direction; $I_2$ is the relevant [second moment of area](../../../../../second-moment-of-area.md). Take [filament tension](../../../../../filament-tension.md) as positive in extension. A cut at height $z$ supports the weight of the material above it, so its axial force is compressive:

$$
\boxed{T(z)=-\lambda g(L-z)},\qquad T(L)=0.
$$

The small transverse displacement induces a transverse tension force density $(TX_z)_z$, while bending produces $-BX_{zzzz}$. Their balance gives

$$
\boxed{BX_{zzzz}-(TX_z)_z=0}.
$$

The same result follows from [elastic energy](../../../../../elastic-energy.md) and [gravitational energy](../../../../../gravitational-energy.md). To quadratic order, local [inextensibility](../../../../../inextensible-filament.md) shortens the height of the material point labelled $z$ by $\frac12\int_0^zX_z(s)^2ds$. Integrating its weight and interchanging the integrals gives the second-order [potential energy](../../../../../potential-energy.md)

$$
\mathcal E_2[X]=\frac12\int_0^L\left[B X_{zz}^2-\lambda g(L-z)X_z^2\right]dz
=\frac12\int_0^L\left[B X_{zz}^2+T X_z^2\right]dz.
$$

Two [integration by parts](../../../../../integration-by-parts.md) steps in its first variation give

$$
\delta\mathcal E_2=\int_0^L[BX_{zzzz}-(TX_z)_z]\delta X\,dz
+\left[BX_{zz}\delta X_z+(TX_z-BX_{zzz})\delta X\right]_0^L.
$$

The [clamped boundary conditions](../../../../../clamped-boundary-condition.md) fix displacement and slope at the base, and the unconstrained tip must have zero bending moment and transverse end force. Thus the complete four conditions are

$$
\boxed{X(0)=X_z(0)=0,\qquad X_{zz}(L)=0,\qquad
BX_{zzz}(L)-T(L)X_z(L)=0}.
$$

Since the [filament tension](../../../../../filament-tension.md) vanishes at the tip, the last condition is $X_{zzz}(L)=0$. Integrate the [ordinary differential equation](../../../../../ordinary-differential-equation.md) once: $BX_{zzz}-TX_z$ is constant, and its tip value makes that constant zero. For the slope $u=X_z$, it follows that

$$
B u_{zz}+\lambda g(L-z)u=0,\qquad
\boxed{u(0)=0,\quad u_z(L)=0}.
$$

The other tip condition $u_{zz}(L)=0$ already follows from this equation for a regular solution; it is not a third independent condition on the second-order slope problem. Finally reconstruct $X(z)=\int_0^zu(s)ds$ to impose the base position.

Set $x=L-z$, $\alpha=\lambda g/B$, and $\eta=(2/3)\sqrt\alpha\,x^{3/2}$. Then $d\eta/dx=3\eta/(2x)$ and $d^2\eta/dx^2=3\eta/(4x^2)$, so $u_{xx}+\alpha xu=0$ becomes

$$
\eta^2u_{\eta\eta}+\frac13\eta u_\eta+\eta^2u=0.
$$

Substituting $u=\eta^{1/3}F(\eta)$ gives

$$
\eta^2F''+\eta F'+\left(\eta^2-\frac19\right)F=0.
$$

This is the [Bessel differential equation](../../../../../bessel-differential-equation.md) of order $1/3$, whose two independent [Bessel functions of the first kind](../../../../../bessel-function-of-the-first-kind.md) give

$$
\boxed{u=\eta^{1/3}\left[aJ_{-1/3}(\eta)+bJ_{1/3}(\eta)\right]}.
$$

The tip is $x=\eta=0$. To decide which branch is admissible, retain both leading behaviours, not just the fact that $u$ stays finite:

$$
\eta^{1/3}J_{-1/3}(\eta)
=\frac{2^{1/3}}{\Gamma(2/3)}\left[1-\frac38\eta^2+O(\eta^4)\right],\qquad
\eta^{1/3}J_{1/3}(\eta)
=\frac{\eta^{2/3}}{2^{1/3}\Gamma(4/3)}\left[1+O(\eta^2)\right].
$$

Since $\eta^2\propto x^3$ and $\eta^{2/3}\propto x$, the first branch has zero tip derivative, while the second has a nonzero tip derivative. The moment-free condition therefore sets $b=0$, and it does not require the tip slope itself to vanish. The base condition now requires

$$
J_{-1/3}\left(\frac23\sqrt{\frac{\lambda gL^3}{EI_2}}\right)=0.
$$

Let $j_{-1/3,1}$ be the first positive zero. The [Bessel threshold for self-buckling of a vertical rod](../../../../../bessel-threshold-for-self-buckling-of-a-vertical-rod.md) is

$$
\boxed{\frac{\lambda gL_c^3}{EI_2}=\frac94j_{-1/3,1}^2\simeq7.83735,
\qquad L_c\simeq1.98635\left(\frac{EI_2}{\lambda g}\right)^{1/3}}.
$$

To identify this as the first loss of stability, write the quadratic energy in terms of the slope as $\frac12[B\int u_z^2dz-\lambda g\int(L-z)u^2dz]$. On functions with $u(0)=0$, its critical coefficient is the minimum [Rayleigh quotient](../../../../../rayleigh-quotient.md) $\int u_z^2dz/\int(L-z)u^2dz$; variation supplies the moment-free condition at the tip and the same [Sturm-Liouville problem](../../../../../sturm-liouville-problem.md). The first zero gives the lowest [eigenvalue](../../../../../eigenvalue.md), so **the straight state is stable below this load, neutral at it, and unstable above it**, with the easier $I_2$ direction buckling first.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 67](../../paper-67-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
