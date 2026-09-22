<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use incompressible [ideal MHD](../../../../../ideal-magnetohydrodynamics.md) at scales above the [ion skin depth](../../../../../ion-skin-depth.md), a strong uniform mean field, and a statistically steady local [energy cascade](../../../../../energy-cascade.md) with mean flux $\epsilon$ per unit mass. Assume balanced counterpropagating wave populations, comparable velocity and magnetic amplitudes in velocity units, and no additional scale-dependent alignment or intermittency correction. Write $\mathbf b=\delta\mathbf B/\sqrt{4\pi\rho}$ and introduce the fluctuation [Elsässer variables](../../../../../elsasser-variable.md) $\mathbf z^\pm=\mathbf u\pm\mathbf b$. Their equations are

$$
\partial_t\mathbf z^\pm\mp v_A\partial_\parallel\mathbf z^\pm+(\mathbf z^\mp\cdot\nabla)\mathbf z^\pm=-\nabla\Pi,\qquad\nabla\cdot\mathbf z^\pm=0.
$$

Only opposite populations distort one another. A single population has no leading nonlinear self-interaction, so the balance assumption is essential to a one-amplitude cascade estimate.

Let $\delta z_l$ denote the typical balanced amplitude and let $l_\perp,l_\parallel$ be coherence lengths relative to the local mean field. The [Alfvén wave](../../../../../alfven-wave.md) time and [eddy turnover time](../../../../../eddy-turnover-time.md) are

$$
\tau_A=\frac{l_\parallel}{v_A},\qquad\tau_{\rm nl}=\frac{l_\perp}{\delta z_l},\qquad\chi=\frac{\tau_A}{\tau_{\rm nl}}.
$$

For $\chi\ll1$, one counterpropagating encounter changes the packet fractionally by order $\chi$. Assume phases decorrelate between encounters. After $N$ encounters, random accumulation is of order $\sqrt N\chi$; an order-one change requires $N\sim\chi^{-2}$. The [weak wave cascade](../../../../../weak-wave-cascade.md) time is therefore

$$
\tau_{\rm cas}\sim N\tau_A=\frac{\tau_{\rm nl}^2}{\tau_A}.
$$

Weakness by itself does not prove this [random walk](../../../../../random-walk.md) estimate; phase decorrelation and the interaction geometry are additional assumptions.

For the [Iroshnikov-Kraichnan spectrum](../../../../../iroshnikov-kraichnan-spectrum.md), impose isotropy, $l_\parallel\sim l_\perp\sim l$, in addition to $\delta z_l\ll v_A$. Then $\tau_A=l/v_A\ll\tau_{\rm nl}=l/\delta z_l$ and

$$
\tau_{\rm cas}\sim\frac{v_Al}{\delta z_l^2},\qquad
\epsilon\sim\frac{\delta z_l^2}{\tau_{\rm cas}}\sim\frac{\delta z_l^4}{v_Al}.
$$

Hence $\delta z_l\sim(\epsilon v_Al)^{1/4}$. A local shell-integrated [turbulent energy spectrum](../../../../../turbulent-energy-spectrum.md) has $\delta z_l^2\sim kE(k)$, $k\sim l^{-1}$, so

$$
\boxed{E_{\rm IK}(k)\sim(\epsilon v_A)^{1/2}k^{-3/2}.}
$$

The isotropy is imposed phenomenologically; a strong guide field actually distinguishes directions and does not force this isotropic picture. The spectrum is not an automatically valid asymptotic result for every strongly magnetized cascade.

For the anisotropic [weak Alfvénic cascade](../../../../../weak-alfvenic-cascade.md), keep $l_\parallel$ approximately fixed while cascading to smaller $l_\perp$, and require $\chi\ll1$. This geometry follows from resonant three-wave Alfvén interactions: frequency conservation together with parallel-wavenumber conservation makes one member of an oppositely propagating resonant triad have zero parallel wavenumber, so the propagating modes retain their parallel wavenumber in the leading resonant transfer. Thus there is no leading parallel cascade in this ideal weak-wave ordering. Using the fixed parallel scale,

$$
\tau_{\rm cas}\sim\frac{v_Al_\perp^2}{\delta z_l^2l_\parallel},\qquad
\epsilon\sim\frac{\delta z_l^4l_\parallel}{v_Al_\perp^2}.
$$

Therefore $\delta z_l\sim(\epsilon v_A/l_\parallel)^{1/4}l_\perp^{1/2}$. For the one-dimensional perpendicular spectrum, $\delta z_l^2\sim k_\perp E_\perp(k_\perp)$ gives

$$
\boxed{E_{\perp,\rm weak}(k_\perp)\sim\left(\frac{\epsilon v_A}{l_\parallel}\right)^{1/2}k_\perp^{-2}.}
$$

Unlike the isotropic estimate, the parallel length does not decrease with the perpendicular length. Since $\chi=\delta z_l l_\parallel/(v_Al_\perp)\propto l_\perp^{-1/2}$, the interactions become stronger down the cascade. If $\chi_0\ll1$ at outer perpendicular scale $L_\perp$, the weak approximation breaks at $l_{\perp,*}\sim L_\perp\chi_0^2$. This is the [weak-to-strong transition of an Alfvénic cascade](../../../../../weak-to-strong-transition-of-an-alfvenic-cascade.md).

For [Goldreich–Sridhar turbulence](../../../../../goldreich-sridhar-turbulence.md), abandon the weak-collision estimate and impose [critical balance](../../../../../critical-balance.md), $\tau_A\sim\tau_{\rm nl}$. The local cascade is strong, with transfer time of order one [eddy turnover time](../../../../../eddy-turnover-time.md). Then

$$
\epsilon\sim\frac{\delta z_l^3}{l_\perp},\qquad\delta z_l\sim(\epsilon l_\perp)^{1/3},
\qquad\boxed{E_{\perp,\rm GS}(k_\perp)\sim\epsilon^{2/3}k_\perp^{-5/3}.}
$$

The parallel scale is set dynamically, not held fixed:

$$
\boxed{l_\parallel\sim v_A\epsilon^{-1/3}l_\perp^{2/3},\qquad k_\parallel\sim\frac{\epsilon^{1/3}}{v_A}k_\perp^{2/3}.}
$$

At smaller scales $l_\parallel/l_\perp$ grows, so the eddies are increasingly elongated along the local [magnetic field](../../../../../magnetic-field.md). Strong turbulence does not mean $\delta z_l\sim v_A$: small transverse amplitudes can still be strong when the eddies are sufficiently anisotropic to satisfy [critical balance](../../../../../critical-balance.md). Imbalance, alignment or nonlocal interactions would require different cascade reasoning.

Finally, in the usual isotropic hydrodynamic [Kolmogorov 1941 theory](../../../../../kolmogorov-1941-theory.md) inertial-range argument, the only relevant dimensional quantities are $\epsilon$ and $k$. With $[\epsilon]=L^2T^{-3}$ and $[E]=L^3T^{-2}$, writing $E\propto\epsilon^ak^b$ forces $a=2/3$, $b=-5/3$. This uses the physical assumptions that outer-scale, viscous and intermittency effects do not supply another leading dependence; dimensions alone are not a proof of those assumptions.

A magnetic guide field supplies the independent speed $v_A$, and anisotropy adds independent parallel lengths. Even before adding anisotropy, dimensions permit

$$
\boxed{E(k)=\epsilon^{2/3}k^{-5/3}\Phi\left(v_A\epsilon^{-1/3}k^{1/3}\right),}
$$

with arbitrary dimensionless $\Phi$. For example $\Phi(x)\propto x^{1/2}$ reproduces the isotropic [Iroshnikov-Kraichnan spectrum](../../../../../iroshnikov-kraichnan-spectrum.md) estimate. This [dimensional freedom of an MHD spectrum](../../../../../dimensional-freedom-of-an-mhd-spectrum.md) explains why propagation, decorrelation, anisotropy and cascade-time assumptions must select among the spectra: purely dimensional considerations do not select a unique MHD exponent.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 75](../../paper-75-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
