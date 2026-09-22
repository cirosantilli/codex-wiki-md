<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $\Gamma=-\dot\tau=a\bar n_e\sigma_T$ and let $D=\partial_\eta+\mathbf e\cdot\nabla$ differentiate along the unperturbed photon trajectory. Use $1+(\mathbf e\cdot\hat{\mathbf m})^2=4/3+(2/3)P_2(\mathbf e\cdot\hat{\mathbf m})$ to decompose the [Thomson scattering](../../../../../../thomson-scattering.md) gain term:

$$
\frac{3\Gamma}{16\pi}\int d\hat{\mathbf m}\,\Theta(\hat{\mathbf m})[1+(\mathbf e\cdot\hat{\mathbf m})^2]
=\Gamma[\Theta_0+Q(\mathbf e)],
\quad
Q(\mathbf e)=\frac12\int\frac{d\hat{\mathbf m}}{4\pi}\Theta(\hat{\mathbf m})P_2(\mathbf e\cdot\hat{\mathbf m}).
$$

The [Orthogonality of Legendre polynomials](../../../../../../orthogonality-of-legendre-polynomials.md) identifies $Q$ as a pure [photon quadrupole](../../../../../../photon-quadrupole.md). Dropping $Q$ is an approximation, justified when [tight coupling](../../../../../../tight-coupling-approximation.md) makes the scattering quadrupole small; the supplied unpolarized equation already neglects polarization corrections. The [Cosmic microwave background line-of-sight solution](../../../../../../cosmic-microwave-background-line-of-sight-solution.md) requested here omits that quadrupole source.

Set $Y=\Theta+\psi$. Adding $D\psi=\dot\psi+\mathbf e\cdot\nabla\psi$ to the [Photon Boltzmann equation with Thomson scattering](../../../../../../photon-boltzmann-equation-with-thomson-scattering.md) yields

$$
DY+\Gamma Y\simeq\dot\phi+\dot\psi+\Gamma(\Theta_0+\psi+\mathbf e\cdot\mathbf v_b).
$$

Along $\mathbf x(\eta)=\mathbf x_0-(\eta_0-\eta)\mathbf e$, the integrating factor is $e^{-\tau}$ because $d e^{-\tau}/d\eta=\Gamma e^{-\tau}$. Consequently

$$
\frac{d}{d\eta}[e^{-\tau}Y(\eta,\mathbf x(\eta),\mathbf e)]
\simeq e^{-\tau}(\dot\phi+\dot\psi)+g(\Theta_0+\psi+\mathbf e\cdot\mathbf v_b).
$$

An early optically thick boundary makes $e^{-\tau}Y$ vanish for finite initial perturbations, and $e^{-\tau(\eta_0)}=1$. Therefore

$$
\boxed{\begin{aligned}
\Theta(\eta_0,\mathbf x_0,\mathbf e)+\psi(\eta_0,\mathbf x_0)
&\simeq\int_{\eta_i}^{\eta_0}g(\eta)(\Theta_0+\psi+\mathbf e\cdot\mathbf v_b)(\eta,\mathbf x_0-\chi\mathbf e)d\eta\\
&\quad+\int_{\eta_i}^{\eta_0}e^{-\tau}(\dot\phi+\dot\psi)(\eta,\mathbf x_0-\chi\mathbf e)d\eta,
\end{aligned}}\qquad\chi=\eta_0-\eta.
$$

Here $\dot\phi$ and $\dot\psi$ are partial time derivatives, not total derivatives along the ray. We work at first order in [scalar cosmological perturbations](../../../../../../scalar-cosmological-perturbation.md), evaluate sources along the background [radial null geodesic in FLRW spacetime](../../../../../../radial-null-geodesic-in-flrw-spacetime.md), and ignore observer peculiar velocity. Perturbed paths and lensing affect this first-order source solution only at higher perturbative order. A moving observer adds its local Doppler dipole.

The original PDF, unlike the transcribed TeX, also asks for the instantaneous-last-scattering limit and its interpretation. For $g(\eta)=\delta^{(D)}(\eta-\eta_*)$ with no later scattering, and a matter-era growing mode with constant $\phi$ and $\psi$, the [Integrated Sachs-Wolfe effect](../../../../../../integrated-sachs-wolfe-effect.md) vanishes. Hence

$$
\boxed{\Theta_{\rm obs}(\mathbf e)\simeq\Theta_0(\eta_*,\mathbf x_*)+\psi(\eta_*,\mathbf x_*)-\psi(\eta_0,\mathbf x_0)
+\mathbf e\cdot\mathbf v_b(\eta_*,\mathbf x_*),\quad\mathbf x_*=\mathbf x_0-\chi_*\mathbf e}.
$$

The four terms are the intrinsic emission temperature, the gravitational potential at emission, the observer's potential, and the [Doppler CMB anisotropy](../../../../../../doppler-cmb-anisotropy.md). The two potentials describe the gravitational redshift; the observer term is independent of direction and is absorbed into the measured temperature monopole. The intrinsic temperature and emission potential form the [Sachs-Wolfe combination](../../../../../../sachs-wolfe-combination.md). On [superhorizon scales](../../../../../../superhorizon-scale.md) for [adiabatic initial conditions](../../../../../../adiabatic-initial-conditions.md) in [matter domination](../../../../../../matter-domination.md), $\Theta_0=-2\psi/3$, giving the ordinary [Sachs-Wolfe effect](../../../../../../sachs-wolfe-effect.md) $\Theta_0+\psi=\psi/3$. The Doppler sign is positive with the paper's propagation direction $\mathbf e$; the viewing direction is $-\mathbf e$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 312](../../../paper-312-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
