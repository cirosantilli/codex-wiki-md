<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Here “bumpy” means a [nowhere locally homogeneous metric](../../../../../nowhere-locally-homogeneous-metric.md), not the different convention concerning nondegenerate closed [geodesics](../../../../../geodesic.md). A smooth [Riemannian metric](../../../../../riemannian-metric.md) has this property if every [local isometry](../../../../../local-isometry.md) between connected open subsets is the identity on its domain; in particular, no two distinct open subsets are isometric. The [Sunada local isometry lemma](../../../../../sunada-local-isometry-lemma.md) states that, on a compact smooth [manifold](../../../../../topological-manifold.md) without boundary of dimension at least two, such [Riemannian metrics](../../../../../riemannian-metric.md) form a [residual set](../../../../../residual-set.md) and are dense in the $C^\infty$ topology. The dimension restriction matters: in dimension one, arclength coordinates always give nontrivial [local isometries](../../../../../local-isometry.md).

An element $j_x^kf$ of the [jet bundle of maps](../../../../../jet-bundle-of-maps.md) $J^k(M,N)$ records the source point $x$, target value $f(x)$ and all derivatives through order $k$. If $\dim M=m$ and $\dim N=n$, there are $\binom{m+r-1}{r}$ derivative [multi-indices](../../../../../multi-index-notation.md) of order $r$, and $n$ components for each one. Thus

$$
\boxed{\dim J^k(M,N)=m+n\binom{m+k}{k}.}
$$

For the projection $j_x^kf\mapsto(x,f(x))$ onto $M\times N$, the fiber has dimension $n(\binom{m+k}{k}-1)$. In source and target coordinates its Taylor coefficients identify it with

$$
\boxed{\bigoplus_{r=1}^k\operatorname{Sym}^r(T_x^*M)\otimes T_yN.}
$$

This is a coordinate-dependent identification for $k>1$, since a change of coordinates mixes different derivative orders. For $k=1$ the fiber is canonically $\operatorname{Hom}(T_xM,T_yN)$; for higher orders, truncation to the previous [jet bundle of maps](../../../../../jet-bundle-of-maps.md) is an [affine bundle](../../../../../affine-bundle.md) modeled on $\operatorname{Sym}^k(T_x^*M)\otimes T_yN$. For $k=0$ the fiber is a point.

**The density assertion in the printed question requires distinct closed domains.** Literally, for $i=k$, the identity is an [isometry](../../../../../isometry.md) for every [Riemannian metric](../../../../../riemannian-metric.md), so $\mathcal S_{ii}$ is the whole metric space and its complement is empty. Merely indexing the same closed ball twice has the same defect. The intended assertion is for distinct embedded closed balls $K_i=\overline U_i$ and $K_k=\overline U_k$, with an [isometry](../../../../../isometry.md) meaning an onto [diffeomorphism](../../../../../diffeomorphism.md) preserving the metric. The proof below establishes precisely this corrected assertion.

Distinct embedded closed balls are regular closed sets, so at least one of $\operatorname{int}K_i\setminus K_k$ and $\operatorname{int}K_k\setminus K_i$ contains a nonempty open set. Indeed, if both were empty, taking closures would give both inclusions and hence equality. Interchange the labels if necessary and choose a nonzero nonnegative [smooth bump function](../../../../../smooth-bump-function.md) $\eta$ supported in $\operatorname{int}K_i\setminus K_k$. For any given [Riemannian metric](../../../../../riemannian-metric.md) $g$, make the [localized volume perturbation](../../../../../localized-volume-perturbation.md)

$$
g_t=e^{2t\eta}g.
$$

The [Riemannian volume form](../../../../../riemannian-volume-form.md) satisfies $dV_{g_t}=e^{mt\eta}dV_g$. Therefore

$$
\operatorname{vol}_{g_t}(K_k)=\operatorname{vol}_g(K_k),\qquad
\frac d{dt}\operatorname{vol}_{g_t}(K_i)=m\int_{K_i}\eta e^{mt\eta}\,dV_g>0.
$$

If the original volumes agree, every sufficiently small $t>0$ makes them unequal. If they already disagree, continuity preserves that inequality for sufficiently small $t$. An onto [isometry](../../../../../isometry.md) must preserve volume, so each of these perturbed [Riemannian metrics](../../../../../riemannian-metric.md) belongs to $\mathcal C\mathcal S_{ik}$. Finally $g_t\to g$ in $C^\infty$: all derivatives of $e^{2t\eta}-1$ tend to zero uniformly on compact sets. This proves **density of $\mathcal C\mathcal S_{ik}$ for distinct closed balls**, in fact in every positive dimension. The [localized volume perturbation](../../../../../localized-volume-perturbation.md) settles this particular density claim directly. It also does not imply the stronger [Sunada local isometry lemma](../../../../../sunada-local-isometry-lemma.md) by itself, since a general [local isometry](../../../../../local-isometry.md) need not send one preselected basis ball onto another.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 20](../../paper-20-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
