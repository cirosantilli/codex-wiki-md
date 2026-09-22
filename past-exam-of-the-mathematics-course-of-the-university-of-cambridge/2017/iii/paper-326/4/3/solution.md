<h1 id="4/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Because $w_k\geq c>0$, a finite sum $\sum_kw_k|u_k|$ implies $u\in\ell^1$. Thus the printed [weighted one-norm on l2](../../../../../../weighted-one-norm-on-l2.md) equals the extended nonnegative sum on every $u\in\ell^2$. Unbounded weights may make that sum infinite for some $u\in\ell^1$; membership in $\ell^1$ alone is not a finiteness assertion.

For each $N$, $J_N(u)=\sum_{k=1}^Nw_k|u_k|$ is continuous in the [l2 sequence space](../../../../../../l2-sequence-space.md), and $J=\sup_NJ_N$. If $u^{(n)}\to u$ in [norm](../../../../../../norm.md), then for every $N$,

$$
J_N(u)=\lim_nJ_N(u^{(n)})\leq\liminf_nJ(u^{(n)}).
$$

Taking the supremum over $N$ proves

$$
\boxed{J(u)\leq\liminf_nJ(u^{(n)}).}
$$

It is also weakly lower semicontinuous by the same finite-coordinate argument, and convex and proper because zero and finite sequences have finite penalty.

At a finite-penalty base point $v$, coordinate variations give the [subdifferential of a weighted one-norm on l2](../../../../../../subdifferential-of-a-weighted-one-norm-on-l2.md):

$$
p\in\partial J(v)\iff p\in\ell^2,\quad p_k=w_k\operatorname{sign}(v_k)\ (v_k\ne0),\quad |p_k|\leq w_k\ (v_k=0).
$$

These conditions are sufficient by summing the coordinate supporting inequalities. Since $w_k\geq c$, an infinitely supported $v$ would require infinitely many $|p_k|\geq c$, contradicting $p\in\ell^2$. Thus a finite-penalty point can have empty [subdifferential](../../../../../../subdifferential.md); a Bregman base with an actual [subgradient](../../../../../../subgradient.md) must be finitely supported.

For any such $p$, $\langle p,v\rangle=J(v)$ and the [Bregman distance](../../../../../../bregman-divergence.md) simplifies to

$$
\boxed{D_J^p(u,v)=J(u)-\langle p,u\rangle=\sum_{k\geq1}(w_k|u_k|-p_ku_k).}
$$

Each summand is nonnegative; the sum may be infinite. The pairing converges by [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md). This definition does not silently assume a [subgradient](../../../../../../subgradient.md) exists at every $v\in\ell^1$.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [4](../../4.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
