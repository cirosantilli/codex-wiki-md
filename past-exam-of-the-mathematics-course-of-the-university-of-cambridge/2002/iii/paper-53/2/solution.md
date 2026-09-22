<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [simple fluid](../../../../../simple-fluid.md) reduces to a [linear viscoelastic fluid](../../../../../linear-viscoelastic-fluid.md) when its deformation and rotation over the relevant memory interval are small enough to linearize the constitutive history about an isotropic relaxed state. Small amplitude is essential; small frequency is not. For example, arbitrarily high-frequency oscillation can still be linear if its strain amplitude is sufficiently small. The [relaxation modulus](../../../../../relaxation-modulus.md) $G(t)$ is the shear-stress response to a unit small step of shear [strain](../../../../../strain.md).

Choose the harmonic convention $e^{i\omega t}$. If the imposed [shear rate](../../../../../shear-rate.md) is $\operatorname{Re}(\widehat{\dot\gamma}e^{i\omega t})$, the corresponding [shear stress](../../../../../shear-stress.md) is $\operatorname{Re}(\eta^*(\omega)\widehat{\dot\gamma}e^{i\omega t})$. Substitution into the constitutive [convolution](../../../../../convolution.md) gives the [complex viscosity](../../../../../complex-viscosity.md):

$$
\boxed{\eta^*(\omega)=\int_0^\infty G(s)e^{-i\omega s}ds.}
$$

For a nondecaying elastic part this formula is understood through the limit from a positive Laplace damping parameter. The complex shear modulus is $G^*=i\omega\eta^*=G'+iG''$, so $G'$ is the [storage modulus](../../../../../storage-modulus.md), $G''$ the [loss modulus](../../../../../loss-modulus.md), and $\eta^*=G''/\omega-iG'/\omega$ in this convention.

Creep is the progressive deformation produced by a held [stress](../../../../../stress.md). For a small step $S_0H(t)$ of shear stress, define the [creep compliance](../../../../../creep-compliance.md) $J$ by $\gamma(t)=S_0J(t)$ from a relaxed state. Writing hats for [Laplace transforms](../../../../../laplace-transform.md), the same constitutive law gives $\widehat S=p\widehat G\widehat\gamma$. Since $\widehat S=S_0/p$, this yields

$$
\boxed{\widehat J(p)=\frac{1}{p^2\widehat G(p)}.}
$$

Here $H$ is the [Heaviside step function](../../../../../heaviside-step-function.md). Inversion determines the full creep response, including any instantaneous elastic strain jump. Equivalently, the causal relaxation/creep [convolution](../../../../../convolution.md) includes that jump through $\int_{0^-}^tG(t-s)dJ(s)=1$ for $t>0$.

For the [Maxwell fluid](../../../../../linear-maxwell-fluid.md), $\widehat G(p)=G_0/(p+1/\tau)$. Thus the two material responses are

$$
\eta^*(\omega)=\frac{G_0\tau}{1+i\omega\tau},\qquad
J(t)=\frac1{G_0}+\frac{t}{G_0\tau}\quad(t\ge0).
$$

The creep response is an elastic jump followed by constant-rate viscous deformation. The zero-frequency [shear viscosity](../../../../../dynamic-viscosity.md) is $\eta=G_0\tau$.

For the wall problem, take $v=u(y,t)e_x$ and denote the shear component of [stress](../../../../../stress.md) by $S$. The [incompressibility](../../../../../incompressible-flow.md) constraint is satisfied, and the advective part of the [material derivative](../../../../../material-derivative.md) vanishes because no field depends on $x$. With no imposed longitudinal [pressure gradient](../../../../../pressure-gradient.md), [momentum conservation](../../../../../momentum-conservation.md) and the linear Maxwell law give

$$
\rho u_t=S_y,\qquad S_t+\frac S\tau=G_0u_y.
$$

The initial conditions are $u=S=0$ in $y>0$; the [no-slip boundary condition](../../../../../no-slip-boundary-condition.md) is $u(0,t)=UH(t)$, with decay as $y\to\infty$. Transforming these equations gives

$$
\widehat S=\frac{G_0}{p+1/\tau}\widehat u_y,\qquad
\widehat u_{yy}=q(p)^2\widehat u,\qquad
q(p)=\sqrt{\frac{\rho p(1+p\tau)}{G_0\tau}}.
$$

Choose the analytic square-root branch in $\operatorname{Re}p>0$ with $\operatorname{Re}q>0$, so that the spatially increasing solution is excluded. The [Maxwell start-up shear layer](../../../../../maxwell-start-up-shear-layer.md) consequently has

$$
\widehat u(y,p)=\frac Up e^{-q(p)y}.
$$

The [Bromwich inversion formula](../../../../../bromwich-inversion-formula.md) now gives

$$
\boxed{u(y,t)=\frac{U}{2\pi i}\int_{b-i\infty}^{b+i\infty}\frac1p\exp\left[pt-y\sqrt{\frac{\rho p(1+p\tau)}{G_0\tau}}\right]dp,\qquad b>0.}
$$

The vertical [Bromwich contour](../../../../../bromwich-contour.md) is directed upward and lies to the right of all singularities, including the origin and the branch points at $0$ and $-1/\tau$. A cut joining these branch points is a possible continuation into the left half-plane; inversion only requires the stated right-half-plane branch.

The Newtonian limit holds $\eta=G_0\tau$ fixed while $\tau\to0$, so $G_0\to\infty$. Then $q(p)\to\sqrt{\rho p/\eta}$. With $\nu=\eta/\rho$, the inverse [Laplace transform](../../../../../laplace-transform.md) gives the [complementary error function](../../../../../complementary-error-function.md) profile

$$
\boxed{u(y,t)=U\operatorname{erfc}\left(\frac{y}{2\sqrt{\nu t}}\right).}
$$

This is diffusive momentum penetration in a [Newtonian fluid](../../../../../newtonian-fluid.md), with thickness of order $\sqrt{\nu t}$.

The elastic limit instead holds $G_0$ fixed while $\tau\to\infty$. Write $c=\sqrt{G_0/\rho}$. On the chosen branch, $q(p)\to p/c$, so the [Laplace transform time-shift rule](../../../../../laplace-transform-time-shift-rule.md) yields

$$
\boxed{u(y,t)=U H(t-y/c).}
$$

An elastic shear front travels at speed $c$: the material ahead is at rest, while that behind moves at the wall speed. Indeed the limiting displacement is $d(y,t)=U(t-y/c)H(t-y/c)$, whose shear [strain](../../../../../strain.md) is $d_y=-(U/c)H(t-y/c)$. A nonzero pointwise velocity gradient at the front is interpreted distributionally, or by smoothing the ideal wall start.

**The use of linear viscoelasticity is conditional, rather than automatically justified for arbitrary $U$.** The [material derivative](../../../../../material-derivative.md) simplifying to a time derivative does not remove the nonlinear constitutive effects of finite shear [strain](../../../../../strain.md). In this Maxwell problem the rapid elastic response supplies the natural strain scale $U/c=U\sqrt{\rho/G_0}$, which must be small for linearization through start-up. Away from the front, the strain accumulated over an effective memory interval must likewise be small. In the late diffusive regime its characteristic size is $\tau U/\sqrt{\nu t}$, which decreases with time. Large absolute wall displacement $Ut$ alone is not a disqualification for a fluid with finite memory; it is relative deformation during that memory that matters. In the elastic limit, where memory does not decay, the explicit strain behind the front confirms the condition $U/c\ll1$. Without such a small-strain restriction, the computed field is a formal linear response and need not describe an arbitrary [simple fluid](../../../../../simple-fluid.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 53](../../paper-53-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
