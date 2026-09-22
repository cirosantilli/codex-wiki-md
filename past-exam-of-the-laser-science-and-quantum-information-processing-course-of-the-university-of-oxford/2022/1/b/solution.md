<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the complex [electric field](../../../../electric-field-split.md) convention $e^{-i\omega t}$ and take the locked [wave amplitudes](../../../../wave-amplitude.md) $a(\omega_p)$ to be real and nonnegative after extracting their common [phase](../../../../phase-waves.md). Linear [superposition](../../../../superposition-principle.md) gives

$$
E(t)=\sum_p a(\omega_p)e^{-i\omega_pt+i\phi_0}
=e^{-i(\omega_{\rm ce}t-\phi_0)}\sum_p a(\omega_p)e^{-ip\Delta\omega t}.
$$

The leading factor has unit modulus, so it does not change the [light intensity](../../../../light-intensity.md). The [triangle inequality](../../../../triangle-inequality.md) bounds the remaining modulus by $\sum_pa(\omega_p)$. Consecutive occupied [normal modes](../../../../normal-mode.md) attain this bound together at

$$
\boxed{t_m=mT,\qquad T=\frac{2\pi}{\Delta\omega},\qquad m=1,2,\ldots.}
$$

There is also a peak at $t=0$. The [electric field](../../../../electric-field-split.md) obeys $E(t+T)=e^{-i\omega_{\rm ce}T}E(t)$, although the [light intensity](../../../../light-intensity.md) is periodic.

The [carrier-envelope phase](../../../../carrier-envelope-phase.md) specifies where the carrier oscillation lies relative to the maximum of an [optical pulse](../../../../optical-pulse.md)'s envelope. With $s=t-t_m$ and $E=F(s)e^{-i\omega_0s+i\psi_m}$, the signed complex-field [phase](../../../../phase-waves.md) at the envelope maximum is $\psi_m$. Consequently,

$$
\boxed{\psi_{m+1}-\psi_m=-\omega_{\rm ce}T
=-\frac{2\pi\omega_{\rm ce}}{\Delta\omega}\pmod{2\pi}.}
$$

If instead the real [electric field](../../../../electric-field-split.md) is written $F(s)\cos(\omega_0s+\phi_{{\rm CE},m})$, then $\phi_{{\rm CE},m}=-\psi_m$ and the conventionally quoted slip is $\phi_{\rm slip}=+2\pi\omega_{\rm ce}/\Delta\omega$. These are the same physical shift with opposite phase definitions.

The [carrier-envelope phase](../../../../carrier-envelope-phase.md) matters for few-cycle [optical pulses](../../../../optical-pulse.md), when the largest instantaneous [electric field](../../../../electric-field-split.md) affects strong-field dynamics, for [high harmonic generation](../../../../high-harmonic-generation.md), and for stabilizing an [optical frequency comb](../../../../optical-frequency-comb.md). An ordinary cycle-averaged [light intensity](../../../../light-intensity.md) measurement does not determine it.

## ↑ Ancestors (12)

1. [B](../b.md)
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
