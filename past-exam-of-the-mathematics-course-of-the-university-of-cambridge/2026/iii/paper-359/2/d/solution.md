<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For each $\nu>0$, choose the solution from parts (a)--(c). The maximum estimate gives a $\nu$-independent bound

$$
\|\omega_\nu\|_\infty\leq\gamma^{-1}\|g\|_\infty.
$$

Thus a sequence $\nu_j\downarrow0$ has $\omega_{\nu_j}\rightharpoonup^\ast\omega$ in $L^\infty$. The periodic elliptic estimates for

$$
-\Delta\Psi_{\nu_j}=\omega_{\nu_j},
\qquad
u_{\nu_j}=\nabla^\perp\Psi_{\nu_j}
$$

bound $\Psi_{\nu_j}$ in $W^{2,p}$ and $u_{\nu_j}$ in $W^{1,p}$ for every finite $p$. Taking $p>2$ and using compact [Sobolev embedding](../../../../../../failure-of-first-order-sobolev-embedding-into-linfinity-in-two-dimensions.md) gives, after a further subsequence, uniform convergence $u_{\nu_j}\to u$. It follows that $u_{\nu_j}\omega_{\nu_j}\rightharpoonup u\omega$ distributionally.

The first energy estimate gives

$$
\|\nu_j\nabla\omega_{\nu_j}\|_2
\leq\sqrt{\nu_j}\,R_1\longrightarrow0.
$$

Therefore the viscous term vanishes in $H^{-1}$, and the weak formulation passes to the limit as

$$
\boxed{\gamma\omega+\nabla\mathbin\cdot(u\omega)=g}.
$$

The elliptic relations pass to the limit as well and give

$$
u=\nabla^\perp\Psi,\qquad-\Delta\Psi=\omega.
$$

Since $\omega\in L^\infty\subset L^2$, periodic elliptic regularity gives $\Psi\in H^2_{\rm per}$ and $u\in H^1_{\rm per}\cap H$. Moreover $u\omega\in L^2$, so its divergence lies in $H^{-1}_{\rm per}$. This constructs the required weak solution of the damped-driven Euler system by a [vanishing-viscosity limit](../../../../../../vanishing-viscosity-limit.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 359](../../../paper-359-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
