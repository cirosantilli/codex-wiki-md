<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a [harmonic function](../../../../../../harmonic-function.md) $u$ on $\mathbb C\cong\mathbb R^2$, the [Itô formula](../../../../../../ito-s-lemma.md) gives

$$
u(B_t)=u(B_0)+\int_0^t\nabla u(B_s)\cdot dB_s+\frac12\int_0^t\Delta u(B_s)ds=u(B_0)+\int_0^t\nabla u(B_s)\cdot dB_s.
$$

Stop on leaving increasing discs and at increasing deterministic times. On each such interval the [gradient](../../../../../../gradient.md) is bounded, so the [stochastic integral](../../../../../../stochastic-integral.md) is a [martingale](../../../../../../martingale-split.md). This proves that **$u(B)$ is a [continuous local martingale](../../../../../../continuous-local-martingale.md)**.

If $|u|\leq K$, this is a bounded [local martingale](../../../../../../local-martingale.md) and hence a true [martingale](../../../../../../martingale-split.md). Start [Brownian motion](../../../../../../brownian-motion-split.md) at an arbitrary $z$. Its [Gaussian heat kernel](../../../../../../gaussian-heat-kernel.md) gives

$$
u(z)=\mathbb E_z u(B_t)=\int_{\mathbb R^2}u(v)p_t(v-z)dv,\qquad p_t(v)=\frac1{2\pi t}e^{-|v|^2/(2t)}.
$$

For a unit vector $e$, $\partial_e p_t(v)=-(e\cdot v)p_t(v)/t$, so $\int|\partial_ep_t(v)|dv=\sqrt{2/\pi}/\sqrt t$. Integrating the directional derivative along the segment from $z$ to $w$ yields

$$
|u(z)-u(w)|\leq K\int|p_t(v-z)-p_t(v-w)|dv\leq K\sqrt{\frac2\pi}\frac{|z-w|}{\sqrt t}.
$$

Letting $t\to\infty$ gives **the [harmonic Liouville theorem](../../../../../../harmonic-liouville-theorem.md)**:

$$
\boxed{u(z)=u(w)\text{ for all }z,w\in\mathbb C;\quad u\text{ is constant}.}
$$

This [Gaussian heat-kernel proof of the harmonic Liouville theorem](../../../../../../gaussian-heat-kernel-proof-of-the-harmonic-liouville-theorem.md) uses the bounded [martingale](../../../../../../martingale-split.md) identity established above.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
