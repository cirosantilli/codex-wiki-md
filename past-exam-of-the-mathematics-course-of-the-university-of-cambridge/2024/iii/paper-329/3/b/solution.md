<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The expression in braces in the first equation is the net axial force. The term $-\pi a^2\gamma/a$ is the compressive force from the [capillary pressure](../../../../../../capillary-pressure.md) $\gamma/a$, $3\pi\mu a^2w_z$ is the Newtonian extensional tension with [Trouton ratio](../../../../../../trouton-ratio.md) three, and $2\pi a\gamma$ is the axial pull of [surface tension](../../../../../../surface-tension.md) around the circumference. Its $z$-derivative vanishes because axial force is conserved.

The final equation is conservation of an [insoluble surfactant](../../../../../../insoluble-surfactant.md). The surface divergence $w_z+u/a$ is the sum of axial and circumferential extension rates. Positive surface divergence increases interfacial area and dilutes $C$; negative divergence concentrates it. The absence of a diffusion term expresses the assumption of negligible surface diffusion.

Linearizing the area and surfactant equations gives

$$
2\eta_t=-a_0w_z,
\qquad
C'_t=-C_0\left(w_z+\frac{\eta_t}{a_0}\right)
=\frac{C_0}{a_0}\eta_t.
$$

Thus

$$
\frac\partial{\partial t}(a_0C'-C_0\eta)=0,
$$

and hence

$$
\boxed{a_0C'(z,t)=C_0\eta(z,t)+\psi(z)},
$$

where $\psi$ is fixed by the initial data.

Linearizing the displayed net axial force and using $\gamma'=-AC'$ gives

$$
3\pi\mu a_0^2w_z+\pi\gamma_0\eta
-\pi Aa_0C'=0.
$$

Eliminating $w_z$ and $C'$ therefore gives directly

$$
6\mu a_0\eta_t
=(\gamma_0-AC_0)\eta-A\psi(z).
$$

Thus the three displayed evolution equations imply

$$
\boxed{
\eta_t=s\eta-\frac{A\psi(z)}{6\mu a_0},
\qquad
s=\frac{\gamma_0-AC_0}{6\mu a_0}}.
$$

The target formula printed later in the paper contains an additional factor of $\pi$ in both denominators. That factor does not follow from the displayed equations because every term in the axial-force balance contains the same factor $\pi$. If the target formula is adopted as the intended normalization, its corresponding value is $s=(\gamma_0-AC_0)/(6\pi\mu a_0)$.

Initially $\eta=0$ and $C'>0$, so $\psi>0$ and $\eta_t<0$: a surfactant-rich, low-tension region begins to neck as neighboring higher tension pulls fluid away. The accompanying axial extension dilutes the surfactant.

If $A<\gamma_0/C_0$, then $s>0$. The [Rayleigh–Plateau instability](../../../../../../rayleigh-plateau-instability.md) overwhelms the weak surface-elastic response: the necking perturbation grows in the linear model while the original concentration excess is diluted and eventually changes sign.

If $A>\gamma_0/C_0$, then $s<0$. Strong surface elasticity arrests the disturbance at

$$
\eta_\infty=\frac{A\psi}{\gamma_0-AC_0}<0.
$$

The concentration perturbation becomes negative, raising the local surface tension until its axial force balances that of the wider regions. This is stabilization by a [surfactant-induced Marangoni stress](../../../../../../marangoni-effect.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
