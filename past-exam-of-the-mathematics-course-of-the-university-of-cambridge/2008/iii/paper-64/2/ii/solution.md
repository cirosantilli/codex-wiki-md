<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

In the [tight-coupling approximation](../../../../../../tight-coupling-approximation.md), repeated [Thomson scattering](../../../../../../thomson-scattering.md) drives the photon distribution toward isotropy in the local baryon rest frame. At linear order a temperature perturbation gives a monopole and a small boost gives only a dipole. A photon propagating along $\mathbf n$ has rest-frame energy $p(1-\mathbf n\cdot\mathbf v)$, so

$$
f_1=-qf_0'(q)\left(\Theta_{\rm rest}+\mathbf n\cdot\mathbf v\right).
$$

Since the rest-frame [density contrast](../../../../../../density-contrast.md) is $\delta_\gamma=4\Theta_{\rm rest}$, the initial [photon brightness perturbation](../../../../../../photon-brightness-perturbation.md) is

$$
\boxed{\Delta_*=\delta_{\gamma *}+4\mathbf n\cdot\mathbf v_*.}
$$

The quadrupole and higher [photon temperature multipoles](../../../../../../photon-temperature-multipole.md) are small when the conformal collision rate $\kappa=a n_e\sigma_T$ greatly exceeds both $k$ and $\mathcal H$. For example the quadrupole is suppressed by a factor of order $k/\kappa$ relative to the dipole. Instantaneous decoupling idealizes this strongly coupled state as the initial data for collisionless propagation; finite mean free path and polarization corrections are omitted from that initial truncation.

Multiply the [synchronous photon brightness equation](../../../../../../synchronous-photon-brightness-equation.md) by $e^{ik\mu\tau}$ and integrate from $\tau_*$ to $\tau_0$. The [line-of-sight solution for free-streaming photons](../../../../../../line-of-sight-solution-for-free-streaming-photons.md) is

$$
\Delta(\mathbf k,\mathbf n,\tau_0)=e^{-ik\mu(\tau_0-\tau_*)}\Delta_*(\mathbf k,\mathbf n)-2\int_{\tau_*}^{\tau_0}e^{-ik\mu(\tau_0-\tau)}h'_{ij}(\mathbf k,\tau)n^in^j d\tau.
$$

The phase is essential: it specifies the emission point and the points traversed by the ray. In real space define $\mathbf x(\tau)=\mathbf x_0-\mathbf n(\tau_0-\tau)$ and $\mathbf x_*=\mathbf x(\tau_*)$. Dividing by four gives the [synchronous Sachs-Wolfe line-of-sight formula](../../../../../../synchronous-sachs-wolfe-line-of-sight-formula.md),

$$
\boxed{\frac{\Delta T}{T}(\mathbf x_0,\mathbf n,\tau_0)=\frac14\delta_\gamma(\mathbf x_*,\tau_*)+\mathbf n\cdot\mathbf v(\mathbf x_*,\tau_*)-\frac12\int_{\tau_*}^{\tau_0}h'_{ij}(\mathbf x(\tau),\tau)n^in^j d\tau.}
$$

The spatial arguments suppressed in a shorthand version must be understood in this retarded sense; evaluating the emission terms at $\mathbf x_0$ instead would discard free streaming. Here $\mathbf n$ is propagation direction. The observer-to-source direction on the sky is $-\mathbf n$, explaining the opposite Doppler sign often used with that convention. The formula describes the synchronous-frame observer; an additional observer peculiar velocity contributes a dipole.

The first term is the intrinsic temperature perturbation at emission, since $\delta_\gamma=4\Theta$. The second is the [Doppler CMB anisotropy](../../../../../../doppler-cmb-anisotropy.md) from the plasma bulk velocity. The third is gravitational frequency shifting by the time-dependent spatial metric along the ray, and can include scalar and tensor metric contributions. In scalar [Newtonian gauge](../../../../../../newtonian-gauge.md), rearranging that metric contribution supplies the emission gravitational potential as well as the [Integrated Sachs-Wolfe effect](../../../../../../integrated-sachs-wolfe-effect.md), up to the observer terms. It should not be identified solely with the integrated Sachs-Wolfe term: a constant Newtonian potential need not give a vanishing synchronous metric integral.

On large angles, modes are outside or comparable to the sound horizon at emission. For the growing [adiabatic mode](../../../../../../adiabatic-mode.md) during matter domination, the intrinsic and emission-potential contributions give the ordinary [Sachs-Wolfe effect](../../../../../../sachs-wolfe-effect.md), $\Theta_0+\Psi=\Psi/3$ in Newtonian variables. Velocity is a gradient effect, of order $k\tau_*\Psi$ on superhorizon scales, so its Doppler contribution is suppressed there. A scale-invariant primordial curvature spectrum produces approximately the familiar large-angle plateau in $\ell(\ell+1)C_\ell$. Evolving potentials during radiation-to-matter transition or late acceleration can add integrated gravitational anisotropy; constant matter-era scalar potentials do not generate a genuine scalar integrated Sachs-Wolfe source.

On smaller angles, the [photon-baryon fluid](../../../../../../photon-baryon-fluid.md) has undergone acoustic oscillations. Its density and velocity are approximately in cosine and sine phases, producing acoustic structure in the intrinsic and Doppler sources and their projection onto angular multipoles. [Silk damping](../../../../../../cosmic-microwave-background-diffusion-damping.md) suppresses sufficiently short wavelengths before decoupling, while the finite width of last scattering also smooths the real small-angle signal. These corrections refine the instantaneous-decoupling model rather than follow from a collisionless equation alone. The separate intrinsic, velocity and metric pieces depend on gauge convention; the complete observed anisotropy, including the appropriate observer terms and removal of the unobservable mean, is the physical quantity.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
