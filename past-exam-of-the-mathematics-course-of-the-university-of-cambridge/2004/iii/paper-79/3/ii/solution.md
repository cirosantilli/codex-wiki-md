<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let the [shear-horizontal wave](../../../../../../shear-horizontal-wave.md) [displacement field](../../../../../../displacement-field-mechanics.md) be $U(z)e^{ikx-i\omega t}$. Its [velocity](../../../../../../velocity.md) is $V=-i\omega U$, and its [traction](../../../../../../traction.md) is $T=\mu U'$. The scalar shear-wave equation gives

$$
(\mu U')'+(\rho\omega^2-\mu k^2)U=0.
$$

With $p=k/\omega$ and $p_\beta^2=\beta^{-2}-p^2$, the first-order [velocity](../../../../../../velocity.md)–[traction](../../../../../../traction.md) system is

$$
V'=-\frac{i\omega}{\mu}T,\qquad T'=-i\omega\mu p_\beta^2V.
$$

These equations remain valid for depth-dependent $\mu,\rho$; differentiating $\mu U'$ is essential and one must not incorrectly use $\mu U''$ when $\mu$ varies.

Where $V\ne0$, define the [SH input impedance](../../../../../../sh-input-impedance.md) $Z=-T/V$. Differentiating $T=-ZV$ and substituting the two equations gives the [SH impedance Riccati equation](../../../../../../sh-impedance-riccati-equation.md):

$$
\boxed{Z'=-i\omega\left(\frac{Z^2}{\mu}-\mu p_\beta^2\right),\qquad
V'=i\omega\frac Z\mu V.}
$$

The second relation is a one-way scalar equation once the complete [SH input impedance](../../../../../../sh-input-impedance.md) is known. It does not discard reflections: $Z$ describes the actual superposition of both wave directions. At a zero of $V$, $Z$ may have a pole while the [velocity](../../../../../../velocity.md)–[traction](../../../../../../traction.md) system stays regular.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
