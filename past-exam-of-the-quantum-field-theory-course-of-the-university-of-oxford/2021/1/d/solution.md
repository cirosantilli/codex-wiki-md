<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**The printed integration labels need correction.** The parent's [four-momentum](../../../../four-momentum.md) is fixed, so the two [Lorentz-invariant phase-space measures](../../../../lorentz-invariant-phase-space-measure.md) must integrate $p_2$ and $p_3$, rather than the printed $p_1$ and $p_2$. Write $P=p_1=(M,\mathbf0)$ and $p=p_2$, $k=p_3$. The physical [decay width](../../../../decay-width.md) is

$$
\Gamma=\frac{\overline{|\mathcal M|^2}}{2M}
\int\frac{d^3p}{(2\pi)^3\,2E_p}
\frac{d^3k}{(2\pi)^3\,2E_k}
(2\pi)^4\delta^{(4)}(P-p-k).
$$

The spatial [Dirac delta function](../../../../dirac-delta-function.md) sets $\mathbf k=-\mathbf p$. Performing the angular integral in [spherical coordinates](../../../../spherical-coordinate-system.md), with $E=\sqrt{p^2+m^2}$, gives the integrated [two-body decay phase space](../../../../two-body-decay-phase-space.md)

$$
\Phi_2=\frac1{4\pi}\int_0^\infty\frac{p^2\,dp}{E^2}\delta(M-2E).
$$

The positive root is $p_*=\sqrt{M^2/4-m^2}$. Since $d(2E)/dp=2p/E$, the [Dirac delta function](../../../../dirac-delta-function.md) integration yields $\Phi_2=p_*/(4\pi M)$. Thus

$$
\boxed{\Gamma=\frac{\overline{|\mathcal M|^2}\,p_*}{8\pi M^2}
=\frac{g^2(M+2m)}{16\pi}\sqrt{1-\frac{4m^2}{M^2}},\qquad M>2m.}
$$

The two final particles have different species, so there is no [identical final-state symmetry factor](../../../../identical-particle-factor-in-a-final-state-phase-space-integral.md). The result tends to $g^2M/(16\pi)$ as $m\to0$ and vanishes at the two-particle [decay threshold](../../../../decay-threshold.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
