<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The constitutive convolution is the response of a [linear viscoelastic fluid](../../../../../linear-viscoelastic-fluid.md) close to its relaxed state. Deformations and rotations during the material's memory time must be small, so the [stress](../../../../../stress.md) is linear in the deformation history and evaluating that history at a fixed position is consistent with linearization about rest. For an isotropic [incompressible flow](../../../../../incompressible-flow.md), the [deviatoric stress](../../../../../deviatoric-stress.md) is proportional to the history of the [rate-of-strain tensor](../../../../../strain-rate-tensor.md); an arbitrary isotropic [pressure](../../../../../pressure.md) is separate. Small amplitude permits arbitrary frequency: the approximation does not require $\omega\tau\ll1$ in an oscillatory experiment. Large accumulated deformation, substantial advection of memory, and nonlinear [normal-stress differences](../../../../../normal-stress-difference.md) are outside this formula's scope.

If a small step of strain $\varepsilon_0$ is imposed at time zero and then held, $E(t)=\varepsilon_0\delta(t)$ to linear order. The convolution consequently gives $\sigma'(t)=2G(t)\varepsilon_0$ for $t>0$. In [simple shear flow](../../../../../simple-shear-flow.md), this reads $\sigma_{xy}(t)=G(t)\gamma_0$ for a shear-strain step $\gamma_0$. Thus **$G(t)$ is the remaining shear stress per unit imposed step of shear strain**, which explains the name [relaxation modulus](../../../../../relaxation-modulus.md) and directly describes [stress relaxation](../../../../../stress-relaxation.md).

Use the convention $E(t)=\operatorname{Re}[\widehat E e^{i\omega t}]$. Substitution into the convolution defines the [complex viscosity](../../../../../complex-viscosity.md):

$$
\widehat\sigma'=2\widehat\mu(\omega)\widehat E,\qquad
\boxed{\widehat\mu(\omega)=\int_0^\infty G(s)e^{-i\omega s}\,ds.}
$$

Write $\widehat\mu=\mu'-i\mu''$. Its real part $\mu'$ multiplies the component in phase with the [rate-of-strain tensor](../../../../../strain-rate-tensor.md), causing dissipation; its imaginary part describes the out-of-phase, elastic response. More precisely the complex shear modulus is $G^*=i\omega\widehat\mu$, so the [storage modulus](../../../../../storage-modulus.md) and [loss modulus](../../../../../loss-modulus.md) are

$$
G'=\omega\mu''=-\omega\operatorname{Im}\widehat\mu,\qquad G''=\omega\mu'=\omega\operatorname{Re}\widehat\mu.
$$

For shear-rate amplitude $\widehat{\dot\gamma}$ the mean dissipated power per unit volume is $\tfrac12\mu'|\widehat{\dot\gamma}|^2$. For the exponential [Maxwell fluid](../../../../../linear-maxwell-fluid.md) memory kernel, direct integration gives

$$
\boxed{\widehat\mu=\frac{G_0\tau}{1+i\omega\tau},\quad
\mu'=\frac{G_0\tau}{1+\omega^2\tau^2},\quad
\mu''=\frac{G_0\omega\tau^2}{1+\omega^2\tau^2}.}
$$

The [zero-shear viscosity](../../../../../zero-shear-viscosity.md) is $\mu_0=G_0\tau$, and the high-frequency [storage modulus](../../../../../storage-modulus.md) tends to $G_0$.

For the channel, let $v_x(y,t)=\operatorname{Re}[U(y)e^{i\omega t}]$ and interpret $\Delta p$ as the signed amplitude of $\partial_xp$, not the positive pressure drop. The [Cauchy momentum equation](../../../../../cauchy-momentum-equation.md) and [no-slip boundary conditions](../../../../../no-slip-boundary-condition.md) give

$$
i\omega\rho U=-\Delta p+\widehat\mu U'',\qquad U(\pm h)=0.
$$

Define $k^2=i\omega\rho/\widehat\mu$ and $z=kh$, choosing either square-root branch consistently; the flux expression is even in $z$. The symmetric solution is

$$
U(y)=-\frac{\Delta p}{i\omega\rho}\left[1-\frac{\cosh(ky)}{\cosh(kh)}\right].
$$

Its integral across the channel gives the [oscillatory channel flux of a linear Maxwell fluid](../../../../../oscillatory-channel-flux-of-a-linear-maxwell-fluid.md):

$$
\boxed{Q=\int_{-h}^h U(y)\,dy=-\frac{2\Delta p h}{i\omega\rho}\left(1-\frac{\tanh z}{z}\right),\qquad
z^2=\frac{i\omega\rho h^2(1+i\omega\tau)}{G_0\tau}.}
$$

This includes inertia while using the linear constitutive response. The pressure-gradient amplitude must be small enough that the resulting deformation stays in that response regime.

As $\omega\to0$, $\tanh z/z=1-z^2/3+2z^4/15+\cdots$. Hence

$$
Q=-\frac{2\Delta p h^3}{3\widehat\mu}\left[1-\frac25z^2+O(z^4)\right]
=-\frac{2\Delta p h^3}{3\mu_0}\left[1+i\omega\left(\tau-\frac{2\rho h^2}{5\mu_0}\right)+O(\omega^2)\right].
$$

In particular **$Q\to-2\Delta p h^3/(3G_0\tau)$**, the usual [plane Poiseuille flow](../../../../../plane-poiseuille-flow.md) flux with viscosity $\mu_0$. The fluid has enough time to relax and behaves as a [Newtonian fluid](../../../../../newtonian-fluid.md) at leading order.

For fixed positive $h,\tau,\rho,G_0$, let $c=\sqrt{G_0/\rho}$. At large frequency the square root with positive real part satisfies

$$
z=\frac{h}{2c\tau}+i\frac{\omega h}{c}+O(\omega^{-1}).
$$

Its real part tends to a positive constant, so $\tanh z$ remains bounded although it oscillates. Thus $\tanh z/z=O(\omega^{-1})$ and

$$
\boxed{Q=-\frac{2\Delta p h}{i\omega\rho}[1+O(\omega^{-1})]\qquad(\omega\to\infty).}
$$

The leading volume-integrated response is an inertial balance and is in quadrature with the driving force $-\Delta p$. It is not necessary for the local profile to be a nearly uniform plug: the [Maxwell fluid](../../../../../linear-maxwell-fluid.md) is elastic at these frequencies, and shear waves with speed $c$ can cross the gap. The oscillatory part of $U$ largely cancels on integration. Small attenuation allows resonance-like enhancements at finite frequencies; the leading flux limit still holds for fixed nonzero relaxation and gap parameters. A Newtonian thin viscous-layer argument would not justify the Maxwell profile here.

Finally take the different ordering $\omega\tau\gg1$ but $\rho\omega^2h^2/G_0\ll1$. Now $z^2=-\rho\omega^2h^2/G_0+i\rho\omega h^2/(G_0\tau)$ is small, so the small-$z$ expansion remains appropriate even at a large [Deborah number](../../../../../deborah-number.md). The result is

$$
Q\simeq-\frac{2\Delta p h^3(1+i\omega\tau)}{3G_0\tau},\qquad
\boxed{Q\sim-\frac{2i\omega\Delta p h^3}{3G_0}.}
$$

Here inertia is negligible throughout the narrow gap. Dividing the [velocity](../../../../../velocity.md) by $i\omega$ gives the displacement amplitude, whose parabolic profile is determined by an elastic shear balance with modulus $G_0$. The velocity therefore grows like frequency for a fixed displacement response. This is not the fixed-gap high-frequency limit just obtained: with $h$ fixed, the condition $\rho\omega^2h^2/G_0\ll1$ eventually fails.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 49](../../paper-49-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
