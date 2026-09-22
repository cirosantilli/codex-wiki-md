<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For an autonomous [Lagrangian](../../../../../../lagrangian.md), the [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md) uses

$$
\frac{\delta A}{\delta x}=L_x-\frac{d}{dt}L_{\dot x},
\qquad H=\dot xL_{\dot x}-L.
$$

Apply the [chain rule](../../../../../../chain-rule.md) to the [Hamiltonian](../../../../../../hamiltonian.md) along an arbitrary smooth path, without assuming the unforced [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md):

$$
\frac{dH}{dt}
=\ddot xL_{\dot x}+\dot x\frac{d}{dt}L_{\dot x}
-L_x\dot x-L_{\dot x}\ddot x
=-\dot x\frac{\delta A}{\delta x}.
$$

Consequently the [energy balance for an autonomous Lagrangian](../../../../../../energy-balance-for-an-autonomous-lagrangian.md) is

$$
\boxed{-\int_{t_1}^{t_2}\dot x\frac{\delta A}{\delta x(t)}\,dt=H_2-H_1}.
$$

With explicit time dependence, an additional $-\partial_tL$ enters $dH/dt$. For ideal [Gaussian white noise](../../../../../../gaussian-white-noise.md), the identity is understood through smooth-noise regularization or the [Stratonovich chain rule](../../../../../../stratonovich-chain-rule.md). The original PDF correctly differentiates $L$ with respect to $\dot x$ in $H$; the supplied TeX's derivative with respect to $x$, its endpoint $t^2$, and its ordinary derivative of $A$ are transcription errors.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
