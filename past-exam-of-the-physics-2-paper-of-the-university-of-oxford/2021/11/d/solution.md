<h1 id="11/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The single secondary turn links the primary [magnetic flux](../../../../magnetic-flux.md) $\mu_0n\pi a^2I_p$, so its [mutual inductance](../../../../mutual-inductance.md) with the primary is

$$
M=\mu_0n\pi a^2=\frac{L}{nD}.
$$

Choose positive winding directions so that positive secondary [electric current](../../../../electric-current.md) would reinforce the primary [magnetic flux](../../../../magnetic-flux.md). [Faraday's law](../../../../faraday-s-law-of-induction.md) and [Kirchhoff's voltage law](../../../../kirchhoff-cycle-law.md) then give

$$
L_s\frac{dI_s}{dt}+RI_s=-M\frac{dI_p}{dt}=\omega MI_0\sin\omega t.
$$

After the transient proportional to $e^{-Rt/L_s}$ has decayed, put $\alpha=\tan^{-1}(\omega L_s/R)$. The steady [electric current](../../../../electric-current.md) is

$$
\boxed{I_s(t)=\frac{\omega MI_0}{\sqrt{R^2+(\omega L_s)^2}}\sin(\omega t-\alpha).}
$$

Its [wave amplitude](../../../../wave-amplitude.md) is $\omega MI_0/\sqrt{R^2+(\omega L_s)^2}$ and it lags the induced [electromotive force](../../../../electromotive-force.md) by $\alpha$. Relative to the primary $I_0\cos\omega t$, its [phase shift](../../../../phase-shift.md) is $-\pi/2-\alpha$, modulo $2\pi$. Reversing the chosen secondary winding direction adds $\pi$ to this signed [phase shift](../../../../phase-shift.md) and leaves all [power](../../../../power.md) predictions unchanged.

The lamp's mean [Joule heating](../../../../joule-heating.md) is

$$
\boxed{\langle P_R\rangle=\frac12R|I_s|^2=\frac{R\omega^2M^2I_0^2}{2[R^2+(\omega L_s)^2]}.}
$$

For $\omega L_s\ll R$ the response is nearly in phase with the induced [electromotive force](../../../../electromotive-force.md); for $\omega L_s\gg R$ the secondary [electric current](../../../../electric-current.md) nearly opposes the primary [electric current](../../../../electric-current.md) in the stated winding convention.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [11](../../11.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
