<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let the positive real material parameters depend on $x$ but not on time. Define the [flux-normalized elastic characteristic amplitudes](../../../../../../flux-normalized-elastic-characteristic-amplitudes.md) and logarithmic [seismic impedance](../../../../../../seismic-impedance.md) [gradient](../../../../../../gradient.md)

$$
\phi_\pm=\frac12\left(\sqrt Z\,v\mp\frac{\sigma}{\sqrt Z}\right),\qquad g=\frac12\frac{d\log Z}{dx}.
$$

Write $P=\phi_++\phi_-$ and $Q=\phi_+-\phi_-$. Then $v=Z^{-1/2}P$, $\sigma=-Z^{1/2}Q$, and direct substitution gives

$$
P_t=-\beta(Q_x+gQ),\qquad Q_t=-\beta(P_x-gP).
$$

For example, the first relation uses $(Z^{1/2})'=gZ^{1/2}$ and $Z/\rho=\beta$; the second uses $\mu/Z=\beta$. Adding and subtracting now proves

$$
\boxed{\partial_x\phi_++\beta^{-1}\partial_t\phi_+=g\phi_-,\qquad \partial_x\phi_--\beta^{-1}\partial_t\phi_-=g\phi_+.}
$$

The original PDF has these two first-order equations. The TeX mistakenly combines them into ratios, which must not be used. A [seismic impedance](../../../../../../seismic-impedance.md) [gradient](../../../../../../gradient.md) couples forward and backward [wave amplitudes](../../../../../../wave-amplitude.md) even when the local [wave speed](../../../../../../wave-speed.md) is allowed to vary.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 82](../../../paper-82-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
