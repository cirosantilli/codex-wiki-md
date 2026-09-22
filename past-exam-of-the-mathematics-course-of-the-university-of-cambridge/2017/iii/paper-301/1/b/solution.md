<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $D=\partial_\mu A^\mu$. The additional [gauge fixing](../../../../../../gauge-fixing.md) variation is $\delta(-D^2/2)=-D\partial_\mu\delta A^\mu$. [Integration by parts](../../../../../../integration-by-parts.md) gives the [Euler-Lagrange field equation](../../../../../../euler-lagrange-field-equation.md) $\partial_\mu F^{\mu\nu}+\partial^\nu D=0$, hence $\Box A^\nu=0$. This equation follows from the gauge-fixed density without imposing $D=0$ as a separate operator identity.

Direct differentiation of the density as printed gives the [canonical momentum](../../../../../../canonical-momentum.md) components conjugate to the lower-index fields:

$$
\boxed{\pi^\nu=\frac{\partial\mathcal L}{\partial\dot A_\nu}=-F^{0\nu}-\eta^{0\nu}D,\qquad \pi^0=-D,\quad\pi^i=\dot A_i-\partial_iA_0.}
$$

There is a boundary-term convention to reconcile with part (c). The [Feynman-gauge Maxwell kinetic density after a boundary-term subtraction](../../../../../../feynman-gauge-maxwell-kinetic-density-after-a-boundary-term-subtraction.md) is

$$
\mathcal L'=-\frac12\partial_\mu A_\nu\partial^\mu A^\nu,
\qquad
\mathcal L=\mathcal L'+\partial_\mu K^\mu,
\qquad
K^\mu=\frac12\bigl(A_\nu\partial^\nu A^\mu-A^\mu D\bigr).
$$

It has the same [Euler-Lagrange field equations](../../../../../../euler-lagrange-field-equation.md), but its [canonical momentum](../../../../../../canonical-momentum.md) components are $\pi'^\nu=-\dot A^\nu$. The mode expansion supplied in part (c) is the expansion of these latter momenta. Thus it is valid after the stated boundary-term subtraction; it is not the direct derivative of the original density. For example, a time-independent spatially varying $A_0$ with $A_i=0$ gives $\pi^i=-\partial_iA_0$ but $\pi'^i=0$.

The [boundary-term shift of canonical field momenta](../../../../../../boundary-term-shift-of-canonical-field-momenta.md) is a [canonical transformation](../../../../../../canonical-transformation.md). If spatial boundary terms vanish, $B=\int d^3x\,K^0=\int d^3x\,A_0\partial_iA_i$, and $\pi^\nu=\pi'^\nu+\delta B/\delta A_\nu$. This explains why the two conventions have the same dynamics while their [momentum](../../../../../../momentum.md) formulas differ.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 301](../../../paper-301-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
