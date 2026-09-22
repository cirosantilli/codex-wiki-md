<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The starting point is the [Grassmannian](../../../../../grassmannian.md) of complex two-planes $W\subset\mathbb T\cong\mathbb C^4$. Choose a basis $u,v$ and form the simple [bivector](../../../../../bivector.md) $P=u\wedge v\in\Lambda^2\mathbb T$. A change of basis multiplies $P$ by a nonzero determinant, so its projective class is independent of that choice. The [Plücker embedding](../../../../../plucker-embedding.md) is therefore

$$
\operatorname{Gr}(2,4)\longrightarrow\mathbb P(\Lambda^2\mathbb C^4)\cong\mathbb{CP}^5,\qquad W\longmapsto[u\wedge v].
$$

It is injective because $W=\{z:z\wedge P=0\}$. In a basis of $\mathbb T$, its six homogeneous coordinates $p_{ij}=u_iv_j-u_jv_i$ satisfy

$$
\boxed{p_{12}p_{34}-p_{13}p_{24}+p_{14}p_{23}=0.}
$$

This is the condition $P\wedge P=0$. Conversely, a nonzero antisymmetric $4\times4$ matrix satisfying it has [Pfaffian](../../../../../pfaffian.md) zero, hence rank at most two; its nonzero rank is even, so it has rank two and is a simple [bivector](../../../../../bivector.md). Therefore the equation characterizes the image, the [Klein quadric](../../../../../klein-quadric.md) $Q\subset\mathbb{CP}^5$. Its gradient cannot vanish at a projective point, since its six partial derivatives are the six coordinates up to permutation and sign. Thus $Q$ is smooth and has complex dimension four, agreeing with $\operatorname{Gr}(2,4)$.

The [Klein quadric](../../../../../klein-quadric.md) is the [complexified compactified Minkowski space](../../../../../complexified-compactified-minkowski-space.md) of the [twistor correspondence](../../../../../twistor-correspondence.md). A volume form on $\mathbb T$ turns $P\wedge P'$ into a scalar symmetric [bilinear form](../../../../../bilinear-form.md) $B(P,P')$. It is zero exactly when the two underlying two-planes have nontrivial intersection: the four spanning vectors are then linearly dependent. In [projective twistor space](../../../../../projective-twistor-space.md) this says that the two [twistor lines](../../../../../twistor-line.md) meet. In the affine graph chart supplied by the [twistor incidence relation](../../../../../twistor-incidence-relation.md), it is $\det(x-y)=0$, so it is precisely null separation.

This also determines a [conformal geometry](../../../../../conformal-geometry.md) on $Q$. At $[P]$, the tangent space is $P^\perp/\langle P\rangle$ for $B$. The restriction of $B$ descends to a nondegenerate quadratic form on this four-dimensional quotient. Rescaling the representative $P$ changes the identification by a scalar, so its invariant content is a conformal class. In a graph chart its null tangent vectors are the rank-one matrices in $\operatorname{Hom}(W,\mathbb T/W)$, equivalently $dx^{AA'}=a^Ab^{A'}$.

The compact complex geometry does not yet specify a real spacetime. The Lorentzian slice comes from the [twistor Hermitian form](../../../../../twistor-hermitian-form.md) $h$ of signature $(2,2)$: real points are maximal totally isotropic two-planes. In the incidence chart, isotropy of $W_x=\{(ix\pi,\pi)\}$ is equivalent to $x=x^\dagger$, the usual real Minkowski condition. Its [twistor lines](../../../../../twistor-line.md) lie wholly in [projective null twistor space](../../../../../projective-null-twistor-space.md). Diagonalizing $h$ as positive and negative two-dimensional blocks also gives a useful global description: an isotropic two-plane projects isomorphically to the positive block, so it is a graph $(z,Uz)$, and isotropy is $U^\dagger U=1$. The real compact space is therefore $U(2)$, equivalently $(S^1\times S^3)/\mathbb Z_2$.

The same result is especially transparent in coordinates of the [Plücker embedding](../../../../../plucker-embedding.md) after a complex linear change of coordinates on $\Lambda^2\mathbb T$. The real Lorentzian cone has equation

$$
T^2+V^2-W^2-X^2-Y^2-Z^2=0.
$$

Its nonzero real generators represent points. Normalize the lengths of its positive and negative parts to one; real projectivization identifies their simultaneous antipodes. Consequently

$$
\boxed{\overline M_L\cong(S^1\times S^3)/\{(u,v)\sim(-u,-v)\}.}
$$

This is the [Projective Minkowski compactification](../../../../../projective-minkowski-compactification.md). Its universal cover is $\mathbb R\times S^3$, with deck generator $(s,v)\mapsto(s+\pi,-v)$, so its [fundamental group](../../../../../fundamental-group.md) is $\mathbb Z$. The projective version includes periodic identifications; an unwrapped Einstein-cylinder or [Penrose diagram](../../../../../penrose-diagram.md) description uses the appropriate cover and affine domain instead.

For example, use homogeneous cone coordinates $[U,V,t,\boldsymbol x]$ with quadratic equation $2UV+t^2-|\boldsymbol x|^2=0$. The affine patch $U\ne0$ sets $U=1$ and then $V=-(t^2-|\boldsymbol x|^2)/2$. The complement $U=0$ is the null cone $t^2-|\boldsymbol x|^2=0$ at infinity. It is much larger than a single point: different null directions retain different limits there.

For the Euclidean slice, choose an antilinear [quaternionic structure on a complex vector space](../../../../../quaternionic-structure-on-a-complex-vector-space.md) $J$ on [twistor space](../../../../../twistor-space.md), for example

$$
J(z_1,z_2,z_3,z_4)=(-\overline z_2,\overline z_1,-\overline z_4,\overline z_3),\qquad J^2=-1.
$$

The [Euclidean reality structure on twistor space](../../../../../euclidean-reality-structure-on-twistor-space.md) selects $J$-invariant complex two-planes. Such a plane is a quaternionic line in $\mathbb H^2$, giving

$$
\boxed{\overline M_E\cong\mathbb{HP}^1\cong S^4.}
$$

There are no fixed projective twistors for $J$: if $JZ=cZ$, applying $J$ again would give $-Z=|c|^2Z$. Every projective twistor instead lies on the unique invariant line $\mathbb P\operatorname{span}(Z,JZ)$. Thus the Euclidean correspondence becomes a fibration $\mathbb{CP}^3\to S^4$ with fiber $\mathbb{CP}^1$, in contrast to the Lorentzian correspondence where only null twistors represent real null geodesics. Distinct Euclidean real points have disjoint [twistor lines](../../../../../twistor-line.md), since the line through any $Z$ and $JZ$ is unique. This reflects the absence of nonzero real null vectors for a positive-definite metric.

On the [Klein quadric](../../../../../klein-quadric.md) the Euclidean real cone has signature $(1,5)$; normalize its timelike coordinate to one and obtain the unit sphere $S^4$. Its affine Euclidean chart omits one point. Inverse [stereographic projection](../../../../../stereographic-projection.md) explicitly gives the round conformal metric

$$
\boxed{ds_{S^4}^2=\frac{4\sum_{j=1}^4dy_j^2}{(1+|y|^2)^2},}
$$

which extends smoothly across that point. This proves the one-point [conformal compactification of Euclidean space](../../../../../conformal-compactification-of-euclidean-space.md). The distinction between the Lorentzian Hermitian and Euclidean quaternionic reality structures is also described in [Adamo's lectures on twistor theory](https://arxiv.org/pdf/1712.02196); the global statements here follow from the explicit models just derived.

Finally, [Wick rotation](../../../../../wick-rotation.md) $t\mapsto it$ compares affine real slices through their complexification. Locally it changes $dt^2-|d\boldsymbol x|^2$ to $-d\tau^2-|d\boldsymbol x|^2$, the negative of the Euclidean metric; the overall sign does not change its null cone in the complexified setting. It does **not** identify the two real [conformal compactifications](../../../../../conformal-compactification.md) globally. The Lorentzian projective space has [fundamental group](../../../../../fundamental-group.md) $\mathbb Z$, while $S^4$ is simply connected. Its causal universal cover $\mathbb R\times S^3$ is noncompact, so passing to that cover does not repair the mismatch with the compact Euclidean sphere.

There is also a direct algebraic obstruction. In the homogeneous coordinates above the affine Wick substitution extends only as the rational map

$$
[U,V,t,\boldsymbol x]\longmapsto[U^2,UV+t^2,iUt,U\boldsymbol x].
$$

Substitution verifies that the image satisfies the same complex quadric equation. For $U=0$ and $t\ne0$ it collapses the point to $[0,1,0,\boldsymbol0]$, while at some infinity points every output coordinate vanishes. In particular it is indeterminate at $[0,1,0,\boldsymbol0]$. This is a genuine failure of holomorphic extension: the affine paths $(t,\boldsymbol x)=(0,(s,0,0))$ and $(s,(is,0,0))$, as $s\to\infty$, both tend to that input point. Their Wick images tend respectively to $[0,1,0,\boldsymbol0]$ and $[0,0,1,(1,0,0)]$, which are distinct points of the complex quadric.

Thus the **answer to the global compatibility question is no**: ordinary affine Wick rotation is a local analytic continuation, not a globally regular invertible map of the conformally compactified real spacetimes. The [global obstruction to Wick rotation of conformal compactifications](../../../../../global-obstruction-to-wick-rotation-of-conformal-compactifications.md) does not prevent both real slices from being studied inside the same smooth complex [Klein quadric](../../../../../klein-quadric.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 59](../../paper-59-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
