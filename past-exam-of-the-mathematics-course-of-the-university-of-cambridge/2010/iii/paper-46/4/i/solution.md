<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take metric signature $(+---)$ and the [Fourier transform](../../../../../../fourier-transform.md) convention $e^{-ipx}$. Introduce an even source $J$ for the gauge field and odd sources $\eta,\bar\eta$ for the [Faddeev-Popov ghost field](../../../../../../faddeev-popov-ghost.md):

$$
Z[J,\bar\eta,\eta]=\frac1{Z[0]}\int\mathcal DA\,\mathcal D\bar c\,\mathcal Dc\,\exp\left[iS+i\int d^4x\,(J^{a\mu}A_\mu^a+\bar\eta^ac^a+\bar c^a\eta^a)\right].
$$

At tree level the two-point functions come from the quadratic action. Integrating the gauge kinetic term by parts gives its momentum-space kernel

$$
K_{\mu\nu}^{ab}(p)=\delta^{ab}\left[-p^2g_{\mu\nu}+(1-\zeta^{-1})p_\mu p_\nu\right].
$$

Its inverse follows from transverse and longitudinal projectors: $K=-p^2(P_T+\zeta^{-1}P_L)$, so $K^{-1}=-p^{-2}(P_T+\zeta P_L)$. Completing the bosonic Gaussian square gives $Z_0[J]=\exp[-iJK_F^{-1}J/2]$, with the [Feynman i-epsilon prescription](../../../../../../feynman-i-epsilon-prescription.md) in the inverse. Two source derivatives and their insertion factors give the [gauge-boson propagator](../../../../../../gauge-boson-propagator.md) $D_F=iK_F^{-1}$. Hence

$$
\boxed{\langle\Omega|T A_\mu^a(x)A_\nu^b(y)|\Omega\rangle=\delta^{ab}\int\frac{d^4p}{(2\pi)^4}e^{-ip(x-y)}\frac{-i}{p^2+i0}\left[g_{\mu\nu}-(1-\zeta)\frac{p_\mu p_\nu}{p^2+i0}\right].}
$$

For $\zeta=1$ this reduces to the [Feynman-gauge adjoint propagator](../../../../../../feynman-gauge-adjoint-propagator.md). The longitudinal double pole is understood with the compatible Feynman boundary prescription.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
