<h1 id="1/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Write $\epsilon=l/d_i\ll1$ and $\delta=v_A\tau/l\ll1$. For magnetic amplitudes of order $B_0$, [ion](../../../../../../ion.md) acceleration is of order $v_A^2/l$. Thus its change over the fast time is

$$
\Delta u\sim\frac{v_A^2\tau}{l}=\delta v_A\ll v_A.
$$

The [ions](../../../../../../ion.md) are consequently fixed to leading order on this timescale. Their first nonzero response is driven by the momentum equation, with negligible self-advection for an initially resting [ion](../../../../../../ion.md) flow; one need not assert that the dimensional Lorentz acceleration literally vanishes. In fast-time, Alfvén-velocity dimensionless variables, the [ion](../../../../../../ion.md) equation reads $\partial_{\hat t}\hat{\mathbf u}=O(\delta)$, giving $\partial_{\hat t}\hat{\mathbf u}=0$ at leading order.

Meanwhile the electron-current velocity is $j/(en)\sim v_Ad_i/l=v_A/\epsilon$, larger than a bulk flow of order $v_A$. The ion-advection term in induction is smaller than Hall induction by $O(\epsilon)$ even if that slow flow is retained. The leading magnetic equation is therefore

$$
\boxed{\partial_t\mathbf B=-\frac c{4\pi en}\nabla\times[(\nabla\times\mathbf B)\times\mathbf B],\qquad\nabla\cdot\mathbf B=0,}
$$

with stationary [ions](../../../../../../ion.md) at leading order. This is the [fast-time electron-MHD limit of Hall magnetohydrodynamics](../../../../../../fast-time-electron-mhd-limit-of-hall-magnetohydrodynamics.md) and is precisely [electron magnetohydrodynamics](../../../../../../electron-magnetohydrodynamics.md).

The already obtained fast-wave eigenvector has $u/b=|q/\omega|\sim1/(kd_i)\ll1$, confirming that [ion](../../../../../../ion.md) motion cannot affect its leading frequency. The closed magnetic equation therefore suffices to obtain that branch without using momentum to close it. Its timescale is $\tau_w\sim1/(v_Ad_i|k_\parallel|k)$; compatibility with $\tau_w\ll l/v_A$ requires $|k_\parallel|d_i\gg1$ when $l\sim k^{-1}$. Arbitrarily small $k_\parallel$ can violate this fast-time assumption even though $kd_i\gg1$. The slow branch does not obey the stated ordering and is not retained by the fixed-ion reduction.

## ↑ Ancestors (11)

1. [5](../5.md)
2. [1](../../1.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
