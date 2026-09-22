<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Here the otherwise undefined printed domain $H$ must mean $D=\mathbb H\setminus K$. Let the [Brownian motion](../../../../../../brownian-motion-split.md) start at $z\in D$, and let $\tau_R$ stop it on reaching height $R$ or leaving $D$. Take $R>\max(\operatorname{Im}z,\sup_K\operatorname{Im}w)$. This stopping time is finite almost surely, since it is no later than exit of its imaginary coordinate from $(0,R)$.

By part (d), $0\leq v(w)\leq R$ in the stopped domain. Its finite-boundary values vanish except on the top boundary, by the argument of part (d). Localization and the [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) for this bounded harmonic [martingale](../../../../../../martingale-split.md) therefore give

$$
v(z)=\mathbb E_z\bigl[v(B_{\tau_R})\,1_{\{\operatorname{Im}B_{\tau_R}=R\}}\bigr].
$$

Write $p_R=\mathbb P_z(\operatorname{Im}B_{\tau_R}=R)$ and use the uniform displacement bound $M$ from part (c). On the top boundary, $|v(w)-R|\leq M$, hence

$$
|v(z)-Rp_R|\leq Mp_R.
$$

The stopped imaginary coordinate is itself a bounded [martingale](../../../../../../martingale-split.md). Since its exit height is nonnegative,

$$
\operatorname{Im}z=\mathbb E_z[\operatorname{Im}B_{\tau_R}]\geq Rp_R.
$$

Consequently $|v(z)-Rp_R|\leq M\operatorname{Im}z/R\to0$, proving the [high-level escape representation of a mapping-out height](../../../../../../high-level-escape-representation-of-a-mapping-out-height.md):

$$
\boxed{\operatorname{Im}g_K(z)=\lim_{R\to\infty}R\,\mathbb P_z(\operatorname{Im}B_{\tau_R}=R).}
$$

If $H$ instead meant the whole upper half-plane, the right side would always be $\operatorname{Im}z$. For example, the [mapping-out function of a vertical slit](../../../../../../mapping-out-function-of-a-vertical-slit.md) $K=(0,ia]$ is $g_K(w)=\sqrt{w^2+a^2}$ with branch asymptotic to $w$; at $z=iy$, $y>a$, its height is $\sqrt{y^2-a^2}<y$. This demonstrates why killing on the hull is essential to the printed formula.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
