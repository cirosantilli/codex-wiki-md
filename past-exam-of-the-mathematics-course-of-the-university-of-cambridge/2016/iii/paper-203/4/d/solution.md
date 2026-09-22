<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For the [SLE](../../../../../../schramm-loewner-evolution.md) driver $d\xi_t=\sqrt6\,dW_t$, apply the [Itô formula](../../../../../../ito-s-lemma.md) to $\widetilde\xi_t=\phi_t(\xi_t)$. At a fixed spatial point, $\phi_t$ has [finite variation](../../../../../../total-variation-of-a-function.md) locally in time by the derivative formula in part (c); there is no extra spatial martingale term. Consequently

$$
d\widetilde\xi_t
=\left(\dot\phi_t(\xi_t)+3\phi_t''(\xi_t)\right)dt
+\sqrt6\,\phi_t'(\xi_t)\,dW_t
=\sqrt6\,p_t\,dW_t.
$$

This exact cancellation is the [target-change locality of SLE6](../../../../../../target-change-locality-of-sle6.md). For a general parameter the [transformed SLE driving function](../../../../../../transformed-sle-driving-function.md) would have drift $(\kappa/2-3)\phi_t''(\xi_t)$.

Define the increasing clock and its inverse by

$$
a(t)=\int_0^tp_r^2\,dr=\frac12\operatorname{hcap}(\widetilde K_t),
\qquad t(s)=a^{-1}(s).
$$

The derivative $p_t$ is real and strictly positive before $T$, so this is a valid continuous [time change of a continuous process](../../../../../../time-change-of-a-continuous-process.md). The driver is a continuous [local martingale](../../../../../../local-martingale.md) with [quadratic variation](../../../../../../quadratic-variation.md) $[\widetilde\xi]_t=6a(t)$ and initial value zero. The [Dambis-Dubins-Schwarz theorem](../../../../../../dambis-dubins-schwarz-theorem.md) gives a standard [Brownian motion](../../../../../../brownian-motion-split.md) $\widehat W$ such that

$$
\widetilde\xi_{t(s)}=\sqrt6\,\widehat W_s,
\qquad 0\leq s<a(T-).
$$

If the terminal clock is finite, the Brownian motion may be extended beyond that stopping time; only its stopped part is used here. Reparameterizing the image maps gives

$$
\partial_s\widetilde g_{t(s)}(z)
=\frac2{\widetilde g_{t(s)}(z)-\sqrt6\,\widehat W_s},
\qquad\operatorname{hcap}(\widetilde K_{t(s)})=2s.
$$

These are exactly the defining [Chordal Loewner equation](../../../../../../chordal-loewner-equation.md) and [half-plane-capacity parameterization](../../../../../../half-plane-capacity-parameterization.md) for $\operatorname{SLE}_6$. The trace is $\widetilde\gamma_{t(s)}$. Hence **the image curve is also ordinary chordal $\operatorname{SLE}_6$ after this time change, up to the specified stopping time**:

$$
\boxed{\bigl(\widetilde\gamma_{t(s)}\bigr)_{0\leq s<a(T-)}
\text{ is stopped }\operatorname{SLE}_6\text{ in }(\mathbb H,0,\infty).}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 203](../../../paper-203-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
