<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $b=-g\rho'/\rho_0$ be the buoyancy perturbation and $p$ the pressure perturbation divided by $\rho_0$. For stable stratification, $N>0$. The nonrotating [Linearized Boussinesq equations](../../../../../linearized-boussinesq-equations.md) are

$$
u_t=-p_x,\qquad w_t=-p_z+b,\qquad b_t+N^2w=0,\qquad u_x+w_z=0.
$$

Eliminating $u,p,b$ gives $(\partial_x^2+\partial_z^2)w_{tt}+N^2w_{xx}=0$. Since $w=\zeta_t$, a nonzero-frequency plane wave obeys the same equation for its displacement. Substituting its phase yields the [dispersion relation](../../../../../dispersion-relation.md) for a [plane internal gravity wave](../../../../../plane-internal-gravity-wave.md):

$$
\boxed{\Omega^2=\frac{N^2k^2}{k^2+m^2}.}
$$

Thus the frequency depends on the [wavevector](../../../../../wavevector.md) direction rather than its magnitude.

Advection of the background density gives $\rho'=-\zeta\,\bar\rho_z$ to first order. With constant $\bar\rho_z<0$, the instantaneous density gradient is $\rho_z=\bar\rho_z(1-\zeta_z)$. A region has [unstable density stratification](../../../../../unstable-density-stratification.md) when this becomes positive, namely when $\zeta_z>1$. The maximum of $\zeta_z$ is $|mA_\zeta|$, so the [monochromatic internal-wave overturning criterion](../../../../../monochromatic-internal-wave-overturning-criterion.md) is

$$
\boxed{|mA_\zeta|>1.}
$$

Equality gives a locally vanishing gradient. This is the prediction of the displacement field extrapolated to overturning; the small-amplitude approximation itself ceases to be reliable there.

For the rising packet, distinguish its conserved [absolute frequency](../../../../../absolute-frequency.md) $\omega$ from its actual [intrinsic frequency](../../../../../intrinsic-frequency.md) $\sigma=\omega-kU(z)$. The printed terminology calls $\omega$ intrinsic while also assigning it to a stationary observer; the stationary-observer interpretation is the one consistent with the displayed Doppler shift. On the positive-frequency branch, the ray Hamiltonian is

$$
\omega(z,k,m)=kU(z)+\sigma(k,m),\qquad \sigma=\frac{Nk}{\sqrt{k^2+m^2}}.
$$

The [Hamiltonian ray-tracing equations](../../../../../hamiltonian-ray-tracing-equations.md) give

$$
\dot x=\partial_k\omega,\quad \dot z=\partial_m\omega,\quad
\dot k=-\partial_x\omega=0,\quad \dot m=-\partial_z\omega=-ks,\quad
\frac{d\omega}{dt}=\partial_t\omega=0.
$$

The last identity follows also by differentiating the Hamiltonian along its canonical trajectory: the spatial and [wavevector](../../../../../wavevector.md) terms cancel in pairs. Thus [absolute-frequency conservation in steady shear](../../../../../absolute-frequency-conservation-in-steady-shear.md) gives constant $k$, constant $\omega$, and constant stationary-observer horizontal phase speed $c_x=\omega/k$. In contrast, $\sigma=\omega-ksz$ decreases as the packet rises. At its initial height,

$$
\omega=\frac{Nk}{\sqrt{k^2+m_0^2}},\qquad
\boxed{z_c=\frac{\omega}{ks}=\frac{N}{s\sqrt{k^2+m_0^2}}.}
$$

This is the [critical level of an internal gravity wave](../../../../../critical-level-of-an-internal-gravity-wave.md). In fact $m(t)=m_0-kst$ and $z(t)=[\omega-\sigma(k,m(t))]/(ks)$, so the inviscid ray approaches $z_c$ as $t\to\infty$, rather than reaching it at a finite time.

Write $\theta=|\Theta|=\arctan(|m|/k)$, so $\sigma=N\cos\theta$ with $0<\theta<\pi/2$. The intrinsic [internal-wave phase and group velocity](../../../../../internal-wave-phase-and-group-velocity.md) calculation gives

$$
c_{gx}=\frac{Nm^2}{(k^2+m^2)^{3/2}}=\frac Nk\sin^2\theta\cos\theta,\qquad
c_{gz}=-\frac{Nkm}{(k^2+m^2)^{3/2}}=\frac Nk\sin\theta\cos^2\theta>0.
$$

The observer-frame horizontal ray velocity is $U+c_{gx}$. Dividing it by $c_{gz}$ proves the [internal-wave ray in uniform vertical shear](../../../../../internal-wave-ray-in-uniform-vertical-shear.md):

$$
\boxed{\frac{dx}{dz}=\tan\theta+\frac{ksz}{N\sin\theta\cos^2\theta},\qquad
\tan^2\theta=\frac{N^2}{(\omega-ksz)^2}-1.}
$$

The angle increases toward $\pi/2$ and the vertical group speed tends to zero near the [critical level](../../../../../critical-level-of-a-shear-flow-wave.md).

The [wave-action conservation law](../../../../../wave-action-conservation-law.md) fixes the prescribed upward flux. For a nonzero packet, $B>0$, and the given flux relation implies

$$
A_\zeta^2=\frac{B\sigma}{N^2c_{gz}}=
\frac{Bk\sigma}{N^3\sin\theta\cos^2\theta}.
$$

Apply the [monochromatic internal-wave overturning criterion](../../../../../monochromatic-internal-wave-overturning-criterion.md), using $|m|=k\tan\theta$. After multiplying by the positive trigonometric factors, the exact instability condition is

$$
\boxed{\cot^4\theta<\frac{Bk^3\sigma}{N^3\sin^3\theta}.}
$$

At marginal overturning near a [critical level](../../../../../critical-level-of-a-shear-flow-wave.md), $\sin\theta\simeq1$, so the [wave-action criterion for critical-level overturning](../../../../../wave-action-criterion-for-critical-level-overturning.md) gives

$$
\cot\theta\sim\left(\frac{Bk^3}{N^3}\right)^{1/4}(\omega-ksz)^{1/4}.
$$

With fixed $B,k,N$, this is the requested quarter-power order estimate; the prefactor supplies the dimensions suppressed in that notation. It is an onset balance, not a replacement for $\cos\theta=\sigma/N$. Combining the two relations instead gives $\cos^3\theta=(Bk^3/N^2)\sin\theta$ at onset. Since $m^2A_\zeta^2$ diverges as $\sigma^{-3}$ toward $z_c$, any nonzero packet flux eventually violates the linear overturning criterion before reaching that level, within this nondissipative ray model.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 70](../../paper-70-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
