<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $V=4\pi R^3/3$, $w_p=w(Z)$ and $\rho_p=\rho(Z)$, with the subscript $p$ here referring to the plume fluid. The section at $Z(t)$ moves upward at $U=\dot Z$. Its incoming [volume flux](../../../../../../../volumetric-flow-rate.md) relative to that moving section is therefore

$$
J=\pi B^2(w_p-U).
$$

The thermal's sectional model allows no direct ambient [fluid entrainment](../../../../../../../fluid-entrainment.md), so its volume and mass balances are

$$
\boxed{\dot V=J,\qquad \frac{d}{dt}(\rho_tV)=\rho_pJ.}
$$

Subtracting these balances with $g_t=g(\rho_0-\rho_t)/\rho_0$ and $g_p=g(\rho_0-\rho_p)/\rho_0$ gives the [buoyant thermal mass balance](../../../../../../../buoyant-thermal-mass-balance.md)

$$
\frac{d}{dt}(g_tV)=g_pJ=g_p\dot V.
$$

For the [self-similar starting plume](../../../../../../../self-similar-starting-plume.md), $V\propto t^{9/4}$ and $g_t\propto t^{-5/4}$, so $g_tV\propto t$. Hence

$$
\frac{g_tV}{t}=g_p\frac94\frac Vt,\qquad
\boxed{g_t=\frac94g_p.}
$$

Using $\pi B^2w_p$ instead of the relative inflow would miss the volume swept out by the rising matching section. The larger thermal [reduced gravity](../../../../../../../reduced-gravity-split.md) reflects fluid accumulated from earlier, lower, more buoyant parts of the plume.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Paper 345](../../../../paper-345-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
