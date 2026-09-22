<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $\mathbf n$ point from fluid $-$ to fluid $+$, $P_s=I-\mathbf n\mathbf n$, $\nabla_s=P_s\nabla$, and $\mathcal K=\nabla_s\cdot\mathbf n$. A clean material interface without phase change has continuous [velocity](../../../../../velocity.md), with normal interface speed $V_n=\mathbf u_\pm\cdot\mathbf n$. Its surface stress is $\gamma P_s$. The [surface divergence](../../../../../surface-divergence.md) of that tensor is $\nabla_s\gamma-\gamma\mathcal K\mathbf n$. Balancing forces on a small interfacial patch therefore gives the [interfacial stress balance with variable surface tension](../../../../../interfacial-stress-balance-with-variable-surface-tension.md)

$$
\boxed{(\boldsymbol\sigma_+-\boldsymbol\sigma_-)\mathbf n
=\gamma\mathcal K\mathbf n-\nabla_s\gamma,\qquad
\boldsymbol\sigma_\pm=-p_\pm I+\mu_\pm(\nabla\mathbf u_\pm+\nabla\mathbf u_\pm^{T}).}
$$

The normal condition is $\mathbf n\cdot(\boldsymbol\sigma_+-\boldsymbol\sigma_-)\mathbf n=\gamma\mathcal K$; the tangential condition is $P_s(\boldsymbol\sigma_+-\boldsymbol\sigma_-)\mathbf n=-\nabla_s\gamma$. On a stationary [sphere](../../../../../sphere.md) with outward normal these reduce to $p_--p_+=2\gamma/a$ when viscous normal stresses vanish. This fixes the sign convention for the [Marangoni stress](../../../../../marangoni-effect.md) rather than leaving the direction ambiguous.

For the bubble take negligible internal [dynamic viscosity](../../../../../dynamic-viscosity.md), no contaminants, and initially the standard effectively insulating gas-bubble approximation. With heat advection neglected, the exterior [temperature](../../../../../temperature.md) satisfies [Laplace's equation](../../../../../laplace-equation.md), approaches $T_0+\mathbf H\cdot\mathbf r$ remotely, and has zero normal heat flux at $r=a$. The [temperature dipole around an insulating sphere](../../../../../temperature-dipole-around-an-insulating-sphere.md) gives

$$
T=T_0+(\mathbf H\cdot\mathbf r)\left(1+\frac{a^3}{2r^3}\right),\qquad
T_s=T_0+\frac32a\mathbf H\cdot\mathbf n.
$$

The zero-flux condition follows by differentiating the radial factor. Let $\gamma_T=(d\gamma/dT)_{T_0}$. To first order in the weak gradient,

$$
\gamma_s=\gamma_0+\frac32a\gamma_T\mathbf H\cdot\mathbf n,\qquad
\nabla_s\gamma_s=\frac32\gamma_TP_s\mathbf H.
$$

In the laboratory frame the force-free bubble can be described by the harmonic [Papkovich–Neuber representation](../../../../../papkovich-neuber-representation.md) potentials

$$
\boldsymbol\Phi=0,\qquad \chi=-\frac{a^3\mathbf U\cdot\mathbf r}{2r^3}.
$$

They give constant exterior [pressure](../../../../../pressure.md) and the decaying [source dipole](../../../../../source-dipole.md) field

$$
\mathbf u=-\frac{a^3}{2r^3}[\mathbf U-3(\mathbf U\cdot\widehat{\mathbf r})\widehat{\mathbf r}].
$$

At the surface $\mathbf u\cdot\mathbf n=\mathbf U\cdot\mathbf n$, so the normal [kinematic boundary condition](../../../../../kinematic-boundary-condition.md) holds for translation. In coordinates aligned with $\mathbf U$, $u_r=a^3U\cos\theta/r^3$ and $u_\theta=a^3U\sin\theta/(2r^3)$. Direct differentiation gives

$$
\sigma_{r\theta}=\mu\left(\partial_ru_\theta-u_\theta/r+r^{-1}\partial_\theta u_r\right)
=-3\mu a^3U\sin\theta/r^4.
$$

Equivalently, the surface tangential [traction](../../../../../traction.md) is $(3\mu/a)P_s\mathbf U$. The tangential stress condition therefore requires

$$
\frac{3\mu}{a}P_s\mathbf U=-\frac32\gamma_TP_s\mathbf H,
\qquad\boxed{\mathbf U=-\frac{a\gamma_T}{2\mu}\mathbf H.}
$$

For the usual negative $\gamma_T$, the bubble moves toward hotter liquid. The normal condition is consistent as well: its viscous dipole is $-6\mu\mathbf U\cdot\mathbf n/a=3\gamma_T\mathbf H\cdot\mathbf n$, exactly the dipolar part of $2\gamma_s/a$. The constant part fixes $p_{\rm gas}-p_\infty=2\gamma_0/a$. There is no [Stokeslet](../../../../../stokeslet.md) term, hence no net applied [force](../../../../../force.md) or drag imbalance.

The thermal assumption matters. The problem gives the exterior [thermal diffusivity](../../../../../thermal-diffusivity.md) but no gas [thermal conductivity](../../../../../thermal-conductivity.md). For an inviscid bubble with conductivity ratio $K=k_{\rm gas}/k_{\rm liquid}$, temperature and normal heat-flux continuity instead give

$$
T_{\rm out}=T_0+(\mathbf H\cdot\mathbf r)\left[1+\frac{1-K}{2+K}\frac{a^3}{r^3}\right],\qquad
T_s=T_0+\frac3{2+K}a\mathbf H\cdot\mathbf n,
$$

so the same stress calculation gives

$$
\boxed{\mathbf U=-\frac{a\gamma_T}{\mu(2+K)}\mathbf H.}
$$

The insulating-bubble result uses $K\ll1$. If instead an undisturbed surface temperature gradient is imposed, corresponding to $K=1$, the coefficient is $1/3$ rather than $1/2$. Exterior [thermal diffusivity](../../../../../thermal-diffusivity.md) alone does not select between those thermal boundary conditions. This dependence is explicit rather than silently treating a missing gas property as a prescribed value.

The small parameters can now be stated precisely. With $U_*=a|\gamma_T||\mathbf H|/(2\mu)$ and $\nu=\mu/\rho$, require

$$
\boxed{\mathrm{Re}=U_*a/\nu\ll1,\qquad
\mathrm{Pe}=U_*a/\kappa\ll1,\qquad
\mathrm{Ca}=\mu U_*/\gamma_0\ll1,\qquad
\frac{a|\gamma_T||\mathbf H|}{\gamma_0}\ll1.}
$$

Small [Reynolds number](../../../../../reynolds-number.md) justifies [Stokes flow](../../../../../stokes-flow-split.md); small [Péclet number](../../../../../peclet-number.md) allows quasi-static [heat conduction](../../../../../thermal-conduction.md) without advective distortion; small [capillary number](../../../../../capillary-number.md) and fractional surface-tension variation support a nearly spherical interface and a weak perturbation of its base [surface tension](../../../../../surface-tension.md). These last two conditions are proportional for this velocity scale but describe different approximations. Linearizing $\gamma(T)$ also needs $a|\mathbf H||\gamma_{TT}/\gamma_T|\ll1$ if its derivative varies appreciably. Negligible internal viscosity and the insulating specialization require the corresponding gas-to-liquid viscosity and conductivity ratios to be small. Gravity has been excluded; if restored, its buoyancy-induced migration must be small compared with $U_*$, not merely small enough to avoid deformation.

Finally, [surfactants](../../../../../surfactant.md) change both the constitutive surface tension and the surface stress dynamics. The surface flow driven by the thermal [Marangoni effect](../../../../../marangoni-effect.md) carries insoluble surfactant toward the high-tension side, lowering its tension and producing an opposing concentration-driven gradient. When surface diffusion or exchange is slow, this tends to immobilize the interface, suppressing the clean-bubble [thermocapillary migration of an insulating bubble](../../../../../thermocapillary-migration-of-an-insulating-bubble.md), sometimes nearly stopping it. If the surfactant stays uniformly equilibrated, it can instead change $\gamma_T$ without a large opposing gradient. Its concentration, surface diffusivity and adsorption kinetics must be supplied to compute a replacement speed; no universal numerical reduction factor follows merely from its presence.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 73](../../paper-73-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
