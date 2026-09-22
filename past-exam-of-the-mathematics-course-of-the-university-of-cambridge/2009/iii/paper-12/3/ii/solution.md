<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

First use weak compactness of bounded sets in the [Hilbert space](../../../../../../hilbert-space-split.md) $L^2(\Omega)$ to pass to a subsequence with $u_k\rightharpoonup u$ globally in $L^2$. The [weak lower semicontinuity of the Hilbert norm](../../../../../../weak-lower-semicontinuity-of-the-hilbert-norm.md) gives $\|u\|_{L^2(\Omega)}\leq K$. This global step also applies if $\Omega$ is unbounded.

Choose a nested exhaustion $U_j\Subset U_{j+1}\Subset\Omega$ by bounded smooth open sets. Part (i) bounds $u_k$ in $H^1(U_j)$ for every $j$. By the [Rellich-Kondrachov compactness theorem](../../../../../../rellich-kondrachov-theorem.md), $H^1(U_j)$ embeds compactly in $L^2(U_j)$. Weak compactness in $H^1(U_j)$ and a [diagonal subsequence argument](../../../../../../diagonal-subsequence-argument.md) therefore give, for the same subsequence,

$$
u_k\rightharpoonup u\text{ in }H^1(U_j),\qquad u_k\longrightarrow u\text{ in }L^2(U_j)\quad\text{for every }j.
$$

The local limit agrees with the global weak $L^2$ limit. Using smooth exhaustion sets avoids imposing any unprinted boundary regularity on a general $\Omega'$.

For a smooth [compactly supported](../../../../../../compact-support.md) [test function](../../../../../../test-function.md), the weak equation passes to the limit: the fixed bounded coefficients multiply fixed [test functions](../../../../../../test-function.md), and local [weak gradient](../../../../../../weak-gradient.md) convergence handles both the principal and drift terms. The zeroth-order term passes by local $L^2$ convergence. Thus $Lu=f$ weakly, $u\in H^1_{\mathrm{loc}}(\Omega)$, and the global bound already proved gives $u\in S_K$.

To improve convergence of the [gradients](../../../../../../gradient.md), put $w_k=u_k-u$. Crucially the forcing is the same for all $k$, so $Lw_k=0$. Given $\Omega'\Subset\Omega$, choose $j$ with $\overline{\Omega'}\subset U_j$. Apply part (i) on $U_j$ to the homogeneous equation for $w_k$:

$$
\|w_k\|_{H^1(\Omega')}\leq C\|w_k\|_{L^2(U_j)}\longrightarrow0.
$$

This establishes [strong local Sobolev compactness for a fixed elliptic equation](../../../../../../strong-local-sobolev-compactness-for-a-fixed-elliptic-equation.md) and proves

$$
\boxed{u\in S_K,\qquad u_{k'}\longrightarrow u\text{ in }W^{1,2}(\Omega')\text{ for every }\Omega'\Subset\Omega.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
