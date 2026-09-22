<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the growing adiabatic mode in an epoch of constant $w$, the superhorizon potential is constant. The [Friedmann equation](../../../../../../friedmann-equations.md) gives $4\pi Ga^2(\bar\rho+\bar P)=\tfrac32(1+w)\mathcal H^2$, so the given relation implies

$$
\mathcal R=-\frac{5+3w}{3(1+w)}\phi.
$$

Thus $\phi_{\rm rad}=-2\mathcal R/3$ and $\phi_{\rm mat}=-3\mathcal R/5$. Photon continuity, neglecting its gradient term on [superhorizon scales](../../../../../../superhorizon-scale.md), gives $(\Theta_0-\phi)'=0$. The radiation-era initial condition fixes $\Theta_0-\phi=\mathcal R$. Through the matter-radiation transition it follows that $\Theta_{0*}=\mathcal R+\phi_{\rm mat}=2\mathcal R/5$. Since $\psi=\phi$, **the matched large-scale emission perturbation is**

$$
\boxed{(\Theta_0+\psi)_*=\frac{2\mathcal R}5-\frac{3\mathcal R}5=-\frac{\mathcal R}5.}
$$

Keeping the radiation value of $\Theta_0$ unchanged across the transition would give the wrong coefficient. This is the [Sachs-Wolfe radiation-to-matter matching](../../../../../../sachs-wolfe-radiation-to-matter-matching.md) for the paper's sign convention for [comoving curvature perturbation](../../../../../../comoving-curvature-perturbation.md).

Neglect the [Integrated Sachs-Wolfe effect](../../../../../../integrated-sachs-wolfe-effect.md), the superhorizon-suppressed Doppler term, observer monopole, and any observer kinematic dipole. Put $\mathbf x_0=0$ by [statistical homogeneity](../../../../../../statistical-homogeneity.md), and define

$$
\langle\mathcal R(\mathbf k)\mathcal R^*(\mathbf k')\rangle
=(2\pi)^3\delta^{(3)}(\mathbf k-\mathbf k')\frac{2\pi^2}{k^3}\mathcal P_{\mathcal R}(k).
$$

The plane-wave expansion on $\mathbf x_*=-\chi_*\mathbf e$ gives angular multipoles

$$
a_{\ell m}=-\frac{4\pi}5(-i)^\ell\int\frac{d^3k}{(2\pi)^3}
\mathcal R(\mathbf k)j_\ell(k\chi_*)Y_{\ell m}^*(\hat{\mathbf k}).
$$

[Statistical isotropy](../../../../../../statistical-isotropy.md) and orthonormal [spherical harmonics](../../../../../../spherical-harmonic.md) then imply $\langle a_{\ell m}a_{\ell'm'}^*\rangle=\delta_{\ell\ell'}\delta_{mm'}C_\ell$. Radial integration supplies $(4\pi)^2(2\pi^2)/(2\pi)^3=4\pi$, giving **the large-angle angular power spectrum**

$$
\boxed{C_\ell\simeq\frac{4\pi}{25}\int d\ln k\,\mathcal P_{\mathcal R}(k)j_\ell^2(k\chi_*).}
$$

This assumes adiabatic growing modes, [matter domination](../../../../../../matter-domination.md) at emission, negligible anisotropic stress, and wavenumbers that are outside the [Hubble radius](../../../../../../hubble-radius.md) then. It treats recombination as instantaneous, omits late potential evolution and rescattering, and omits lensing at this linear order. The formal primordial contribution is defined for $\ell>0$; the observed dipole has a large additional kinematic contribution, so the clean large-angle primordial comparison is usually $\ell\ge2$. A scale-invariant spectrum also yields the Sachs-Wolfe plateau $\ell(\ell+1)C_\ell=2\pi\mathcal P_{\mathcal R}/25$ for $\ell\ge1$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 55](../../../paper-55-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
