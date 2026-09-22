<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use a [mass counterterm](../../../../../../mass-counterterm.md) and a [wavefunction renormalization](../../../../../../wave-function-renormalization.md) counterterm, defining their additive coefficients by

$$
\mathcal L_{\mathrm{ct}}=\frac12\delta Z(\partial\phi)^2+\frac12\delta m^2\phi^2,\qquad
\delta K(k)=\delta Z k^2+\delta m^2.
$$

The sign follows from how the [Euclidean path integral](../../../../../../euclidean-path-integral.md) expands. A quadratic [counterterm](../../../../../../counterterm.md) inserts $-\delta K$ into the propagator, whereas the loop defined in the question inserts $+I$. To this order,

$$
D(k)=D_0(k)+D_0(k)^2[I(k)-\delta K(k)]+\cdots,
\qquad D(k)^{-1}=k^2+m^2-I(k)+\delta K(k)+\cdots.
$$

Thus cancellation requires $\delta K=I_{\mathrm{div}}$, rather than its negative. In the [minimal subtraction scheme](../../../../../../minimal-subtraction-scheme.md), with no finite parts added,

$$
\boxed{\delta Z=-\frac{g^2}{6(4\pi)^3\epsilon},\qquad
\delta m^2=-\frac{g^2m^2}{(4\pi)^3\epsilon}.}
$$

These are the [minimal-subtraction two-point counterterms in cubic scalar theory](../../../../../../minimal-subtraction-two-point-counterterms-in-cubic-scalar-theory.md). They absorb respectively the $k^2$ and constant terms in the two-point pole.

The additive mass coefficient is distinct from the shift of a bare mass when the bare field also includes [wavefunction renormalization](../../../../../../wave-function-renormalization.md). If $\phi_B=\sqrt{1+\delta Z}\,\phi$ and $(1+\delta Z)m_B^2=m^2+\delta m^2$, then to one-loop order

$$
m_B^2-m^2=\delta m^2-m^2\delta Z=-\frac{5g^2m^2}{6(4\pi)^3\epsilon}.
$$

This last relation specifies the convention; the boxed coefficients are those multiplying the local [counterterms](../../../../../../counterterm.md) displayed above.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
