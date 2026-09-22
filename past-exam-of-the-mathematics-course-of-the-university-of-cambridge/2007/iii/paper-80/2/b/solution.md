<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a complex harmonic field use [complex conjugation](../../../../../../complex-conjugation.md) in its [wave-field correlation](../../../../../../uncentered-wave-field-correlation.md): $m=\langle\psi_{\rm sc}(x_1,z)\psi_{\rm sc}(x_2,z)^*\rangle$. Put $A(\nu)=\widehat\psi_{\rm sc}(\nu)$ and let $C(\nu,\nu')=\langle A(\nu)A(\nu')^*\rangle$. Direct substitution of part (a), before imposing any homogeneity, gives

$$
\langle\psi_{\rm sc}(x_1,z)\psi_{\rm sc}(x_2,z)^*\rangle
=\frac1{(2\pi)^2}\iint C(\nu,\nu')
e^{i\nu x_1-i\nu'x_2+i[q(\nu)-q(\nu')^*]z}\,d\nu\,d\nu'.
$$

This is the general answer. It need not depend only on $\xi=x_1-x_2$: even a deterministic sum of two distinct outgoing [plane waves](../../../../../../plane-wave.md) has cross terms depending on the midpoint. The requested separation-only [wave-field correlation](../../../../../../uncentered-wave-field-correlation.md) therefore presumes translation-homogeneous two-point statistics.

Under that assumption define the uncentered spectrum by $C(\nu,\nu')=2\pi S(\nu)\delta(\nu-\nu')$. Then the [height propagation of an angular-spectrum correlation](../../../../../../height-propagation-of-an-angular-spectrum-correlation.md) is

$$
\boxed{m(\xi,z)=\frac1{2\pi}\int_{\mathbb R}
S(\nu)e^{i\nu\xi-2\operatorname{Im}q(\nu)z}\,d\nu}.
$$

Equivalently, for the [spectral measure of a stationary random field](../../../../../../spectral-measure-of-a-stationary-random-field.md) $F(d\nu)=S(\nu)d\nu/(2\pi)$, write $m=\int e^{i\nu\xi-2\operatorname{Im}qz}F(d\nu)$. This version includes coherent spectral atoms and avoids squaring [Dirac delta functions](../../../../../../dirac-delta-function.md). The propagating spectrum $|\nu|\le k$ is independent of height, while an [evanescent](../../../../../../evanescent-wave.md) contribution is multiplied by $e^{-2\sqrt{\nu^2-k^2}z}$. At $\xi=0$ the formula gives the [mean wave intensity](../../../../../../ensemble-averaged-wave-intensity.md).

If the brackets instead mean the spatial autocorrelation of a finite-energy deterministic field, define $m_L(\xi,z)=\int\psi_{\rm sc}(x+\xi,z)\psi_{\rm sc}(x,z)^*dx$. [Parseval's identity](../../../../../../parseval-identity.md) gives the same integral with $S(\nu)=|\widehat\psi_{\rm sc}(\nu)|^2$. That finite-energy formula must not be applied unmodified to an infinite stationary field or an infinite [plane wave](../../../../../../plane-wave.md), whose transforms require a spectral-measure convention.

## ↑ Ancestors (11)

1. [B](../b.md)
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
