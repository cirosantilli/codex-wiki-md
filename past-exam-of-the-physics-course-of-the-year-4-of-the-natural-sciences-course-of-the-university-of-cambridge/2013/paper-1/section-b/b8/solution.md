<h1 id="section-b/b8/solution">Solution</h1>

↑ **Parent:** [B8](../b8.md)

Substitution of a plane wave in the [Schrödinger equation](../../../../../schrodinger-equation.md) gives $\hbar\omega=\hbar^2k^2/(2m)+V_0$. For a stationary step-scattering state, remove the common phase $e^{-iEt/\hbar}$ and write $\psi_L=e^{ikx}+r e^{-ikx}$, $k=\sqrt{2mE}/\hbar$. If $E>V_0$, the right-side outgoing wave is $\psi_R=t e^{iqx}$, $q=\sqrt{2m(E-V_0)}/\hbar$. A finite step with no delta-function potential in the Schrödinger operator requires continuous $\psi$ and $\psi'$: a discontinuous [wavefunction](../../../../../wave-function-split.md) would generate a delta derivative, and integrating the equation over a vanishing interval gives derivative continuity. Matching yields

$$
r=\frac{k-q}{k+q},\qquad t=\frac{2k}{k+q},\qquad
\boxed{\mathcal R=\left(\frac{\sqrt E-\sqrt{E-V_0}}{\sqrt E+\sqrt{E-V_0}}\right)^2\quad(E>V_0).}
$$

For $0<E<V_0$, take $q=i\kappa$ and the bounded right-side state $te^{-\kappa x}$. It carries no transmitted flux and $\mathcal R=1$. The threshold limit also has reflection [probability](../../../../../probability.md) one. Thus at $V_0=1\,\mathrm{eV}$,

$$
\boxed{\mathcal R(0.9\,\mathrm{eV})=1,\qquad\mathcal R(1.1\,\mathrm{eV})\simeq0.288.}
$$

For the two-step profile, set $k_0=\sqrt{2mE}/\hbar$, $k_1=\sqrt{2m(E-V_1)}/\hbar$ and $k_2=\sqrt{2m(E-V_0)}/\hbar$. With all regions propagating, the net reflection amplitude is

$$
r_{\rm tot}=\frac{r_{01}+r_{12}e^{2ik_1a}}{1+r_{01}r_{12}e^{2ik_1a}},\qquad
r_{ij}=\frac{k_i-k_j}{k_i+k_j}.
$$

The given quarter-wave condition makes $e^{2ik_1a}=-1$. Zero reflection then requires $r_{01}=r_{12}$, equivalent to $k_1^2=k_0k_2$. Consequently

$$
\boxed{E-V_1=\sqrt{E(E-V_0)},\qquad\text{or}\qquad E=\frac{V_1^2}{2V_1-V_0}.}
$$

For an increasing intermediate step this needs $E>V_0$ and $V_0/2<V_1<V_0$, together with the stipulated thickness condition. In this [quarter-wave matching layer for a quantum potential step](../../../../../quarter-wave-matching-layer-for-a-quantum-potential-step.md), two reflected amplitudes cancel while the transmitted flux equals the incident flux.

## ↑ Ancestors (13)

1. [B8](../b8.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
5. [Past exam of the physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
