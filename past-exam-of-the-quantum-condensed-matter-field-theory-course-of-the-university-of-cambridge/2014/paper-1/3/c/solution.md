<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a dilute three-dimensional [weakly interacting Bose gas](../../../../../weakly-interacting-bose-gas.md) with repulsive short-range scattering, use a contact coupling $g=4\pi\hbar^2a_s/m>0$ and $na_s^3\ll1$. In imaginary time $\tau_E$, the grand-canonical action is

$$
S_E=\int_0^{\beta\hbar}d\tau_E\int d^3x\left[\bar\psi\hbar\partial_{\tau_E}\psi+\frac{\hbar^2}{2m}|\nabla\psi|^2-\mu|\psi|^2+\frac g2|\psi|^4\right],\qquad Z=\int\mathcal D\psi\,e^{-S_E/\hbar}.
$$

The uniform saddle has $n_0=\mu/g$. Its real-time equation is the [Gross–Pitaevskii equation](../../../../../gross-pitaevskii-equation.md); quantum depletion means condensate and total density need not coincide exactly.

Writing $\psi=\sqrt{n_0}+\delta\psi$ and retaining quadratic fluctuations gives a Nambu kernel with diagonal $\epsilon_k+gn_0$, anomalous coupling $gn_0$ and $\epsilon_k=\hbar^2k^2/(2m)$. The [Bogoliubov quasiparticle dispersion](../../../../../bogoliubov-quasiparticle-dispersion.md) is

$$
\boxed{E_k=\sqrt{\epsilon_k(\epsilon_k+2gn_0)},\qquad E_k\simeq\hbar c_s|k|,\quad c_s=\sqrt{gn_0/m}.}
$$

Phase and density fluctuations form the gapless sound mode associated with broken global $U(1)$ symmetry. At large momentum the spectrum crosses towards particle behaviour; the [healing length](../../../../../healing-length.md) is $\xi=\hbar/\sqrt{2mgn_0}$. The depletion integral $\int d^3k\,v_k^2/(2\pi)^3$ is finite in three dimensions and gives $(n-n_0)/n\simeq8\sqrt{na_s^3}/(3\sqrt\pi)$ to leading order. The contact coupling denotes a scattering-length-renormalized interaction; naive ultraviolet zero-point integrals require renormalization.

The condensate phase gives [superfluid velocity](../../../../../superfluid-velocity.md) $\mathbf v_s=(\hbar/m)\nabla\theta$ and quantized circulation $\oint\mathbf v_s\cdot d\mathbf l=2\pi\hbar\ell/m$. The [Landau criterion](../../../../../landau-criterion.md), $v_c=\min_kE_k/(\hbar k)$, gives $c_s$ for this homogeneous Bogoliubov spectrum. Boundaries and vortex nucleation can cause dissipation below that value, so it is not a universal measured critical speed. Condensation and superfluid stiffness are related but distinct; dimensional fluctuations can remove true condensate order while retaining superfluid responses.

<a id="3/c/image-the-dilute-gas-bogoliubov-spectrum-crosses-from-sound-to-particle-like-excitations"></a>
![](../../../../../past-exam-of-the-quantum-condensed-matter-field-theory-course-of-the-university-of-cambridge/2014/paper-1-qcm2014-bose-dispersion.png)

**[Figure 3](#3/c/image-the-dilute-gas-bogoliubov-spectrum-crosses-from-sound-to-particle-like-excitations). The dilute-gas Bogoliubov spectrum crosses from sound to particle-like excitations**. [Source](paper-1-qcm2014-bose-dispersion.py).

## ↑ Ancestors (14)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2014](../../../split.md)
5. [Past exam of the quantum Condensed Matter Field Theory course of the University of Cambridge](../../../../split.md)
6. [Quantum Condensed Matter Field Theory course of the University of Cambridge](../../../../../quantum-condensed-matter-field-theory-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
