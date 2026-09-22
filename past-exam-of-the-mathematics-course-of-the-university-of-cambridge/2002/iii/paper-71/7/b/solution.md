<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

There is a sign error in the printed synchronous line-of-sight integrand. Direct contraction of the stated decomposition gives $h'_{ij}n^in^j=(h'-h_S')/3+(\hat{\mathbf k}\cdot\mathbf n)^2h_S'$, with a **plus** sign in its last term. In the positive spatial-perturbation convention of part a, the [redshift](../../../../../../redshift.md) term is half this contraction. The printed minus sign cannot yield the requested Newtonian expression with the supplied transformations.

The consistent identity can be derived explicitly. Work mode by mode with $q=\mathbf k\cdot\mathbf n$, $E(\tau)=e^{iq(\tau-\tau_0)}$ along the unperturbed ray; the shift of the phase origin is immaterial. Put $A=(h-h_S)/6$. Part a gives $A=\Psi-\mathcal HT$, while $\Phi=-\mathcal HT-T'$. Therefore $A'=\Phi'+\Psi'+T''$. The corrected synchronous integral is

$$
I_S=\int_{\tau_d}^{\tau_0}E(A'+q^2T)\,d\tau=\int_{\tau_d}^{\tau_0}E(\Phi'+\Psi')\,d\tau+[E(T'-iqT)]_{\tau_d}^{\tau_0},
$$

since $[E(T'-iqT)]'=E(T''+q^2T)$. This is the [photon redshift identity with positive spatial perturbations](../../../../../../photon-redshift-identity-with-positive-spatial-perturbations.md).

The supplied fluid shifts are $\delta_\gamma^N=\delta_\gamma+4\mathcal HT$ and $\mathbf v_\gamma^N=\mathbf v_\gamma+i\mathbf kT$. At emission, the synchronous intrinsic and Doppler terms are consequently $E_d[\delta_\gamma^N/4+\mathbf v_\gamma^N\cdot\mathbf n-\mathcal HT-iqT]_d$. Adding the lower integral endpoint cancels the velocity shift and leaves $-\mathcal HT-T'=\Phi$. The upper endpoint is the local observer monopole/dipole $[T'-iqT]_0$, removed by [temperature](../../../../../../temperature.md) calibration and the observer-rest-frame convention. With zero [anisotropic stress](../../../../../../anisotropic-stress.md), $\Phi=\Psi$, the observable higher-multipole result is

$$
\boxed{\frac{\Delta T}{T}(\mathbf n)=\left[\frac14\delta_\gamma^N+\mathbf v_\gamma^N\cdot\mathbf n+\Phi\right]_d+2\int_{\tau_d}^{\tau_0}\Phi'\,d\tau}.
$$

All fields are evaluated along the ray; the integral contains the time derivative at fixed spatial position. Retaining the printed negative angular term would leave the additional $-2q^2\int ET\,d\tau$, generally a gauge-dependent, nonzero term. It is therefore not repaired merely by discarding observer monopole and dipole.

The first term is the intrinsic [photon](../../../../../../photon.md) [temperature](../../../../../../temperature.md) perturbation, important in acoustic compressions and rarefactions. The velocity term is the Doppler shift and is prominent near acoustic, roughly degree and subdegree, scales; it is suppressed on very large scales. The potential at emission is the ordinary [Sachs-Wolfe effect](../../../../../../sachs-wolfe-effect.md); combined with the intrinsic term it gives the familiar large-angle adiabatic matter-era result $\Phi/3$. The final term is the [Integrated Sachs-Wolfe effect](../../../../../../integrated-sachs-wolfe-effect.md), caused by changing potentials. It vanishes for constant matter-era potentials, receives an early contribution near radiation-matter transition, and has an important late large-angle contribution when [curvature](../../../../../../curvature.md) or dark [energy](../../../../../../energy.md) causes potentials to evolve. The sign of the Doppler term follows the photon-propagation direction convention used in the ray; reversing that direction reverses it consistently.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [7](../../7.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
