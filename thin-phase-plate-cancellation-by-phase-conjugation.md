# Thin phase-plate cancellation by phase conjugation

↑ **Parent:** [Phase conjugation](phase-conjugation.md)

Model a thin transparent plate by a lossless reciprocal [phase screen](phase-screen.md) with transmission $t(x)=e^{i\psi(x)}$ at the chosen [angular frequency](angular-frequency.md). Both passages multiply the local field by the same $t(x)$: reversing travel does not by itself change the sign of an accumulated [optical path length](optical-path-length.md). Assume the plate is stationary, the two passages use corresponding transverse positions, and the plate is adjacent to the return surface or perfectly reimaged onto it. Ignore propagation between these reference surfaces, [wave absorption](wave-absorption.md), clipping and intensity-dependent changes. Take the incident boundary envelope to be $U_0(x)=A(x)e^{i\phi_0(x)}$. Outward transmission gives $tU_0$. Ideal [phase conjugation](phase-conjugation.md) and the second transmission then give

$$
U_{\mathrm{return}}(x)=t(x)\gamma\bigl[t(x)U_0(x)\bigr]^*
=\gamma t(x)t(x)^*U_0(x)^*
=\gamma U_0(x)^*.
$$

This is a complete short proof of cancellation in the specified [phase screen](phase-screen.md) model. For an ideal ordinary mirror with constant reflection factor $r$, the corresponding envelope is $rt(x)^2U_0(x)$: the extra [wave phase](phase-waves.md) is $2\psi(x)$, rather than zero. A constant reflection [wave phase](phase-waves.md) changes neither conclusion.

For an original toy [optical aberration](optical-aberration.md), let $\xi=x/a$ on $-1\leq\xi\leq1$, take $\phi_0=0$, and choose

$$
\psi(\xi)=\frac{\pi}{2}\xi^2+\frac{\pi}{4}\xi^3.
$$

The even term adds symmetric curvature and the odd term makes the two sides unequal. The outward [wave phase](phase-waves.md) is $\psi$; immediately after ideal [phase conjugation](phase-conjugation.md) it is $-\psi$; after the second passage it is zero. At $\xi=-1,0,1$, the outward values are $\pi/4,0,3\pi/4$, while an ordinary mirror's completed return has values $\pi/2,0,3\pi/2$. All [wave phases](phase-waves.md) here are unwrapped relative to the central ray and are otherwise equivalent modulo $2\pi$. At a stipulated [vacuum](vacuum.md) [wavelength](wavelength.md) $\lambda=532\,\mathrm{nm}$, these outward errors correspond to [optical path length](optical-path-length.md) errors $h=\lambda\psi/(2\pi)$ of $66.5,0,199.5\,\mathrm{nm}$. These are chosen values; they are not observations or physical plate thicknesses.

<a id="phase-conjugate-phase-plate-profiles"></a>
![](phase-conjugate-phase-plate-profiles.png)

**[Figure 6](#phase-conjugate-phase-plate-profiles). Original thin phase screen example: sign reversal at conjugation and cancellation after the second passage**.

The [wave phase](phase-waves.md) plots make a subtle distinction visible: the field is still curved immediately after [phase conjugation](phase-conjugation.md), and becomes flat only after crossing the same plate again. More generally, conjugation restores $U_0^*$, not a universally flat [wavefront](wavefront.md). If the plate instead has transmission $t=\alpha(x)e^{i\psi(x)}$ with real $0\leq\alpha\leq1$, the return is $\gamma\alpha(x)^2U_0^*$. Its plate-induced [wave phase](phase-waves.md) cancels but its lost [wave amplitude](wave-amplitude.md) does not recover. If the return plate has changed to [wave phase](phase-waves.md) $\psi_{\mathrm r}$, the residual factor is $e^{i(\psi_{\mathrm r}-\psi)}$. Those two variations distinguish correction of a stationary [optical aberration](optical-aberration.md) from universal reversal of loss or material evolution.

## ↑ Ancestors (6)

1. [Phase conjugation](phase-conjugation.md)
2. [Physical optics](physical-optics-split.md)
3. [Optics](optics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-nonlinear-optics-and-quantum-states-of-light-course-of-the-university-of-cambridge/2015/paper-1/1/solution.md)
- [Phase conjugation](phase-conjugation.md)
