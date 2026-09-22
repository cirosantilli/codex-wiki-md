<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Choose depth $z$ positive downwards, the free surface at $z=0$ and the interface at $z=h$. A [Love wave](../../../../../../love-wave.md) has only transverse [displacement field](../../../../../../displacement-field-mechanics.md) $u_y=U(z)e^{i(\kappa x-\omega t)}$. Take $\omega>0$, $\kappa=\omega/c_L$, and define

$$
q=\sqrt{\omega^2/\beta_0^2-\kappa^2},\qquad p=\sqrt{\kappa^2-\omega^2/\beta^2}.
$$

A trapped mode requires **$\beta_0<c_L<\beta$**, so both $q,p$ are positive. The SH equations are $U_0''+q^2U_0=0$ in the layer and $U''-p^2U=0$ in the half-space. Zero shear [traction](../../../../../../traction.md) at the free surface and decay at large depth select

$$
U_0=A\cos(qz),\qquad U=C e^{-p(z-h)}.
$$

Continuity of [displacement field](../../../../../../displacement-field-mechanics.md) and shear [traction](../../../../../../traction.md) at $h$ gives $C=A\cos(qh)$ and $-\mu_0qA\sin(qh)=-\mu pC$. Consequently

$$
\boxed{\tan(qh)=\frac{\mu p}{\mu_0q}.}
$$

Substituting the definitions of $q,p$ yields the requested speed-frequency dispersion relation. For negative [frequency](../../../../../../frequency.md) use $|\omega|$ in both vertical wavenumbers; the real [displacement field](../../../../../../displacement-field-mechanics.md) has conjugate [frequency](../../../../../../frequency.md) partners. Neither equality in the trapped-speed interval gives a strictly localized finite-frequency Love mode.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../b.md)
3. [2](../../2.md)
4. [Paper 82](../../../paper-82-split.md)
5. [Iii](../../../split.md)
6. [2005](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
