<h1 id="section-c/c11/solution">Solution</h1>

↑ **Parent:** [C11](../c11.md)

[quantum tunnelling](../../../../../quantum-tunnelling.md) is transmission through a finite region in which the classical kinetic [energy](../../../../../energy-split.md) $E-V$ is negative. The [wavefunction](../../../../../wave-function-split.md) need not vanish there: the [Schrödinger equation](../../../../../schrodinger-equation.md) permits evanescent solutions. The transmitted particle retains its conserved [energy](../../../../../energy-split.md); it does not borrow [energy](../../../../../energy-split.md) to surmount the barrier.

For a rectangular barrier of height $V_b$ on $0<x<d$, with $0<E<V_b$ and zero exterior [potential energy](../../../../../potential-energy.md), define $k=\sqrt{2mE}/\hbar$ and $\kappa=\sqrt{2m(V_b-E)}/\hbar$. A left-incident scattering solution has the three pieces

$$
\psi_{\rm L}=e^{ikx}+re^{-ikx},\qquad
\psi_{\rm B}=b e^{\kappa x}+c e^{-\kappa x},\qquad
\psi_{\rm R}=te^{ikx}.
$$

Continuity of $\psi,\psi'$ at both boundaries imposes

$$
1+r=b+c,\quad ik(1-r)=\kappa(b-c),\quad
be^{\kappa d}+ce^{-\kappa d}=te^{ikd},\quad
\kappa(be^{\kappa d}-ce^{-\kappa d})=ik te^{ikd}.
$$

Eliminating $b,c,r$ gives

$$
t=\frac{e^{-ikd}}{\cosh\kappa d+i\frac{\kappa^2-k^2}{2k\kappa}\sinh\kappa d},\qquad
\boxed{T=|t|^2=\left[1+\frac{V_b^2\sinh^2(\kappa d)}{4E(V_b-E)}\right]^{-1}}.
$$

Equal incident and exit velocities justify $T=|t|^2$; different exterior [potential energies](../../../../../potential-energy.md) require the velocity ratio. Probability-current conservation gives $R+T=1$. Although either real exponential alone has zero current, their complex-coefficient combination can carry the current crossing the barrier.

For $\kappa d\gg1$, $T\simeq16E(V_b-E)V_b^{-2}e^{-2\kappa d}$. A slowly varying barrier generalizes this to the [WKB approximation](../../../../../wkb-approximation.md) $T\sim\exp[-2\int_{x_1}^{x_2}\sqrt{2m(V-E)}\,dx/\hbar]$, with matching prefactors and turning-point limitations. This exponential sensitivity explains why very small geometric or [energy](../../../../../energy-split.md) changes can produce large changes in a tunnelling rate.

In [alpha decay](../../../../../alpha-decay.md), a quasibound alpha particle penetrates the nuclear [Coulomb barrier](../../../../../coulomb-barrier.md); penetration [probability](../../../../../probability.md), attempt [frequency](../../../../../frequency.md) and nuclear preformation determine the rate. In a [scanning tunnelling microscope](../../../../../scanning-tunneling-microscope.md), a bias between a conducting tip and sample gives current approximately proportional to $e^{-2\kappa d}$. Piezoelectric positioning and constant-current feedback probe surfaces, while vibration isolation and electronic-state dependence limit a purely geometric interpretation. Atomic-scale steps and surface reconstruction were resolved in the original surface-imaging study.[Abstract and pp. 57–61, atomic-scale surface images](../../../../../surface-studies-by-scanning-tunneling-microscopy-by-gerd-binnig-and-others.md) In a [Josephson junction](../../../../../josephson-junction.md), coherent tunnelling of [Cooper pairs](../../../../../cooper-pair.md) permits $I=I_c\sin\varphi$, a phase-dependent supercurrent through a weak link. Thus the same barrier physics explains natural decay and underpins sensitive surface and superconducting devices.

## ↑ Ancestors (14)

1. [C11](../c11.md)
2. [Section C](../../section-c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2010](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
