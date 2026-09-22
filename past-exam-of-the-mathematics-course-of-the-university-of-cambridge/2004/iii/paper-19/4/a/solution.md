<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

There is a normalization issue in the printed constant. Let $\operatorname{Ric}_{\mathrm{tr}}$ denote the trace convention in the catalog's [Ricci curvature](../../../../../../ricci-curvature.md), and write $\overline{\operatorname{Ric}}=\operatorname{Ric}_{\mathrm{tr}}/(n-1)$ for [normalized Ricci curvature](../../../../../../normalized-ricci-curvature.md), with $n\geq2$. The claimed $\pi/\sqrt k$ bound corresponds to $\overline{\operatorname{Ric}}\geq kg$, or equivalently $\operatorname{Ric}_{\mathrm{tr}}\geq(n-1)kg$. We prove the estimate in both conventions.

Take a unit-speed [minimizing geodesic](../../../../../../minimizing-geodesic.md) of length $L>0$ and perpendicular parallel orthonormal fields $E_1,\ldots,E_{n-1}$. Set $V_i(t)=\sin(\pi t/L)E_i(t)$. The fields vanish at the endpoints. The allowed [second variation of geodesic energy](../../../../../../second-variation-of-geodesic-energy.md) makes each [Riemannian index form](../../../../../../riemannian-index-form.md) nonnegative. Summing them gives

$$
\begin{aligned}
0\leq\sum_i I(V_i,V_i)
&=\int_0^L\left((n-1)\frac{\pi^2}{L^2}\cos^2(\pi t/L)
-\operatorname{Ric}_{\mathrm{tr}}(\dot\gamma,\dot\gamma)\sin^2(\pi t/L)\right)dt\\
&\leq\frac{n-1}{2}\left(\frac{\pi^2}{L}-kL\right)
\end{aligned}
$$

under the normalized lower bound. Thus $L\leq\pi/\sqrt k$. Completeness and the [Hopf-Rinow theorem](../../../../../../hopf-rinow-theorem.md) supply a [minimizing geodesic](../../../../../../minimizing-geodesic.md) between any two points, so this bounds the diameter. A closed ball of that radius about any point contains the whole manifold and is [compact](../../../../../../compact-space.md), again by the [Hopf-Rinow theorem](../../../../../../hopf-rinow-theorem.md).

Hence the intended [Bonnet-Myers theorem](../../../../../../myers-s-theorem.md) conclusion is

$$
\boxed{\overline{\operatorname{Ric}}\geq kg\ \Longrightarrow\ M\text{ compact},\quad\operatorname{diam}M\leq\frac\pi{\sqrt k}.}
$$

If the printed $\operatorname{Ric}\geq k$ means trace Ricci curvature instead, the same integral has lower curvature term $kL/2$ and yields

$$
\boxed{\operatorname{Ric}_{\mathrm{tr}}\geq kg\ \Longrightarrow\ \operatorname{diam}M\leq\pi\sqrt{\frac{n-1}{k}}.}
$$

The smaller bound is false under that convention when $n>2$: the round unit $S^n$ has trace Ricci tensor $(n-1)g$ and diameter $\pi$. Taking $k=n-1$ contradicts the printed $\pi/\sqrt k$ inequality. The [compactness](../../../../../../compact-space.md) assertion remains true.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 19](../../../paper-19-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
