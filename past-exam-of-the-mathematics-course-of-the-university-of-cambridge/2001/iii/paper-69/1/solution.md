<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use $G=\hbar=c_{\rm light}=k_B=1$ and normalize the stationary time at infinity. For a regular stationary, asymptotically flat electrovacuum [black hole](../../../../../black-hole.md), the [Kerr-Newman metric](../../../../../kerr-newman-metric.md) has

$$
a=\frac JM,\qquad d=\sqrt{M^2-Q^2-a^2},\qquad
r_\pm=M\pm d,\qquad
D_H=r_+^2+a^2=2M^2-Q^2+2Md.
$$

Initially assume $M>0$ and $d>0$, so the outer [Killing horizon](../../../../../killing-horizon.md) is nondegenerate. Its [surface gravity](../../../../../surface-gravity.md), angular velocity, electric potential and area are

$$
\kappa=\frac{r_+-r_-}{2D_H}=\frac d{D_H},\qquad
\Omega_H=\frac a{D_H},\qquad
\Phi_H=\frac{Qr_+}{D_H},\qquad
A_H=4\pi D_H.
$$

These are horizon quantities for the generator $\chi=\partial_t+\Omega_H\partial_\phi$.

The [laws of black-hole mechanics](../../../../../laws-of-black-hole-mechanics.md) provide the first reason to regard $\kappa$ and area as thermodynamic variables. The [Zeroth law of black-hole mechanics](../../../../../zeroth-law-of-black-hole-mechanics.md) makes $\kappa$ constant on an equilibrium horizon. The [first law for the Kerr-Newman family](../../../../../first-law-for-the-kerr-newman-family.md) reads

$$
dM=\frac{\kappa}{8\pi}\,dA_H+\Omega_H\,dJ+\Phi_H\,dQ.
$$

For example, write the horizon relation as $M=(r_+^2+a^2+Q^2)/(2r_+)$ and use $J=Ma$; differentiating eliminates $dr_+$ and $da$ to give this law. The last two terms are rotational and electric work. The classical [second law of black-hole mechanics](../../../../../second-law-of-black-hole-mechanics.md) says that area cannot decrease under the [null energy condition](../../../../../null-energy-condition.md) and appropriate global horizon assumptions. The [third law of black-hole mechanics](../../../../../third-law-of-black-hole-mechanics.md) concerns unattainability of a zero-surface-gravity regular horizon by a finite physical process.

This analogy alone does not determine the [temperature](../../../../../temperature.md) scale: if entropy were $\eta A_H$, the first law would only give $T=\kappa/(8\pi\eta)$. The decisive input is [quantum field theory](../../../../../quantum-field-theory-split.md) in the collapsing or stationary background. In a collapse vacuum that is regular for freely falling observers, the late outgoing retarded time $u$ and a regular affine null coordinate $U$ satisfy the [Hawking exponential ray map](../../../../../hawking-exponential-ray-map.md)

$$
U=-C e^{-\kappa u},\qquad C>0.
$$

An outgoing mode $e^{-i\omega u}$ therefore behaves as $(-U/C)^{i\omega/\kappa}$. Continuing this power through the horizon changes its amplitude by the factor $e^{-\pi\omega/\kappa}$. Its positive- and negative-frequency decomposition consequently has the [thermal ratio of Hawking Bogoliubov coefficients](../../../../../thermal-ratio-of-hawking-bogoliubov-coefficients.md)

$$
\frac{|\beta_\omega|^2}{|\alpha_\omega|^2}=e^{-2\pi\omega/\kappa}.
$$

Combining that ratio with bosonic normalization $|\alpha|^2-|\beta|^2=1$ gives a Planck occupation $1/(e^{2\pi\omega/\kappa}-1)$. The fermionic normalization instead gives the corresponding Fermi factor. Thus [Hawking radiation](../../../../../hawking-radiation.md) fixes

$$
T_H=\frac{\kappa}{2\pi}.
$$

For rotating charged modes, the horizon energy is $\widetilde\omega=\omega-m_\phi\Omega_H-q\Phi_H$, so the emission spectrum contains the same [temperature](../../../../../temperature.md) with angular-momentum and charge chemical potentials. Exterior scattering supplies [greybody factors](../../../../../greybody-factor.md); it changes the received flux, not the horizon [temperature](../../../../../temperature.md). Superradiant bosonic modes require the usual signed absorption factor, and a globally regular thermal bath need not exist throughout an asymptotically flat rotating exterior. The collapse-state emission argument is the relevant one.

A complementary check is the [Euclidean black-hole regularity condition](../../../../../euclidean-black-hole-regularity-condition.md). The local corotating nondegenerate horizon geometry is Rindler-like:

$$
ds_E^2\simeq d\rho^2+\kappa^2\rho^2d\tau^2+\text{horizon metric}.
$$

Smoothness at $\rho=0$ requires $\tau$ to have period $2\pi/\kappa$. Imaginary-time periodicity is precisely inverse [temperature](../../../../../temperature.md), agreeing with the radiation calculation. Matching the resulting [temperature](../../../../../temperature.md) to the first law fixes the [Bekenstein-Hawking entropy](../../../../../bekenstein-hawking-entropy.md) to $S=A_H/4$. The [generalized second law](../../../../../generalized-second-law.md) then uses $S_{\rm outside}+A_H/4$: the classical area theorem alone does not apply to the negative-energy quantum flux responsible for evaporation.

Substitution gives the [Kerr-Newman horizon temperature](../../../../../kerr-newman-horizon-temperature.md)

$$
\boxed{T_H=\frac{\sqrt{M^2-Q^2-J^2/M^2}}
{2\pi\left(2M^2-Q^2+2M\sqrt{M^2-Q^2-J^2/M^2}\right)}.}
$$

It reduces to $1/(8\pi M)$ for a [Schwarzschild black hole](../../../../../schwarzschild-spacetime.md). The nonextremal limit towards $d=0$ gives zero [temperature](../../../../../temperature.md). At exact extremality the Euclidean horizon is degenerate, so the elementary conical-period argument does not itself fix a period; zero [temperature](../../../../../temperature.md) here is the limiting semiclassical result. The reasoning assumes ordinary Einstein–Maxwell dynamics, a regular horizon, the stated normalization at infinity and a regime where quantum fields on a slowly evolving classical geometry are a useful approximation. The mechanical laws, radiation spectrum and Euclidean regularity agree under these assumptions, which is substantially stronger evidence than the classical analogy alone.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 69](../../paper-69-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
