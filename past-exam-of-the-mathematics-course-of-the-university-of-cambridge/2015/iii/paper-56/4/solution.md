<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [degree of a map between oriented manifolds](../../../../../degree-of-a-map-between-oriented-manifolds.md) measures how many times the domain covers the target, with signs recording the local [local orientation of a manifold](../../../../../local-orientation-of-a-manifold.md). Let $M,N$ be connected, oriented [closed manifolds](../../../../../closed-manifold.md) of the same dimension $n>0$. A continuous map $f:M\to N$ acts on top-dimensional [homology](../../../../../homology-split.md) by

$$
\boxed{f_*[M]=\deg(f)[N],\qquad\deg(f)\in\mathbb Z,}
$$

where $[M],[N]$ are their [fundamental classes](../../../../../fundamental-class.md). Connectedness and the choices of [local orientation of a manifold](../../../../../local-orientation-of-a-manifold.md) identify $H_n(N;\mathbb Z)$ with $\mathbb Z$. Reversing the orientation of either manifold changes the sign; reversing both does not.

For a smooth map, [Sard theorem](../../../../../sard-s-theorem.md) supplies a [regular value](../../../../../regular-value.md) $y$. Its inverse image is discrete and, by compactness, finite. At each $x\in f^{-1}(y)$ the differential is an isomorphism; let its sign be $+1$ or $-1$ according to whether it preserves or reverses the chosen local orientations. The [degree as a sum of local degrees](../../../../../degree-as-a-sum-of-local-degrees.md) is

$$
\boxed{\deg(f)=\sum_{x\in f^{-1}(y)}\operatorname{sgn}\det(df_x).}
$$

The sign is computed in oriented [manifold charts](../../../../../manifold-chart.md). The value is independent of the chosen [regular value](../../../../../regular-value.md), even when inverse images appear or disappear: the signed count is the coefficient of $[N]$ in $f_*[M]$.

There is a useful local-density expression for the same [topological degree](../../../../../topological-degree.md). If $\omega$ is a [volume form](../../../../../volume-form.md) with $\int_N\omega=1$, then

$$
\boxed{\deg(f)=\int_M f^*\omega.}
$$

This [degree by integration of a pullback volume form](../../../../../degree-by-integration-of-a-pullback-volume-form.md) follows first by choosing a smooth top-form supported in a small neighborhood of a [regular value](../../../../../regular-value.md), where the inverse branches contribute their orientation signs. Any other normalized top-form differs from it by an exact form: integration identifies $H^n_{\mathrm{dR}}(N)$ with $\mathbb R$. The integral of its pullback difference vanishes by [Stokes theorem](../../../../../stokes-theorem.md). In particular, for any top-form $\eta$, $\int_M f^*\eta=\deg(f)\int_N\eta$.

A [homotopy](../../../../../homotopy.md) $H:M\times[0,1]\to N$ preserves this integral, since $d\omega=0$ and [Stokes theorem](../../../../../stokes-theorem.md) gives

$$
\int_M f_1^*\omega-\int_M f_0^*\omega=\int_{M\times[0,1]}d(H^*\omega)=0.
$$

Thus [topological degree](../../../../../topological-degree.md) is a [homotopy](../../../../../homotopy.md) invariant. It is multiplicative under composition, because the induced maps on [homology](../../../../../homology-split.md) compose: $\deg(g\circ f)=\deg(g)\deg(f)$. The identity has degree one, a constant map has degree zero for $n>0$, and an orientation-reversing [diffeomorphism](../../../../../diffeomorphism.md) has degree minus one. An orientation-preserving finite [covering map](../../../../../covering-space.md) has degree equal to its number of sheets. Nonzero [topological degree](../../../../../topological-degree.md) forces surjectivity, since an omitted point would be a [regular value](../../../../../regular-value.md) with an empty inverse image.

For the [circle](../../../../../circle.md), $e^{i\theta}\mapsto e^{ik\theta}$ has degree $k$, positive or negative. This is its [winding number](../../../../../winding-number.md), computable as $(2\pi i)^{-1}\int f^{-1}df$. The antipodal map of $S^n$ has degree $(-1)^{n+1}$: its extension $-I$ on the ambient $(n+1)$-dimensional vector space has that determinant sign and respects the outward-normal convention. A holomorphic map $z\mapsto z^k$, $k\geq1$, on the [Riemann sphere](../../../../../riemann-sphere.md) has degree $k$, whereas its complex conjugate has degree $-k$. These examples show how orientation, rather than simply the number of inverse images, determines the integer.

For maps $S^n\to S^n$, [topological degree](../../../../../topological-degree.md) gives the complete [homotopy](../../../../../homotopy.md) classification $\pi_n(S^n)\cong\mathbb Z$. The [degree does not classify general manifold maps](../../../../../degree-does-not-classify-general-manifold-maps.md): the identity of the [torus](../../../../../torus.md) and the map induced by the integer matrix $\begin{pmatrix}1&1\\0&1\end{pmatrix}$ both have degree one, but have different induced maps on $H_1(T^2;\mathbb Z)$ and so are not homotopic. A nonzero-degree map $S^n\to S^n$ cannot extend continuously to $B^{n+1}$, because such an extension would make the boundary map null-homotopic. In the smooth setting, [Stokes theorem](../../../../../stokes-theorem.md) gives the same obstruction by applying it to the pulled-back normalized [volume form](../../../../../volume-form.md).

The hypotheses can be adjusted, but must be stated. For connected oriented noncompact manifolds, a [proper map](../../../../../proper-map.md) has a degree defined using compactly supported top-forms, and it is invariant under proper [homotopies](../../../../../homotopy.md). For [manifolds with boundary](../../../../../manifold-with-boundary.md) one uses relative [fundamental classes](../../../../../fundamental-class.md) and maps of pairs, or fixes appropriate boundary conditions. Without an integral orientation one can still count inverse images modulo two, obtaining a mod-two degree. The integer integral formula used below assumes the oriented setting.

In [classical field theory](../../../../../classical-field-theory.md), these ideas turn continuous fields into quantized [topological charges](../../../../../topological-charge.md). Suppose a field on $\mathbb R^d$ approaches one fixed target value at spatial infinity. The [one-point compactification](../../../../../alexandroff-extension.md) makes it a map $\phi:S^d\to\mathcal V$. When the target $\mathcal V$ is an oriented closed $d$-manifold, its [topological degree](../../../../../topological-degree.md) labels [topological sectors](../../../../../topological-sector.md). More generally the sectors are described by [homotopy groups](../../../../../homotopy-group.md); an integer degree is available only when the domain and target have the appropriate dimensions and orientations. Smooth time evolution preserving the boundary condition is a [homotopy](../../../../../homotopy.md), so it cannot change the integer. A change requires a singular field, escape from the allowed target, or a change at the boundary.

A normalized closed target $d$-form gives the [pullback-volume representation of a topological current](../../../../../pullback-volume-representation-of-a-topological-current.md). On spacetime, put $\alpha=\phi^*\omega$. Since $d\alpha=\phi^*(d\omega)=0$, its dual current is identically conserved, and

$$
Q=\int_{\text{space}}\alpha=\deg(\phi)
$$

is independent of time when there is no flux at infinity. This conservation law follows from geometry without using the field equations; it need not arise from a continuous symmetry through [Noether theorem](../../../../../noether-theorem.md).

A concrete example is the [O3 nonlinear sigma model](../../../../../o3-nonlinear-sigma-model.md) in two spatial dimensions. Its unit-vector field $\mathbf n$ approaches a constant at infinity, defining $S^2\to S^2$. The normalized area form of the target gives the [degree charge of an O3 sigma-model lump](../../../../../degree-charge-of-an-o3-sigma-model-lump.md):

$$
\boxed{Q=\frac1{4\pi}\int_{\mathbb R^2}\mathbf n\cdot(\partial_1\mathbf n\times\partial_2\mathbf n)\,dx^1dx^2\in\mathbb Z.}
$$

For the energy normalization $E=\tfrac12\int(|\partial_1\mathbf n|^2+|\partial_2\mathbf n|^2)$, the identities $\mathbf n\cdot\partial_i\mathbf n=0$ give

$$
E=\frac12\int|\partial_1\mathbf n\pm\mathbf n\times\partial_2\mathbf n|^2\,d^2x\ \pm4\pi Q,\qquad\boxed{E\geq4\pi|Q|.}
$$

This is the [Bogomolny degree bound for the O3 sigma model](../../../../../bogomolny-degree-bound-for-the-o3-sigma-model.md). Choosing the sign appropriate to $Q$ makes the square nonnegative; vanishing of the square gives first-order [Bogomolny equations](../../../../../bogomolny-equations.md) and a [sigma-model lump](../../../../../sigma-model-lump.md) saturating the bound. With the oriented [stereographic projection](../../../../../stereographic-projection.md)

$$
\mathbf n=\frac{(2\operatorname{Re}w,2\operatorname{Im}w,1-|w|^2)}{1+|w|^2},\qquad z=x^1+ix^2,
$$

the maps $w=z^k$ have $Q=k$ and $E=4\pi k$. Their conjugates have $Q=-k$ with the same energy. Holomorphic rational maps have positive degree equal to their degree as rational maps; taking a reciprocal does not reverse the orientation. Antiholomorphic dependence reverses it.

The [Skyrme model](../../../../../skyrme-model.md) supplies a three-dimensional example. A field $U:\mathbb R^3\to\mathrm{SU}(2)$ with $U\to I$ at infinity is a map $S^3\to\mathrm{SU}(2)\cong S^3$. Take $T_i=-i\tau_i$ and $U^{-1}dU=\theta^iT_i$, with $\theta^1\wedge\theta^2\wedge\theta^3$ positive. Since $\operatorname{tr}(T_iT_jT_k)=-2\epsilon_{ijk}$, the normalized target [volume form](../../../../../volume-form.md) is

$$
\omega_3=-\frac1{24\pi^2}\operatorname{tr}(U^{-1}dU)^3=\frac1{2\pi^2}\theta^1\wedge\theta^2\wedge\theta^3.
$$

The integral is one on the unit [three-sphere](../../../../../three-sphere.md). Consequently the [Skyrme baryon number as a mapping degree](../../../../../skyrme-baryon-number-as-a-mapping-degree.md) is

$$
\boxed{B=-\frac1{24\pi^2}\int_{\mathbb R^3}\operatorname{tr}(U^{-1}dU)^3=\deg(U).}
$$

This is the [topological baryon number in the Skyrme model](../../../../../topological-baryon-number-in-the-skyrme-model.md); the sign has been fixed by the stated orientation and anti-Hermitian generator convention.

A [topological charge](../../../../../topological-charge.md) alone does not guarantee a stable finite-size solution. The [degree and energetic stability of a field configuration](../../../../../degree-and-energetic-stability-of-a-field-configuration.md) concern different properties. For a three-dimensional configuration of size $R$, the two-derivative energy scales as $R$, so it can decrease by shrinking while the [topological degree](../../../../../topological-degree.md) remains fixed for every $R>0$. The limit can be singular. The [Skyrme term](../../../../../skyrme-term.md), with four derivatives, scales as $R^{-1}$ and can balance the shrinking tendency. This is the role of [Derrick theorem](../../../../../derrick-s-theorem.md) in distinguishing topological obstruction from energetic stability.

For defects, the relevant boundary map can instead be the sphere surrounding a core. A [vacuum manifold](../../../../../vacuum-manifold.md) equal to $S^1$ gives the integer [winding number](../../../../../winding-number.md) of a [vortex](../../../../../phase-vortex.md); a vacuum manifold $S^2$ gives the degree of a surrounding $S^2$ for a [magnetic monopole](../../../../../magnetic-monopole.md). This [vacuum-boundary degree as a defect charge](../../../../../vacuum-boundary-degree-as-a-defect-charge.md) obstructs extending the normalized vacuum field through the enclosed ball. A nonzero integer therefore forces the field to leave the [vacuum manifold](../../../../../vacuum-manifold.md) somewhere in the core. This construction does not require the field to take one constant value in every direction at infinity.

Degree also appears in four-dimensional gauge theory through a boundary transition function. For an anti-Hermitian [SU(2)](../../../../../su-2-group.md) gauge connection on $\mathbb R^4$, write $F=dA+A\wedge A$ and assume finite-action boundary behavior $A\to g^{-1}dg$ on the large bounding [three-sphere](../../../../../three-sphere.md). In the second-Chern convention

$$
k=\frac1{8\pi^2}\int_{\mathbb R^4}\operatorname{tr}(F\wedge F),
$$

the identity $d\operatorname{tr}(A\wedge dA+\tfrac23A^3)=\operatorname{tr}(F\wedge F)$ and the [Maurer-Cartan equation](../../../../../maurer-cartan-equation.md) give

$$
\boxed{k=-\frac1{24\pi^2}\int_{S^3}\operatorname{tr}(g^{-1}dg)^3=\deg(g).}
$$

This [boundary winding representation of Yang-Mills topological charge](../../../../../boundary-winding-representation-of-yang-mills-topological-charge.md) relates the [Second Chern number](../../../../../second-chern-number.md) to the degree of $g:S^3\to\mathrm{SU}(2)$. The [Chern-Simons 3-form](../../../../../chern-simons-3-form.md) turns the bulk integral into the boundary winding integral. Conventions which define the instanton number with the opposite trace sign reverse $k$; the integer quantization is unchanged. A [Yang-Mills theta term](../../../../../yang-mills-theta-term.md) weights a sector by $e^{i\vartheta k}$, giving periodicity $\vartheta\mapsto\vartheta+2\pi$. Thus the same [topological degree](../../../../../topological-degree.md) that counts oriented inverse images also labels field sectors and expresses their quantized charges as integrals of local densities.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
