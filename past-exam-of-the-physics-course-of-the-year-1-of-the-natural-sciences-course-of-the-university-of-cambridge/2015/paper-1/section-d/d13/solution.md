<h1 id="section-d/d13/solution">Solution</h1>

↑ **Parent:** [D13](../d13.md)

For a flexible uniform string with [linear mass density](../../../../../linear-mass-density.md) $\rho$ and [tension](../../../../../tension.md) $T$, [dimensional analysis](../../../../../dimensional-analysis.md) gives $[T/\rho]=L^2T^{-2}$ and hence $c\propto\sqrt{T/\rho}$. The small-slope [force](../../../../../force-split.md) balance $\rho\psi_{tt}=T\psi_{xx}$ fixes the factor to one:

$$
\boxed{c=\sqrt{T/\rho},\qquad \omega=ck.}
$$

Here $\rho$ has units kg/m, not the volume-density units used for a bulk fluid. The [phase](../../../../../phase-waves.md) moves along the string at $c$, while a material point moves transversely with $\psi_t=A\omega\sin(kx-\omega t)$. Its maximum [speed](../../../../../speed.md) is **$A\omega$**, which is not the [phase velocity](../../../../../phase-velocity.md). Small slope $Ak\ll1$ makes $A\omega\ll c$ in this model.

The [kinetic energy](../../../../../kinetic-energy.md) and extra elastic [energy](../../../../../energy-split.md) of a segment are

$$
K=\frac12\int\rho\psi_t^2\,dx,\qquad U=\frac12\int T\psi_x^2\,dx.
$$

The second expression follows from extra [length](../../../../../length.md) $\sqrt{1+\psi_x^2}dx-dx\simeq\psi_x^2dx/2$ against the pre-existing constant [tension](../../../../../tension.md). Time averaging a harmonic [wave](../../../../../wave-split.md) gives $\langle\mathcal E_K\rangle=\rho A^2\omega^2/4$ and $\langle\mathcal E_U\rangle=TA^2k^2/4=\rho A^2\omega^2/4$. Therefore

$$
\boxed{\varepsilon_{\rm av}=\frac12\rho A^2\omega^2.}
$$

At the driven endpoint the string pulls along its local tangent into $x>0$, with vertical component $T\psi_x$ for small slope. The point exerts the opposite [force](../../../../../force-split.md) on the string, so the [driven-string endpoint power](../../../../../driven-string-endpoint-power.md) is

$$
\boxed{P(0,t)=-T\psi_x(0,t)\psi_t(0,t).}
$$

For the outgoing [wave](../../../../../wave-split.md) $\psi=A\cos(kx-\omega t)$, at $x=0$ the [derivatives](../../../../../derivative.md) are $\psi_x=Ak\sin\omega t$ and $\psi_t=-A\omega\sin\omega t$. Thus $P=TA^2k\omega\sin^2\omega t$ and

$$
\boxed{P_{\rm av}=\frac12TA^2k\omega=c\varepsilon_{\rm av}.}
$$

The [energy flux of a transverse string wave](../../../../../energy-flux-of-a-transverse-string-wave.md) follows by combining the [energy density](../../../../../energy-density.md) $\mathcal E=(\rho\psi_t^2+T\psi_x^2)/2$ and flux $P=-T\psi_x\psi_t$, which satisfy $\partial_t\mathcal E+\partial_xP=0$. For a pure right-going nondispersive [wave](../../../../../wave-split.md), $P=c\mathcal E$ even instantaneously. [energy](../../../../../energy-split.md) is transported with the [wave](../../../../../wave-split.md); a material string element merely oscillates about its unperturbed position.

## ↑ Ancestors (13)

1. [D13](../d13.md)
2. [Section D](../../section-d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
