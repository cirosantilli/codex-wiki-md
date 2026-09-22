<h1 id="6b/solution">Solution</h1>

↑ **Parent:** [6B](../6b.md)

Balancing the viscous and bending terms gives $\zeta\omega h\sim Ah/\ell^4$, so the [elastohydrodynamic penetration length](../../../../../elastohydrodynamic-penetration-length.md) is

$$
\boxed{\ell=(A/(\zeta\omega))^{1/4}.}
$$

Inserting $h=h_0\operatorname{Re}[e^{i\omega t}F(x/\ell)]$ into the linear equation yields $F''''=-iF$, with $F(0)=1$, $F''(0)=0$ and decay at infinity. Write $C=\cos(\pi/8)$, $S=\sin(\pi/8)$. Of the four roots of $\lambda^4=-i$, precisely two have negative real part:

$$
\lambda_L=-C+iS,\qquad\lambda_R=-S-iC.
$$

The two decaying solutions are $e^{\lambda_L\eta}$ and $e^{\lambda_R\eta}$, and the general decaying response is their linear combination. Both coefficients are nonzero: if one vanished, $F''(0)=0$ would force the other to vanish, contradicting $F(0)=1$.

Their real parts in the time-dependent response are proportional to

$$
e^{-C\eta}\cos(\omega t+S\eta+\phi_L),\qquad
e^{-S\eta}\cos(\omega t-C\eta+\phi_R).
$$

Constant phases move respectively with velocities $-\omega\ell/S$ and $\omega\ell/C$, so these are damped travelling waves moving left and right. Since $S<C$, the right-going wave has the longer attenuation length and dominates at large $x$. Thus **the less strongly damped, outward-moving wave dominates the far-field response**. This is the [oscillatory bending of a moment-free semi-infinite filament](../../../../../oscillatory-bending-of-a-moment-free-semi-infinite-filament.md); the two boundary conditions determine its amplitudes without needing them explicitly here.

## ↑ Ancestors (10)

1. [6B](../6b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
