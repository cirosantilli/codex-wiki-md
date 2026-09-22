<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [material derivative](../../../../../material-derivative.md) follows [surfactant](../../../../../surfactant.md) carried by the moving interface. The term $-C\nabla_s\cdot u_s$ is dilution or concentration by tangential area expansion or contraction. The term $-C(u\cdot n)\nabla_s\cdot n$ is the additional area change produced by normal motion of a curved interface. The term $D_s\nabla_s^2C$ represents [surface diffusion](../../../../../surface-diffusion.md), while $-k(C-C_0)$ relaxes the concentration towards a reservoir value through exchange. All these terms refer to concentration per [surface area](../../../../../surface-area.md), as in [surfactant transport with exchange relaxation](../../../../../surfactant-transport-with-exchange-relaxation.md).

In the steady bubble frame, the spherical interface has $u\cdot n=0$. Write $C=C_0+C'$ with uniform $C_0$ and regard both $u$ and $C'$ as first order in the rising speed. Advection of $C'$ and its product with surface dilation are second order. Hence the linear steady equation is

$$
\boxed{D_s\nabla_s^2C'-kC'=C_0\nabla_s\cdot u_s.}
$$

Spherical symmetry and linearity leave only the tangential projection of the imposed translation vector: $u_s=A I_sU$. An azimuthal term $n\times U$ would change sign under reflection and is excluded for this non-chiral rising bubble. The degree-one forcing does not excite other spherical-harmonic degrees in the linear problem.

On $r=a$, differentiating $n=x/r$ gives

$$
\boxed{(\nabla_s n)_{ij}=\frac{\delta_{ij}-n_in_j}{a}=\frac{(I_s)_{ij}}a,\qquad \nabla_s\cdot n=\frac2a.}
$$

Each component of $n$ is a degree-one [spherical harmonic](../../../../../spherical-harmonic.md), so

$$
\boxed{\nabla_s^2n=-\frac{2n}{a^2}.}
$$

One may also obtain the coefficient from $n\cdot n=1$: its [surface Laplacian](../../../../../surface-laplacian.md) gives $n\cdot\nabla_s^2n=-|\nabla_sn|^2=-2/a^2$, while rotational symmetry makes the vector Laplacian parallel to $n$. Expanding $I_sU=U-n(U\cdot n)$ then yields

$$
\boxed{\nabla_s\cdot(I_sU)=-\frac2aU\cdot n.}
$$

The candidate $C'=B U\cdot n$ therefore solves the linear transport equation if

$$
-\left(k+\frac{2D_s}{a^2}\right)B=-\frac{2AC_0}{a},\qquad
\boxed{B=\frac{2AC_0a}{ka^2+2D_s}.}
$$

Its spherical mean is zero. This is the [dipolar surfactant distribution](../../../../../dipolar-surfactant-distribution.md). Assuming $ka^2+2D_s>0$, its consistency condition is

$$
\boxed{\frac{\max|C'|}{C_0}=\frac{2|A||U|a}{ka^2+2D_s}\ll1.}
$$

Diffusion or exchange must restore uniform concentration faster than the interfacial flow redistributes it: this holds with a small surface [Péclet number](../../../../../peclet-number.md), fast exchange, or sufficiently immobilized surface [velocity](../../../../../velocity.md). These same conditions justify neglecting the perturbation's advection. Small [capillary number](../../../../../capillary-number.md) and sufficiently small buoyancy-induced shape distortion are separate requirements for a spherical interface.

Take $+$ to mean the outer liquid, $-$ the bubble interior and $n$ outward from the bubble. The general [interfacial stress balance with variable surface tension](../../../../../interfacial-stress-balance-with-variable-surface-tension.md) is

$$
\boxed{(\sigma^+-\sigma^-)n=\gamma\kappa n-\nabla_s\gamma,\qquad \kappa=\nabla_s\cdot n.}
$$

For $\gamma=\gamma_0-\gamma_1C'$, its tangential part is $-\nabla_s\gamma=\gamma_1 B I_sU/a$. Thus the requested form is

$$
\boxed{[I_s\sigma n]^+_-=\frac{6\mu A\lambda}{a}I_sU,\qquad
\lambda=\frac{\gamma_1C_0a}{3\mu(ka^2+2D_s)}.}
$$

This positive parameter measures the strength of the restoring [Marangoni stress](../../../../../marangoni-effect.md) relative to viscous [stress](../../../../../stress.md), including the relaxation of concentration by diffusion and exchange.

The far [velocity](../../../../../velocity.md) $-U$ is produced by the constant harmonic vector potential $\Phi=U$. The two independent decaying degree-one modes are the force-carrying vector potential $\alpha aU/r$ and the scalar dipole $\chi=\beta a^3U\cdot\nabla(1/r)$. They are harmonic outside the bubble and have precisely the symmetry of uniform translation. The [Unscaled Papkovich–Neuber representation](../../../../../unscaled-papkovich-neuber-representation.md) gives, at arbitrary radius,

$$
u=-\left(1+\frac{\alpha a}{r}+\frac{\beta a^3}{r^3}\right)U
+\left(-\frac{\alpha a}{r}+\frac{3\beta a^3}{r^3}\right)(U\cdot n)n,
\qquad p=-\frac{2\mu\alpha a}{r^2}U\cdot n.
$$

The [velocity](../../../../../velocity.md) at $r=a$ agrees with the printed expression. However, the original PDF's [traction](../../../../../traction.md) formula has a factor-of-two error. Direct differentiation with $\sigma=-pI+\mu(\nabla u+\nabla u^T)$ gives

$$
\boxed{\sigma n=\frac{6\mu}{a}\{\beta U+(\alpha-3\beta)(U\cdot n)n\},}
$$

not the printed prefactor $12\mu/a$. This is [traction of translating-sphere Papkovich–Neuber potentials](../../../../../traction-of-translating-sphere-papkovich-neuber-potentials.md). The $\alpha$ term follows immediately from the [Stokeslet](../../../../../stokeslet.md) [stress](../../../../../stress.md), and the scalar-potential part gives $6\mu\beta[U-3(U\cdot n)n]/a$; neither contribution contains the extra factor two.

With this consistent [traction](../../../../../traction.md), no penetration requires $\beta-\alpha=1/2$, tangential [velocity](../../../../../velocity.md) requires $A=-(1+\alpha+\beta)$, and tangential [stress](../../../../../stress.md) balance requires $\beta=A\lambda$. Solving,

$$
\boxed{A=-\frac1{2(1+2\lambda)},\qquad
\beta=-\frac{\lambda}{2(1+2\lambda)},\qquad
\alpha=-\frac{1+3\lambda}{2(1+2\lambda)}.}
$$

For comparison, taking the printed $12\mu/a$ literally would instead give

$$
A_{\rm printed}=-\frac1{2(1+\lambda)},\qquad
\beta_{\rm printed}=-\frac{\lambda}{4(1+\lambda)},\qquad
\alpha_{\rm printed}=-\frac{2+3\lambda}{4(1+\lambda)}.
$$

Those solve the supplied algebraic pair but not the Newtonian [stress](../../../../../stress.md) calculated from the supplied potentials. The factor-six result is the physically consistent [translating surfactant-coated bubble](../../../../../translating-surfactant-coated-bubble.md) solution.

As $\lambda\to0$, $A\to-1/2$ and $\beta\to0$: **the clean bubble has a mobile interface and zero tangential [traction](../../../../../traction.md)**. As $\lambda\to\infty$, $A\to0$, $\alpha\to-3/4$ and $\beta\to-1/4$: **the interface becomes immobilized and the exterior flow approaches that past a no-slip rigid sphere**. The limiting tangential [traction](../../../../../traction.md) is $-3\mu I_sU/(2a)$, a useful check on the correct normalization.

The normal dynamic [traction](../../../../../traction.md) is

$$
n\cdot\sigma n=\frac{6\mu}{a}(\alpha-2\beta)U\cdot n
=-\frac{3\mu(1+\lambda)}{a(1+2\lambda)}U\cdot n,
$$

apart from an arbitrary constant [pressure](../../../../../pressure.md). In the [normal stress balance on a translating bubble](../../../../../normal-stress-balance-on-a-translating-bubble.md), its degree-one part is balanced by the buoyant [hydrostatic pressure](../../../../../hydrostatic-pressure.md) difference and by the variation $-2\gamma_1C'/a$ of normal capillary [stress](../../../../../stress.md). A uniform internal gas [pressure](../../../../../pressure.md) balances the constant Laplace-pressure term but cannot by itself balance this angular variation. If $U$ is upwards and $\Delta\rho$ is liquid minus bubble [mass density](../../../../../density.md), the degree-one balance can be written

$$
n\cdot\sigma_{\rm dyn}n+\Delta\rho g a\,n_z=-\frac{2\gamma_1 B}{a}U n_z.
$$

It fixes $U=\Delta\rho g a^2(1+2\lambda)/[3\mu(1+3\lambda)]$, tending to the clean-bubble and rigid-sphere rise speeds. A degree-one radial displacement translates a sphere rather than changing its curvature, so a supposed dipolar shape distortion cannot replace this [force](../../../../../force.md) balance.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 78](../../paper-78-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
