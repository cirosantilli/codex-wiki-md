<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A smooth [vector field](../../../../../vector-field.md) on a [smooth manifold](../../../../../smooth-manifold.md) $M$ is a smooth [section of a vector bundle](../../../../../section-of-a-vector-bundle.md) $X:M\to TM$ of the [tangent bundle](../../../../../tangent-bundle.md) projection $\pi$, so $\pi\circ X=\mathrm{id}_M$. In a coordinate chart it has the form $X=\sum_iX^i\partial_i$ with smooth component functions $X^i$.

Suppose a smooth [vector bundle isomorphism](../../../../../vector-bundle-isomorphism.md) $\Phi:M\times\mathbb R^n\to TM$ covering the identity is given. For the standard [basis](../../../../../basis.md) $e_1,\ldots,e_n$ of $\mathbb R^n$, put $X_i(p)=\Phi(p,e_i)$. These are smooth [vector fields](../../../../../vector-field.md), and the [linear isomorphism](../../../../../linear-isomorphism.md) on each fibre makes $X_1(p),\ldots,X_n(p)$ a [basis](../../../../../basis.md) of $T_pM$.

Conversely, given such a global [frame of a vector bundle](../../../../../frame-of-a-vector-bundle.md), define

$$
\boxed{\Phi(p,a_1,\ldots,a_n)=\sum_{i=1}^na_iX_i(p).}
$$

It is smooth, covers the identity and is a [linear isomorphism](../../../../../linear-isomorphism.md) on each fibre. Its inverse is smooth as well: in any coordinate chart, the component columns of the $X_i$ form an invertible smooth [matrix](../../../../../matrix.md) $C(p)$, and the fibre coordinates of the inverse are $C(p)^{-1}v$. [matrix](../../../../../matrix.md) inversion is smooth on the invertible [matrices](../../../../../matrix.md). Thus **the [tangent bundle](../../../../../tangent-bundle.md) is trivial exactly when a global frame exists**, the defining property of a [parallelizable manifold](../../../../../parallelizable-manifold.md).

For a [Lie group](../../../../../lie-group.md) $G$, write $L_h(g)=hg$. A [left-invariant vector field](../../../../../left-invariant-vector-field.md) is a field satisfying

$$
X(hg)=(dL_h)_gX(g).
$$

Such a field is determined by $v=X(e)\in T_eG$, since $X(g)=(dL_g)_ev$. Conversely, this formula defines a left-invariant field, by the [chain rule](../../../../../chain-rule.md) and $L_hL_g=L_{hg}$.

It also proves smoothness even if smoothness was not initially assumed. Choose a [smooth curve](../../../../../smooth-curve.md) $c(t)$ with $c(0)=e$, $c'(0)=v$. Then

$$
X(g)=\left.\frac{d}{dt}\right|_{t=0}g\,c(t).
$$

Multiplication is a [smooth map](../../../../../smooth-map-between-manifolds.md) on a [Lie group](../../../../../lie-group.md), so differentiating its coordinate functions in the second variable yields a [smooth function](../../../../../smooth-function.md) of $g$. This gives smooth components for $X$ in every local chart.

Choose a [basis](../../../../../basis.md) $v_1,\ldots,v_m$ of $T_eG$, where $m=\dim G$, and left translate it. Each $L_g$ is a [diffeomorphism](../../../../../diffeomorphism.md), with inverse $L_{g^{-1}}$, so $(dL_g)_e$ is a [linear isomorphism](../../../../../linear-isomorphism.md) and the translated fields are a [basis](../../../../../basis.md) at every $g$. The explicit [parallelization of a Lie group by left translations](../../../../../parallelization-of-a-lie-group-by-left-translations.md) is

$$
\boxed{G\times T_eG\longrightarrow TG,\qquad(g,v)\longmapsto(dL_g)_ev.}
$$

Its inverse sends $w\in T_gG$ to $(g,(dL_{g^{-1}})_gw)$. Identifying $T_eG$ with $\mathbb R^m$ gives the required product bundle. The differential facts used are linearity, the chain rule, $d(\mathrm{id})=\mathrm{id}$ and smooth dependence of the differential of a [smooth map](../../../../../smooth-map-between-manifolds.md) on its base point.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
