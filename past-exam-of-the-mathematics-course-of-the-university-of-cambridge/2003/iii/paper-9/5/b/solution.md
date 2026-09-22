<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

We prove sufficiency by a [non-tangential maximal function](../../../../../../non-tangential-maximal-function.md) and the [layer cake representation](../../../../../../layer-cake-representation.md). Write $K=C(\mu)$. First $\mu(\mathbb D)\le C K$: three [hyperbolic geodesic caps](../../../../../../hyperbolic-geodesic-cap.md) corresponding to arcs of normalized length $2/3$, with equally spaced centers, cover the [unit disc](../../../../../../unit-disc.md). This handles interior points and large arcs, not only a thin boundary strip.

Fix aperture two and set $Nf(\xi)=\sup_{z\in\Gamma_2(\xi)}|f(z)|$. The crucial [H1 non-tangential maximal inequality on the disk](../../../../../../h1-non-tangential-maximal-inequality-on-the-disk.md) is

$$
\int_{\partial\mathbb D}Nf\,dm\le C\|f\|_1.
$$

Here is its endpoint proof. For $0<R<1$ let $f_R(z)=f(Rz)$, which is [holomorphic](../../../../../../complex-differentiability-at-a-point.md) across the closed [unit disc](../../../../../../unit-disc.md). Since [modulus powers of holomorphic functions are subharmonic](../../../../../../modulus-powers-of-holomorphic-functions-are-subharmonic.md), Poisson comparison gives

$$
|f_R(z)|^{1/2}\le P[g_R](z),\qquad g_R(\xi)=|f(R\xi)|^{1/2}.
$$

The estimate that a [Poisson maximal function is dominated by the Hardy-Littlewood maximal function](../../../../../../poisson-maximal-function-is-dominated-by-the-hardy-littlewood-maximal-function.md) yields $(Nf_R)^{1/2}\le C M g_R$. The strong $L^2$ [Hardy-Littlewood maximal inequality](../../../../../../hardy-littlewood-maximal-inequality.md) now gives

$$
\int Nf_R\,dm\le C\int(Mg_R)^2\,dm
\le C\int|f(R\xi)|\,dm\le C\|f\|_1.
$$

For each interior point $f_R(z)\to f(z)$, hence $Nf\le\liminf_{R\uparrow1}Nf_R$. The [Fatou lemma](../../../../../../fatou-s-lemma.md) proves the maximal inequality. This uses a genuine $L^2$ maximal bound; the [Hardy-Littlewood maximal function](../../../../../../hardy-littlewood-maximal-function.md) is not strongly bounded on $L^1$.

For $t>0$, the set $O_t=\{\xi:Nf(\xi)>t\}$ is open, since each interior point witnessing this strict inequality has an open boundary shadow. Write its disjoint arc components as $I_j$. If $|f(z)|>t$ and $\delta=1-|z|$, the arc centered at $z/|z|$ with angular half-width $\delta$ lies in $O_t$, because $|z-\xi|<2\delta$ there. Thus it lies in one component $I_j$, and $z$ has angular projection in $I_j$ with $\delta\le\pi m(I_j)$. The [geodesic-cap and Carleson-box comparison](../../../../../../geodesic-cap-and-carleson-box-comparison.md) puts all such points in $Q(\kappa I_j)$ for a fixed enlargement factor $\kappa$ whenever $I_j$ is small. For large $I_j$, use $\mu(\mathbb D)\le C K\le C'K m(I_j)$. If $z=0$ or $O_t$ is the entire circle, that same total-mass estimate applies. Summing, without needing the enlarged caps to be disjoint, gives

$$
\mu\{z:|f(z)|>t\}\le C K\sum_jm(I_j)=C K m(O_t).
$$

The [layer cake representation](../../../../../../layer-cake-representation.md) and the proved [H1 non-tangential maximal inequality on the disk](../../../../../../h1-non-tangential-maximal-inequality-on-the-disk.md) finish the argument:

$$
\int_{\mathbb D}|f|\,d\mu
=\int_0^\infty\mu\{|f|>t\}\,dt
\le C K\int_0^\infty m\{Nf>t\}\,dt
\le C K\|f\|_1.
$$

Thus **the two conditions are equivalent**, with their least admissible constants comparable: $C(\mu)\le C_1N(\mu)$ and $N(\mu)\le C_2C(\mu)$. This is the [Carleson embedding theorem on the disk](../../../../../../carleson-embedding-theorem-on-the-disk.md), proved at the analytic $H^1$ endpoint.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
