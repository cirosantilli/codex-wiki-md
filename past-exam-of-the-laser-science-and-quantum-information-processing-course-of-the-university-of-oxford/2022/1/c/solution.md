<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $b=\Delta\omega_b>0$ and $s=t-t_m$. At the peak time, $e^{-ip\Delta\omega t_m}=1$, so the exact comb sum becomes

$$
E(t_m+s)=Ae^{i\phi_0-i\omega_{\rm ce}t_m}
\sum_p e^{-[(\omega_p-\omega_0)/b]^2}e^{-i\omega_ps}.
$$

For many occupied [normal modes](../../../../normal-mode.md), $b\gg\Delta\omega$, replace the sum by an [integral](../../../../integral-split.md) with density $1/\Delta\omega$. Setting $x=\omega-\omega_0$ and evaluating the [Fourier transform of a Gaussian](../../../../fourier-transform-of-a-gaussian.md) gives

$$
\begin{aligned}
E(t_m+s)&\simeq\frac{A}{\Delta\omega}e^{i\phi_0-i\omega_{\rm ce}t_m}
\int_{-\infty}^{\infty}e^{-[(\omega-\omega_0)/b]^2}e^{-i\omega s}\,d\omega\\
&=\frac{A\sqrt\pi b}{\Delta\omega}
 e^{-b^2s^2/4}e^{-i\omega_0s}e^{i\phi_0-i\omega_{\rm ce}t_m}.
\end{aligned}
$$

Thus the isolated-[optical pulse](../../../../optical-pulse.md) approximation has

$$
\boxed{F(s)=\frac{A\sqrt\pi\,\Delta\omega_b}{\Delta\omega}
 e^{-(\Delta\omega_b s/2)^2},\qquad
\psi_m=\phi_0-\omega_{\rm ce}t_m.}
$$

The [optical pulse](../../../../optical-pulse.md) has a [Gaussian function](../../../../gaussian-function.md) envelope and no [chirp](../../../../chirp.md). Its carrier [angular frequency](../../../../angular-frequency.md) is $\omega_0$, and its [light intensity](../../../../light-intensity.md) [full width at half maximum](../../../../full-width-at-half-maximum.md) is $2\sqrt{2\ln2}/b$. Successive envelope maxima have different [carrier-envelope phases](../../../../carrier-envelope-phase.md), consistent with [b](../b.md).

**Approximation in the printed assertion.** A discrete [optical frequency comb](../../../../optical-frequency-comb.md) gives a train, not one exact isolated [Gaussian pulse](../../../../gaussian-pulse.md). Applying the [Poisson summation formula](../../../../poisson-summation-formula.md) to the ideal sum over all [integers](../../../../integer-split.md) instead gives

$$
E(t)=\frac{A\sqrt\pi b}{\Delta\omega}
\sum_{j\in\mathbb Z}e^{-b^2(t-jT)^2/4}
 e^{-i\omega_0(t-jT)}e^{i\phi_0-i\omega_{\rm ce}jT}.
$$

Near $t_m$, the $j=m$ term dominates when $bT\gg1$. The other terms are exponentially small but not identically zero. A single [Gaussian function](../../../../gaussian-function.md) used globally would decay between $0$ and $T$, whereas the exact [light intensity](../../../../light-intensity.md) has equal maxima there; this supplies a concrete reason the isolated form cannot be an exact global identity. The extension to negative [frequencies](../../../../frequency.md) is the usual narrow-positive-band analytic-field approximation when $\omega_0\gg b$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
