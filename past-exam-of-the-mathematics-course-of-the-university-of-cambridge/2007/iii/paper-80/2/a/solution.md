<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use $\widehat\psi_{\rm sc}(\nu)=\int\psi_{\rm sc}(x,0)e^{-i\nu x}dx$, inverse factor $1/(2\pi)$, and $k=\omega/c$. [Fourier transform](../../../../../../fourier-transform.md) the homogeneous [Helmholtz equation](../../../../../../helmholtz-equation.md) gives

$$
\partial_z^2\widehat\psi_{\rm sc}+(k^2-\nu^2)\widehat\psi_{\rm sc}=0.
$$

An upward radiating field has no incoming component from $z=+\infty$. For $q(\nu)=\sqrt{k^2-\nu^2}$, take the nonnegative real root when $|\nu|<k$ and the positive imaginary root when $|\nu|>k$. Consequently the [outgoing angular spectrum](../../../../../../outgoing-angular-spectrum.md) is

$$
\boxed{\psi_{\rm sc}(x,z)=\frac1{2\pi}\int_{\mathbb R}
\widehat\psi_{\rm sc}(\nu)e^{i\nu x+iq(\nu)z}\,d\nu}.
$$

The propagating terms go upward; the [evanescent](../../../../../../evanescent-wave.md) terms decay with increasing $z$. Grazing values are understood by a radiation limit.

There is a reference-plane qualification in the question. For an arbitrary rough surface the full line $z=0$ need not lie in the medium: already $f(x)=h>0$ puts it in vacuum. In that case the stated physical trace is undefined without continuation. The exact representation is obtained instead on a plane $z=z_*>\sup f$,

$$
\psi_{\rm sc}(x,z)=\frac1{2\pi}\int
\widehat\psi_*(\nu)e^{i\nu x+iq(\nu)(z-z_*)}\,d\nu,\qquad z\ge z_*.
$$

One can formally set $\widehat\psi_{\rm sc}=\widehat\psi_*e^{-iqz_*}$, but convergence of that continued spectrum down to the rough boundary is an additional assumption. This is the [reference-plane validity of a rough-surface angular spectrum](../../../../../../reference-plane-validity-of-a-rough-surface-angular-spectrum.md). The first boxed formula is exact in an appropriate homogeneous upper half-space; it is not automatically an exact representation at every point of a completely arbitrary rough domain. Small-height [perturbation theory](../../../../../../perturbation-theory.md) in part (c) uses the mean plane order by order.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 80](../../../paper-80-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
