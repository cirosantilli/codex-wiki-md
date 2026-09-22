<h1 id="3/3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take $\alpha=1+1/\ell>1$. Then $2\alpha<p^*$ in every $\ell\ge2$, including $p^*=\infty$ for $\ell=2$. The supplied [Sobolev embedding theorem](../../../../../../../sobolev-embedding-theorem.md), by the fixed scaling from $B_{1/2}$ to $B_1$, gives $\|w\|_{L^{2\alpha}(B_1)}\le C_\ell\|w\|_{H^1(B_1)}$.

Choose $0\le\zeta\le1$, equal to one on $B_{r_1}$, supported in $B_{r_2}$, with $|\nabla\zeta|\le C/(r_2-r_1)$. Extend $w=\zeta u$ by zero to $B_1$. The [Caccioppoli inequality](../../../../../../../caccioppoli-inequality.md) before discarding the cutoff weight gives

$$
\|\nabla w\|_2\le\|\zeta\nabla u\|_2+\|u\nabla\zeta\|_2\le(2R+1)\|u\nabla\zeta\|_2.
$$

Also $\|w\|_2\le\|u\|_{L^2(B_{r_2})}$. Since $R>1$ and $r_2-r_1\le1$, both terms are controlled by $C R(r_2-r_1)^{-1}\|u\|_2$. Applying the [Sobolev embedding theorem](../../../../../../../sobolev-embedding-theorem.md) to $w$ gives

$$
\boxed{\|u\|_{L^{2\alpha}(B_{r_1})}\le\frac{C_\ell R}{r_2-r_1}\|u\|_{L^2(B_{r_2})},\qquad\alpha=1+1/\ell.}
$$

Using a fixed ambient ball prevents the Sobolev constant from acquiring an unintended dependence on either radius.

## ↑ Ancestors (12)

1. [B](../b.md)
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
