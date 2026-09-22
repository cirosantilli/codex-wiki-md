<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Integration by parts gives the [minimal surface equation for a graph](../../../../../../minimal-surface-equation-for-a-graph.md) in nondivergence form:

$$
a^{ij}(Du)u_{ij}=0,\qquad
a^{ij}(p)=\delta_{ij}-\frac{p_ip_j}{1+|p|^2}.
$$

Its eigenvalues are between $(1+|p|^2)^{-1}$ and one. On each relatively compact subdomain, $Du$ is bounded, so it is a [uniformly elliptic operator](../../../../../../uniformly-elliptic-operator.md). Since $u\in C^2$, its coefficient functions are locally Lipschitz. The [interior Schauder estimate](../../../../../../interior-schauder-estimate.md) gives $C^{2,\beta}_{\rm loc}$ regularity for every $0<\beta<1$; differentiating and repeatedly applying regularity estimates gives $\boxed{u\in C^\infty(\Omega)}$.

Differentiate in direction $k$. Each $u_k$ satisfies $\mathcal Lu_k=0$, with

$$
\mathcal L=a^{ij}D_{ij}+b^\ell D_\ell,\qquad
b^\ell=\frac{\partial a^{ij}}{\partial p_\ell}(Du)u_{ij}.
$$

For $v=|Du|^2$ this yields

$$
\mathcal Lv=2\sum_k a^{ij}u_{ki}u_{kj}\geq0.
$$

If $u\in C^2(\overline\Omega)$, the principal coefficients are uniformly elliptic globally and the drift is bounded. The [weak maximum principle for elliptic operators](../../../../../../weak-maximum-principle-for-elliptic-operators.md) bounds $v$ by its boundary maximum. Boundary values are limits of interior values by [continuity](../../../../../../continuous-function.md), proving the [gradient maximum principle for a minimal graph](../../../../../../gradient-maximum-principle-for-a-minimal-graph.md):

$$
\boxed{\sup_\Omega|Du|=\sup_{\partial\Omega}|Du|.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
