<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

In the [Boussinesq approximation](../../../../../boussinesq-approximation.md), replace density by a constant reference density $\rho_0$ in inertia and [incompressible flow](../../../../../incompressible-flow.md), retaining the small density departure only in the gravitational force. Write $\rho=\bar\rho(z)+\rho'$ and subtract the resting [hydrostatic pressure](../../../../../hydrostatic-pressure.md). The upward [buoyancy perturbation](../../../../../buoyancy-perturbation.md) acceleration and squared [buoyancy frequency](../../../../../buoyancy-frequency.md) are

$$
\sigma=-\frac{g\rho'}{\rho_0},\qquad N^2(z)=-\frac{g}{\rho_0}\frac{d\bar\rho}{dz}.
$$

Thus stable [density stratification](../../../../../density-stratification.md) has $N^2>0$. Let $p$ henceforth denote the pressure anomaly divided by $\rho_0$. The ideal, nonrotating [Boussinesq equations](../../../../../boussinesq-equations.md) are

$$
\frac{D\mathbf u}{Dt}=-\nabla p+\sigma\mathbf e_z,
\qquad \frac{D\sigma}{Dt}+N^2(z)w=0,
\qquad \nabla\cdot\mathbf u=0,
\qquad \frac D{Dt}=\partial_t+u\partial_x+v\partial_y+w\partial_z.
$$

The [buoyancy](../../../../../buoyancy.md) equation follows by materially conserving the total buoyancy $b_0(z)+\sigma$, where $b_0'=N^2$; it does not assume constant $N$.

For an $x$-periodic flow of period $P$, define $\bar a=P^{-1}\int_0^P a\,dx$. An infinite-domain average with vanishing end contributions works as well. The necessary pressure condition is **no mean zonal pressure gradient**, $\overline{p_x}=0$: periodic pressure satisfies it, whereas a pressure containing a term proportional to $x$ does not. Use [incompressible flow](../../../../../incompressible-flow.md) to write the zonal momentum equation in conservative form,

$$
u_t+(u^2)_x+(uv)_y+(uw)_z=-p_x.
$$

Averaging its zonal derivative terms yields the exact [Reynolds stress](../../../../../reynolds-stress.md) relation

$$
\boxed{\bar u_t=-\partial_y\overline{uv}-\partial_z\overline{uw}.}
$$

For two-dimensional small disturbances about rest, the [Linearized Boussinesq equations](../../../../../linearized-boussinesq-equations.md) are $u_t=-p_x$, $w_t=-p_z+\sigma$, $\sigma_t=-N^2w$, and $u_x+w_z=0$. Differentiate the two momentum equations to eliminate pressure: $(u_z-w_x)_t=-\sigma_x$. Differentiating in $x$ and using $u_{xz}=-w_{zz}$ gives $\nabla^2w_t=\sigma_{xx}$. One further time derivative gives

$$
\boxed{\nabla^2w_{tt}+N^2(z)w_{xx}=0.}
$$

**The equation remains valid for $N=N(z)$.** No vertical derivative of $N$ was taken: $\partial_x^2(N^2w)=N^2w_{xx}$.

For constant $N$ and $k\ne0$, a [plane internal gravity wave](../../../../../plane-internal-gravity-wave.md) has

$$
w=\operatorname{Re}\{a e^{i(kx+mz-\omega t)}\},
\qquad \omega^2(k^2+m^2)=N^2k^2,
\qquad m=\pm |k|\sqrt{N^2/\omega^2-1}.
$$

Both signs give the prescribed lower-boundary velocity. The [radiation condition](../../../../../radiation-condition.md) excludes energy arriving from infinity. At positive frequency, the vertical [group velocity](../../../../../group-velocity.md) is

$$
c_{gz}=\frac{\partial\omega}{\partial m}=-\frac{\omega m}{k^2+m^2}.
$$

For a source below the fluid, energy must propagate upward, so **the outgoing solution has $m<0$**, even though its vertical [phase velocity](../../../../../phase-velocity.md) $\omega/m$ is downward.

To obtain this selection causally, let $T=\mu t$ and $Z=\mu z$, and replace the constant amplitude by $a(Z,T)$. The [method of multiple scales](../../../../../method-of-multiple-scales.md) treats $(z,t,Z,T)$ as independent during differentiation: the carrier derivatives hold $Z,T$ fixed, while $a_T$ holds $Z$ fixed and $a_Z$ holds $T$ fixed. Only after differentiating do we restrict to $T=\mu t$, $Z=\mu z$. Acting on the complex wave, the operators become

$$
\partial_t\longmapsto-i\omega+\mu\partial_T,
\qquad \partial_z\longmapsto im+\mu\partial_Z.
$$

With $K^2=k^2+m^2$, the wave equation has residual

$$
(\omega^2K^2-N^2k^2)a
+2i\mu\{\omega K^2a_T-m\omega^2a_Z\}+O(\mu^2).
$$

The zeroth-order term is the [dispersion relation](../../../../../dispersion-relation.md); the first-order term vanishes precisely when

$$
\boxed{a_T+b a_Z=0,\qquad b=-m\omega/K^2=c_{gz}.}
$$

If $a_0(T)$ is the switched-on boundary amplitude, with $a_0(T)=0$ for $T<0$, the outgoing envelope is $a(Z,T)=a_0(T-Z/b)$ for $b>0$. Its characteristics carry the boundary signal into initially undisturbed fluid. If $b<0$, characteristics instead arrive from the upper half-space; zero initial disturbances and no incoming signal cannot establish the proposed boundary-forced wavetrain. This is the [internal-wave envelope radiation condition](../../../../../internal-wave-envelope-radiation-condition.md).

The leading [incompressible flow](../../../../../incompressible-flow.md) polarization gives $u'=-(m/k)w'$. Hence, to second order in amplitude and leading order in the slow modulation,

$$
\overline{u'w'}=-\frac{m}{2k}|a(Z,T)|^2,
\qquad
\bar u_t=\frac{m}{2k}\partial_z|a|^2
=\frac{\mu m}{2k}\partial_Z|a|^2.
$$

There is no meridional transport here. Envelope transport gives $\partial_t|a|^2=-b\partial_z|a|^2$, so an initially vanishing mean develops as

$$
\boxed{\bar u=-\frac{m}{2kb}|a|^2=\frac{K^2}{2k\omega}|a|^2.}
$$

These are the leading expressions for [internal-wave momentum deposition](../../../../../internal-wave-momentum-deposition.md); higher slow-modulation corrections to the stress are beyond the displayed approximation. In particular, a spatially uniform fully established wavetrain has zero stress divergence, but the front has already produced its mean flow.

The mean wave [energy density](../../../../../energy-density.md) per unit mass follows from $\sigma'=-iN^2w'/\omega$:

$$
\mathcal E=\frac12\overline{u'^2+w'^2+\sigma'^2/N^2}
=\frac{K^2}{2k^2}|a|^2,
\qquad \overline{p'w'}=-\frac{\omega m}{2k^2}|a|^2=b\mathcal E.
$$

Thus $\bar u=(k/\omega)\mathcal E$. In the original frame the mean [kinetic energy](../../../../../kinetic-energy.md) is $\bar u^2/2=O(a^4)$. In a frame translating at $c=\omega/k$, the undisturbed velocity is $-c$, and the change in mean [kinetic energy](../../../../../kinetic-energy.md) is $-c\bar u+O(a^4)=O(a^2)$. Indeed $\mathcal E-c\bar u=0$ at this order behind the front. **Mean-flow energy is therefore essential at the same order as wave energy in the translating frame.** This follows also from the frame transformation of energy, $E\mapsto E-cP$ up to the fixed background constant, and is why [conservation of momentum](../../../../../momentum-conservation.md) cannot be omitted from the moving-frame [conservation of energy](../../../../../conservation-of-energy.md) budget.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 81](../../paper-81-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
