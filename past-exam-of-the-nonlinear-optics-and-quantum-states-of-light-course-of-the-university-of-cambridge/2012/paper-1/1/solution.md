<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

[Second-harmonic generation](../../../../second-harmonic-generation.md) doubles optical [frequency](../../../../frequency.md), hence halves the vacuum [wavelength](../../../../wavelength.md). It requires a nonzero effective second-order [nonlinear optical susceptibility](../../../../nonlinear-optical-susceptibility.md) for the selected fields, overlap in the nonlinear medium, and enough intensity and interaction length for a useful signal. Bulk electric-dipole second-order response vanishes in an inversion-symmetric medium. Low absorption at both frequencies and [phase matching](../../../../phase-matching.md) prevent generated amplitudes from being lost or canceling during propagation. Pulses additionally need suitable temporal overlap and bandwidth acceptance.

For the stated lossless amplitude equations, choose real $\alpha$, input $A_0=|A_0|e^{i\phi}$ and **no second-harmonic seed**. Perfect [phase matching](../../../../phase-matching.md) admits

$$
A_\omega(z)=A_0\operatorname{sech}(\lambda z),\qquad
A_{2\omega}(z)=i|A_0|e^{2i\phi}\tanh(\lambda z),\qquad
\boxed{\lambda=\alpha|A_0|.}
$$

The second equation follows by substituting the first into $A_\omega'=i\alpha A_{2\omega}A_\omega^*$. Its derivative then equals $i\alpha A_0^2\operatorname{sech}^2(\lambda z)$, verifying the other coupled equation. Equivalently, $\lambda^2=\alpha^2|A_0|^2$; changing the sign of $\lambda$ does not change the pump profile. The intensity convention in the question therefore gives

$$
\boxed{I_{2\omega}(z)=I_0\tanh^2(\alpha\sqrt{I_0}\,z),\qquad
I_\omega(z)=I_0\operatorname{sech}^2(\alpha\sqrt{I_0}\,z).}
$$

Their sum is $I_0$, as follows directly from the supplied equal-coupling equations. This uses their normalization; physically normalized photon-flux equations can place [frequency](../../../../frequency.md) factors in the two coupling coefficients. A nonzero input harmonic would require a different boundary-value solution.

For an undepleted pump at nonzero mismatch, direct integration gives

$$
A_{2\omega}(z)=i\alpha A_0^2z\,e^{i\Delta kz/2}\operatorname{sinc}(\Delta kz/2),\qquad
I_{2\omega}(z)=\alpha^2I_0^2z^2\operatorname{sinc}^2(\Delta kz/2).
$$

Here $\operatorname{sinc}x=\sin x/x$. The perfectly matched small-signal curve grows quadratically and its depleted continuation saturates. For $\Delta kL=\pi$, destructive phase accumulation reduces output; in the undepleted limit its endpoint is $4/\pi^2$ of the matched small-signal output. For $|\Delta k|L\gg\pi$, successive regions alternately generate and cancel harmonic amplitude, giving rapid low-amplitude oscillations with spatial period $2\pi/|\Delta k|$. For substantial depletion, the complete curve also depends on $\alpha\sqrt{I_0}L$; specifying mismatch alone does not determine a unique numerical sketch.

<a id="1/image-second-harmonic-depletion-phase-mismatch-and-two-crystal-interference"></a>
![](../../../../past-exam-of-the-nonlinear-optics-and-quantum-states-of-light-course-of-the-university-of-cambridge/2012/paper-1-shg-depletion-and-interference.png)

**[Figure 1](#1/image-second-harmonic-depletion-phase-mismatch-and-two-crystal-interference). Second-harmonic depletion, phase mismatch and two-crystal interference**. Original integration of the stated lossless amplitude equations. Left: three mismatches for a declared nonlinear interaction strength. Right: output versus gap phase for identical crystals at several strengths; curves are illustrative model predictions, not measured data.

For the separated crystals, use the undepleted approximation and perfect matching inside each crystal. Up to a common output phase, the harmonic generated in the first crystal contributes $i\alpha A_0^2L e^{ik(2\omega)d}$, while the second crystal contributes $i\alpha A_0^2L e^{2ik(\omega)d}$. The different phases come from propagation of an already generated harmonic versus propagation of two pump factors through the gap. Ideal antireflection coatings remove the multiple-reflection complication. Thus

$$
\boxed{I_{2\omega}^{\rm out}(d)=4\alpha^2I_0^2L^2
\cos^2\left[\frac{\Delta k_gd}{2}\right],\qquad
\Delta k_g=\frac{2\omega}{c}[n(\omega)-n(2\omega)].}
$$

This is [two-crystal second-harmonic interference](../../../../two-crystal-second-harmonic-interference.md). Maxima require $\Delta k_gd=2\pi m$. With nonzero dispersion, their spacing is $2\pi/|\Delta k_g|=\lambda_0/[2|n(\omega)-n(2\omega)|]$, where $\lambda_0$ is the pump vacuum [wavelength](../../../../wavelength.md). If the gap has no index difference between these frequencies, every separation is constructive within this ideal propagation model.

Finite depletion makes the amplitude entering the second crystal smaller and permits coherent backconversion, so the simple cosine-squared envelope no longer applies and the total converted intensity cannot exceed $I_0$. The gap phase remains periodic. In the ideal identical lossless case the constructive setting is equivalent to a matched crystal of length $2L$, giving $I_0\tanh^2(2\alpha\sqrt{I_0}L)$. The opposite relative phase can make the second crystal reverse the first conversion, restoring the pump and leaving zero harmonic. Thus depletion does not necessarily fill an ideal destructive minimum; unequal crystals, loss or other phase errors can spoil that cancellation.

## ↑ Ancestors (13)

1. [1](../1.md)
2. [Paper 1](../../paper-1-split.md)
3. [2012](../../split.md)
4. [Past exam of the nonlinear Optics and Quantum States of Light course of the University of Cambridge](../../../split.md)
5. [Nonlinear Optics and Quantum States of Light course of the University of Cambridge](../../../../nonlinear-optics-and-quantum-states-of-light-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
