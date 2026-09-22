<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The inequalities are compatible: CDM can dominate the total density while photons dominate baryons. With $R\gg1$, $c_s^2\simeq1/3$ and the baryon-inertia expansion term is negligible. Differentiate photon continuity and substitute the combined Euler equation:

$$
\delta_\gamma''=\frac43k^2\theta_\gamma'
=-\frac{k^2}{3}\delta_\gamma+\frac43k^2\sigma_\gamma.
$$

Thus $\delta_\gamma''+k^2\delta_\gamma/3-4k^2\sigma_\gamma/3=0$. The quasistatic quadrupole equation gives

$$
\sigma_\gamma\simeq-\frac4{15}\tau_c k^2\theta_\gamma
=-\frac15\tau_c\delta_\gamma',\qquad \tau_c=q^{-1}.
$$

Substitution yields the [shear-only photon diffusion damping](../../../../../../shear-only-photon-diffusion-damping.md) equation

$$
\boxed{\delta_\gamma''+\frac4{15}\tau_c k^2\delta_\gamma'+\frac{k^2}{3}\delta_\gamma=0.}
$$

To solve it, put $\Gamma=4k^2\tau_c/15$ and $\delta_\gamma=u\exp[-\tfrac12\int^\tau\Gamma(s)ds]$. Direct differentiation, including both derivatives of the prefactor, gives

$$
u''+\left[\frac{k^2}{3}-\frac{\Gamma'}2-\frac{\Gamma^2}{4}\right]u=0.
$$

Neglect the requested $\tau_c'$ and $\tau_c^2$ terms. The remaining equation is the free acoustic oscillator, so its general solution is

$$
\boxed{\delta_\gamma(\mathbf k,\tau)\simeq
\left[A(\mathbf k)\cos\frac{k\tau}{\sqrt3}+B(\mathbf k)\sin\frac{k\tau}{\sqrt3}\right]
\exp\left[-\frac{k^2}{k_D^2(\tau)}\right],}
$$



$$
\boxed{k_D^{-2}(\tau)=\frac2{15}\int_0^\tau\tau_c(s)\,ds.}
$$

A different lower limit is absorbed into the amplitudes. The damping integral is positive and increases with time: shorter wavelengths are smoothed more strongly by photon diffusion. A subhorizon but still tightly coupled mode satisfies $k\tau\gg1$ and $k\tau_c\ll1$, with slowly varying scattering time; the formula is not valid for arbitrarily short waves after tight coupling fails. The truncated shear coefficient is the one implied by the supplied equations, not the more complete damping coefficient including photon polarization and photon-baryon slip. For constant $\tau_c$, the exact oscillator frequency differs from $k/\sqrt3$ only at order $\tau_c^2$, consistent with this expansion.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
