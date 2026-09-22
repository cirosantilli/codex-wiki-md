<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Route a directed [ghost loop](../../../../../ghost-loop.md) so that its internal [four-momenta](../../../../../four-momentum.md) are $l$ and $l+k$. At the external [gluon](../../../../../gluon.md) with indices $(\mu,a)$, let the incoming ghost carry colour $c$ and the outgoing ghost carry colour $d$; the other [Feynman vertex](../../../../../interaction-vertex.md) has the reverse order. The stated ghost-gluon [Feynman rules](../../../../../feynman-rules.md) supply $g_D^2f^{acd}f^{bdc}(l+k)^\mu l^\nu$. Their [colour factor](../../../../../color-factor.md) is

$$
f^{acd}f^{bdc}=-C_A\delta^{ab}.
$$

The two [ghost propagators](../../../../../ghost-propagator.md) supply $i^2=-1$, while the closed [ghost loop](../../../../../ghost-loop.md) supplies another $-1$. Thus, with the insertion convention stated above,

$$
i\Pi_{\mathrm{gh}}^{\mu\nu,ab}=-g_D^2C_A\delta^{ab}I^{\mu\nu},\qquad
I^{\mu\nu}=\int\frac{d^Dl}{(2\pi)^D}\frac{(l+k)^\mu l^\nu}{(l^2+i0)((l+k)^2+i0)}.
$$

This establishes every prefactor before integration. To isolate its [ultraviolet pole](../../../../../ultraviolet-pole.md), take generic [off shell](../../../../../off-shell.md) $k$, initially $k^2<0$, so the massless integral has no overlapping [infrared divergence](../../../../../infrared-divergence.md). Introduce a [Feynman parameter](../../../../../feynman-parameter.md), shift $r=l+xk$, and set $\Delta=-x(1-x)k^2>0$. Odd powers of $r$ vanish, giving

$$
I^{\mu\nu}=\int_0^1dx\left[\frac{g^{\mu\nu}}{D}\int\frac{d^Dr}{(2\pi)^D}\frac{r^2}{(r^2-\Delta+i0)^2}-x(1-x)k^\mu k^\nu\int\frac{d^Dr}{(2\pi)^D}\frac1{(r^2-\Delta+i0)^2}\right].
$$

The needed [dimensional regularization](../../../../../dimensional-regularization.md) integrals follow from the supplied [gamma function](../../../../../gamma-function.md) formula. In $D=4-\epsilon$,

$$
\begin{aligned}
J_1(\Delta)&=\int\frac{d^Dr}{(2\pi)^D}\frac1{r^2-\Delta+i0}
=\frac{i\Delta}{16\pi^2}\frac2\epsilon+O(1),\\
J_2(\Delta)&=\int\frac{d^Dr}{(2\pi)^D}\frac1{(r^2-\Delta+i0)^2}
=\frac{i}{16\pi^2}\frac2\epsilon+O(1),\\
\int\frac{d^Dr}{(2\pi)^D}\frac{r^2}{(r^2-\Delta+i0)^2}&=J_1+\Delta J_2=\frac{i}{16\pi^2}\frac{4\Delta}{\epsilon}+O(1).
\end{aligned}
$$

Here $\Gamma(\epsilon/2)=2/\epsilon+O(1)$, rather than $1/\epsilon$. Using $1/D=1/4+O(\epsilon)$ and $\int_0^1x(1-x)\,dx=1/6$, obtain

$$
I^{\mu\nu}\big|_{\mathrm{UV}}=-\frac{i}{96\pi^2\epsilon}\left(k^2g^{\mu\nu}+2k^\mu k^\nu\right).
$$

Therefore the [ghost-loop pole of the gluon self-energy](../../../../../ghost-loop-pole-of-the-gluon-self-energy.md) is

$$
\boxed{\Pi_{\mathrm{gh}}^{\mu\nu,ab}\big|_{\mathrm{UV}}=\frac{g^2C_A\delta^{ab}}{96\pi^2\epsilon}\left(k^2g^{\mu\nu}+2k^\mu k^\nu\right).}
$$

The factor $\mu^\epsilon$ in $g_D^2$ affects only finite terms at this order. The isolated [ghost loop](../../../../../ghost-loop.md) is not transverse: contracting this result gives $g^2C_A\delta^{ab}k^2k^\nu/(32\pi^2\epsilon)$. Transversality is a condition on the complete [gluon self-energy](../../../../../gluon-self-energy.md), including the other loop graphs.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2019](../../../../2019-split.md)
5. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../../split.md)
6. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Mathematical and theoretical physics course of the University of Oxford](../../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
