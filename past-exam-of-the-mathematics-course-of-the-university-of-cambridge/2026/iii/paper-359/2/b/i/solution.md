<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The second estimate in part (a) bounds $(\omega_m)$ in $H^2_{\rm per}$. The periodic [Poisson equation](../../../../../../../poisson-equation.md) $-\Delta\Psi_m=\omega_m$ and the supplied curl identity then bound $(\Psi_m)$ in $H^4_{\rm per}$ and $(u_m)$ in $H^3_{\rm per}$. After passing to a subsequence,

$$
\omega_m\rightharpoonup\omega\ \hbox{in }H^2,
\qquad
\Psi_m\rightharpoonup\Psi\ \hbox{in }H^4,
\qquad
u_m\rightharpoonup u\ \hbox{in }H^3.
$$

The [Rellich-Kondrachov compactness theorem](../../../../../../../rellich-kondrachov-theorem.md) also gives strong convergence in the corresponding spaces with one fewer derivative. In particular, $u_m\to u$ in $L^\infty$ and $\nabla\omega_m\to\nabla\omega$ in $L^2$, so

$$
(u_m\mathbin\cdot\nabla)\omega_m
\longrightarrow(u\mathbin\cdot\nabla)\omega
\quad\hbox{in }L^2.
$$

Passing to the limit in the Galerkin equations gives

$$
-\nu\Delta\omega+\gamma\omega+(u\mathbin\cdot\nabla)\omega=g,
\qquad
u=\nabla^\perp\Psi,
\qquad
-\Delta\Psi=\omega.
$$

These identities have the claimed [Sobolev regularity](../../../../../../../sobolev-space-split.md), and the first holds in $L^2_{\rm per}$. Finally, the [weak lower semicontinuity of the Hilbert norm](../../../../../../../weak-lower-semicontinuity-of-the-hilbert-norm.md) preserves the estimates

$$
\boxed{\nu\|\Delta\omega\|_2^2\leq R_2^2,
\qquad
\gamma\|\nabla\omega\|_2^2\leq R_2^2}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 359](../../../../paper-359-split.md)
5. [Iii](../../../../split.md)
6. [2026](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
