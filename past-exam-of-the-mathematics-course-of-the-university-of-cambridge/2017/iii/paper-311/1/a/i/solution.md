<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use $G=c=1$, the [Einstein field equations](../../../../../../../einstein-field-equations.md) with zero [cosmological constant](../../../../../../../cosmological-constant.md), and [metric signature](../../../../../../../metric-signature.md) $(-,+,+,+)$. Write $m=m_a\,dx^a$ for the [differential one-form](../../../../../../../one-form.md) dual to the axial [Killing vector field](../../../../../../../killing-vector-field.md). To fix the sign of the volume formula, use the component [Hodge star operator](../../../../../../../hodge-star-operator.md) convention $(\star j)_{abc}=\epsilon_{abcd}j^d$ and $(\star F)_{ab}=\tfrac12\epsilon_{abcd}F^{cd}$. The [Killing equation](../../../../../../../killing-equation.md) gives $(dm)_{ab}=2\nabla_am_b$, and its contracted curvature identity gives

$$
\nabla^b(dm)_{ab}=2R_{ab}m^b,\qquad
d\star dm=-2\star(R_{ab}m^b\,dx^a).
$$

To see the curvature step, tracing the [Killing equation](../../../../../../../killing-equation.md) gives $\nabla_bm^b=0$. The [second covariant derivative of a Killing vector](../../../../../../../second-covariant-derivative-of-a-killing-vector.md) then gives $\nabla^b\nabla_bm_a=-R_{ab}m^b$, while commuting the [covariant derivatives](../../../../../../../covariant-derivative.md) gives $\nabla^b\nabla_am_b=R_{ab}m^b$. Subtracting these two terms is precisely $\nabla^b(dm)_{ab}$ above. The component [Hodge star operator](../../../../../../../hodge-star-operator.md) converts this divergence to $d\star dm$ with the displayed minus sign.

In a [vacuum spacetime](../../../../../../../vacuum-spacetime.md) region $R_{ab}=0$, so $d\star dm=0$. If $S_1$ and $S_2$ are enclosing [spacelike submanifolds](../../../../../../../spacelike-submanifold.md) in the same [homology class](../../../../../../../homology-class.md) bounding a vacuum three-dimensional region $W$, [Stokes theorem](../../../../../../../stokes-theorem.md) yields

$$
\int_{S_2}\star dm-\int_{S_1}\star dm=\int_Wd\star dm=0.
$$

Thus **the [Komar angular momentum](../../../../../../../komar-angular-momentum.md) is independent of the enclosing vacuum spacelike two-manifold**, provided the surfaces have the same [orientation](../../../../../../../orientation-of-a-simplex.md) and enclose the same sources and inner boundaries. The vacuum region need not be stationary: an axial [Killing vector field](../../../../../../../killing-vector-field.md) suffices.

For a regular filling [hypersurface](../../../../../../../hypersurface.md) $\Sigma$ with $\partial\Sigma=S$, the [Einstein field equations](../../../../../../../einstein-field-equations.md) give

$$
d\star dm=-16\pi\star\left[J'-\frac12Tm\right],\qquad
J'_a=T_{ab}m^b.
$$

The pullback of $\star m$ to $\Sigma$ vanishes because $m^a$ is tangent to $\Sigma$: the dual three-form measures the normal component, which is zero. Therefore

$$
\boxed{J=-\int_\Sigma\star J'.}
$$

This is the [stress-energy current from a Killing vector](../../../../../../../stress-energy-current-from-a-killing-vector.md) integrated over the slice, with the signs fixed by the stated [Hodge star operator](../../../../../../../hodge-star-operator.md) convention.

There is a necessary boundary qualification omitted from the printed formulation. If the slice has inner boundaries $S_i$, orient them so $\partial\Sigma=S-\bigcup_iS_i$. The actual [Komar angular momentum with inner boundaries](../../../../../../../komar-angular-momentum-with-inner-boundaries.md) identity is

$$
J-\sum_iJ_i=-\int_\Sigma\star J',\qquad
J_i=\frac1{16\pi}\int_{S_i}\star dm.
$$

For a vacuum [Kerr black hole](../../../../../../../kerr-black-hole.md), $T_{ab}=0$ on the exterior slice but $J\ne0$; its horizon supplies precisely the inner boundary contribution. Thus the matter-only formula is false for arbitrary exterior slices. It is valid when a nonsingular filling with no inner boundaries exists, or when all omitted inner charges vanish. The [Komar angular momentum](../../../../../../../komar-angular-momentum.md) independence likewise concerns homologous surfaces in the same vacuum region, not an unrestricted comparison of differently enclosed objects.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 311](../../../../paper-311-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
