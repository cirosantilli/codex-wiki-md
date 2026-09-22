<h1 id="3/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

In the lower uniform [half-space](../../../../../../half-space.md) the [causal vertical wavenumber branch](../../../../../../causal-vertical-wavenumber-branch.md) has $\operatorname{Im}k_{\beta,b}>0$. The downward factor $e^{ik_{\beta,b}(z-z_b)}$ decays as $z\to+\infty$, whereas the upward factor grows there and represents an incoming wave from the lower infinity. The outgoing [radiation condition](../../../../../../radiation-condition.md) therefore retains only the downward factor and gives

$$
\boxed{Z(z_b)=q_b=\mu_bp_{\beta,b}.}
$$

For each uniform layer $j$ of thickness $h_j$, work upwards from its known bottom load $Z_{j,b}$. With $q_j=\mu_jp_{\beta,j}$ and $\delta_j=\omega p_{\beta,j}h_j$, part (iv) gives

$$
\boxed{Z_{j,t}=\frac{Z_{j,b}\cos\delta_j-iq_j\sin\delta_j}
{\cos\delta_j-i(Z_{j,b}/q_j)\sin\delta_j}.}
$$

[velocity](../../../../../../velocity.md) and [traction](../../../../../../traction.md) are continuous across a bonded interface, so this top impedance becomes the bottom load of the next shallower layer. Repeat up to $z_a$ to obtain $Z_{\rm in}=Z(z_a)$. Poles can be handled by carrying $(V,T)$ or the reciprocal ratio. Since the lower load has positive real part, part (iii) actually ensures that the outgoing whole-stack impedance stays finite with positive real part at all shallower depths in the upper [frequency](../../../../../../frequency.md) half-plane.

The upper [half-space](../../../../../../half-space.md) has directional impedance $q_a=\mu_ap_{\beta,a}$. At $z_a$, an incident [velocity](../../../../../../velocity.md) $V_0$ and reflected [velocity](../../../../../../velocity.md) $RV_0$ give

$$
V(z_a)=V_0(1+R),\qquad T(z_a)=-q_aV_0(1-R).
$$

Taking their ratio and solving establishes [reflection from a layered SH impedance](../../../../../../reflection-from-a-layered-sh-impedance.md):

$$
Z_{\rm in}=q_a\frac{1-R}{1+R},\qquad
\boxed{R=\frac{q_a-Z_{\rm in}}{q_a+Z_{\rm in}}.}
$$

Thus no individual deeper reflection coefficients are needed after $Z_{\rm in}$ is known: it contains all underlying interfaces and their coherent multiples. A matched load gives $R=0$; the real-frequency limits of zero [traction](../../../../../../traction.md) and zero [velocity](../../../../../../velocity.md) give $R=+1$ and $R=-1$. For real [frequency](../../../../../../frequency.md) and propagating upper and lower [half-space](../../../../../../half-space.md) waves, the usual energy-flux balance provides a further check on the computed reflection and transmission. A stable implementation for thick layers uses the ratio update or its decaying-exponential version instead of multiplying growing transfer [matrices](../../../../../../matrix.md).

## ↑ Ancestors (11)

1. [V](../v.md)
2. [3](../../3.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
