<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Resolve the weak [broadband radiation](../../../../broadband-radiation.md) into narrow [frequency](../../../../frequency.md) intervals whose relative phases are uncorrelated. The transition **[probabilities](../../../../probability.md)**, rather than the coherent amplitudes, can then be added after ensemble or time averaging. For the x-polarized field, the [energy](../../../../energy-split.md) density in one interval is $\rho(\omega)d\omega=\epsilon_0\mathcal E_\omega^2/2$, so its squared coupling is $|d_{21}|^2\mathcal E_\omega^2/\hbar^2$. Inserting this into the weak rotating-wave result gives

$$
P_2(t)=\frac{|d_{21}|^2}{2\epsilon_0\hbar^2}
\int_0^\infty\rho(\omega)
\left[\frac{\sin[(\omega-\omega_0)t/2]}{(\omega-\omega_0)/2}\right]^2d\omega.
$$

For times long compared with the [optical coherence time](../../../../optical-coherence-time.md) of the field, the narrow resonant kernel samples a nearly constant $\rho(\omega_0)$. Provided the resonance is well away from the zero-frequency boundary, extend the [Rabi detuning](../../../../rabi-detuning.md) integral to the full real line. Its value is $2\pi t$, yielding

$$
\boxed{P_2(t)\simeq W_{1\to2}t,\qquad
W_{1\to2}=\frac{\pi|\langle2|ex|1\rangle|^2}{\epsilon_0\hbar^2}\rho(\omega_0).}
$$

This is the [stimulated absorption](../../../../stimulated-absorption.md) rate for the specified [polarization](../../../../polarization-waves.md) and spectral [radiation energy density](../../../../radiation-energy-density.md) **per angular-frequency interval**. The averaging window should also satisfy $Wt\ll1$ while the lower state is treated as undepleted. A deterministic phase-locked broadband pulse would not in general permit adding these [probabilities](../../../../probability.md) without its [interference](../../../../interference-wave-propagation.md) terms.

For isotropic unpolarized radiation with total spectral [radiation energy density](../../../../radiation-energy-density.md) $\rho_{\rm tot}$, orientational averaging instead gives $W=\pi|\mathbf d_{21}|^2\rho_{\rm tot}(\omega_0)/(3\epsilon_0\hbar^2)$. The factor one third is not inserted into the original x-polarized formula. If ordinary [frequency](../../../../frequency.md) is used, $\rho_\nu=2\pi\rho_\omega$ and the isotropic coefficient becomes $|\mathbf d_{21}|^2/(6\epsilon_0\hbar^2)$ multiplying $\rho_\nu(\nu_0)$. The spectral convention and [polarization](../../../../polarization-waves.md) must be stated together to avoid spurious factors of three or $2\pi$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the quantum, atomic and molecular physics course of the University of Oxford](../../../split.md)
5. [Quantum, atomic and molecular physics course of the University of Oxford](../../../../quantum-atomic-and-molecular-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
