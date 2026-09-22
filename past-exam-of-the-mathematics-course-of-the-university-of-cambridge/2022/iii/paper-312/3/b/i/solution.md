<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Along the unperturbed photon path, combine the temperature and gravitational-redshift terms and use $\mathcal T'=-\Gamma$:

$$
\frac d{d\tau}(\Theta+\Psi)+\Gamma(\Theta+\Psi)
=\Phi'+\Psi'+\Gamma(\Theta_0+\Psi-\widehat{\mathbf n}\mathbin\cdot\mathbf v_e).
$$

The [integrating factor](../../../../../../../integrating-factor.md) is $e^{-\mathcal T}$, and $g=\Gamma e^{-\mathcal T}$. Neglecting the exponentially hidden initial boundary term gives the [Cosmic microwave background line-of-sight solution](../../../../../../../cosmic-microwave-background-line-of-sight-solution.md)

$$
(\Theta+\Psi)_0
=\int^{\tau_0}d\tau\,e^{-\mathcal T}(\Phi'+\Psi')
+\int^{\tau_0}d\tau\,g(\Theta_0+\Psi-\widehat{\mathbf n}\mathbin\cdot\mathbf v_e).
$$

For instantaneous recombination, $g(\tau)=\delta(\tau-\tau_{\rm dec})$, and the observer potential contributes only an unobservable monopole. Therefore

$$
\boxed{
\Theta(\tau_0,\mathbf0,\widehat{\mathbf n})
=\Theta_{0,{\rm dec}}+\Psi_{\rm dec}
-\widehat{\mathbf n}\mathbin\cdot\mathbf v_{e,{\rm dec}}
+\int_{\tau_{\rm dec}}^{\tau_0}d\tau\,(\Phi'+\Psi')}.
$$

The first two terms form the ordinary [Sachs-Wolfe effect](../../../../../../../sachs-wolfe-effect.md), the velocity term is the [Doppler CMB anisotropy](../../../../../../../doppler-cmb-anisotropy.md) at last scattering, and the integral is the [Integrated Sachs-Wolfe effect](../../../../../../../integrated-sachs-wolfe-effect.md) produced by evolving potentials.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 312](../../../../paper-312-split.md)
5. [Iii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
