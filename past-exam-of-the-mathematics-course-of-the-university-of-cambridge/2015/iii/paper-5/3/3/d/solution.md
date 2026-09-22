<h1 id="3/3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Set $q_i=2\alpha^i$, $r_i=1/2+2^{-i-1}$ and $N_i=\|u\|_{L^{q_i}(B_{r_i})}$. Then $r_0=1$, $r_i-r_{i+1}=2^{-i-2}$, and the sharper [uniform power gain for elliptic solutions](../../../../../../../uniform-power-gain-for-elliptic-solutions.md) gives

$$
N_{i+1}\le\bigl[D_\ell R\,2^{i+2}\bigr]^{\alpha^{-i}}N_i.
$$

The [Moser product on geometric radii](../../../../../../../moser-product-on-geometric-radii.md) converges because

$$
S_0=\sum_{i\ge0}\alpha^{-i}=\frac\alpha{\alpha-1},\qquad S_1=\sum_{i\ge0}(i+2)\alpha^{-i}=\frac\alpha{(\alpha-1)^2}+\frac{2\alpha}{\alpha-1}.
$$

Thus every $N_i$ is at most $B=(D_\ell R)^{S_0}2^{S_1}\|u\|_{L^2(B_1)}$. Since $B_{1/2}\subset B_{r_i}$, its $L^{q_i}$ norms are also bounded by $B$. If $u>B+\delta$ on a set of positive measure $m$ in $B_{1/2}$, these norms are at least $(B+\delta)m^{1/q_i}$, tending to $B+\delta$, a contradiction. Hence

$$
\boxed{\|u\|_{L^\infty(B_{1/2})}\le(D_\ell R)^{\alpha/(\alpha-1)}2^{\alpha/(\alpha-1)^2+2\alpha/(\alpha-1)}\|u\|_{L^2(B_1)}.}
$$

This is the required [Moser iteration](../../../../../../../moser-iteration.md) estimate, with a finite constant depending only on $\ell$ and $R$. The weak-test truncation argument in the preceding solution makes the conclusion valid for locally $H^1$ [weak solutions](../../../../../../../weak-solution.md) with $u\in L^2(B_1)$ and measurable uniformly elliptic coefficients. No differentiability of $A$ or unproved smooth approximation of solutions is required.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [3](../../../3.md)
4. [Paper 5](../../../../paper-5-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
