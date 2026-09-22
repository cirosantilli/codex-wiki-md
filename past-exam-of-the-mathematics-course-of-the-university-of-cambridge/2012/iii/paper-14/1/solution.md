<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Fix the [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) convention

$$
R(X,Y)Z=\nabla_X\nabla_YZ-\nabla_Y\nabla_XZ-\nabla_{[X,Y]}Z.
$$

With this convention the round sphere has positive [sectional curvature](../../../../../sectional-curvature.md). Write $R(X,Y,Z,W)=g(R(X,Y)Z,W)$. We use skew-symmetry in the first and last pairs, pair interchange $R(X,Y,Z,W)=R(Z,W,X,Y)$, and the first Bianchi identity. These are the standard curvature symmetries of the [Levi-Civita connection](../../../../../levi-civita-connection.md).

For an [orthonormal basis](../../../../../orthonormal-basis.md) $e_1,\ldots,e_n$ of $T_pM$, the [Ricci curvature](../../../../../ricci-curvature.md) is the trace

$$
\operatorname{Ric}_p(X,Y)=\sum_i g(R(e_i,X)Y,e_i).
$$

For a plane spanned by linearly independent vectors $U,V$, its [sectional curvature](../../../../../sectional-curvature.md) is

$$
K(U,V)=\frac{g(R(U,V)V,U)}{g(U,U)g(V,V)-g(U,V)^2}.
$$

Both definitions are independent of the chosen basis. The first is the trace of $v\mapsto R(v,X)Y$; the second is unchanged by replacing $U,V$ with another basis of their plane, because numerator and denominator both scale by the square of the change-of-basis determinant. For $U=e_i,V=e_j$, $i\ne j$, the denominator is one. The terms with $i=j$ vanish, so

$$
\boxed{\operatorname{Scal}_p=\sum_j\operatorname{Ric}(e_j,e_j)=\sum_{i\ne j}K(e_i,e_j)=2\sum_{i<j}K(e_i,e_j)}.
$$

The ordered-pair sum counts every unoriented coordinate plane twice.

For $A_X(v)=R(X,v)X$, pair interchange immediately gives

$$
g(A_Xv,w)=R(X,v,X,w)=R(X,w,X,v)=g(v,A_Xw).
$$

Thus **$A_X$ is self-adjoint**, including when $X=0$. The usual [Jacobi curvature operator](../../../../../jacobi-curvature-operator.md) $v\mapsto R(v,X)X$ is its negative and is self-adjoint as well. Keeping these two signs distinct will also fix the [Jacobi field](../../../../../jacobi-field.md) equation below.

The [Bonnet-Myers theorem](../../../../../myers-s-theorem.md) states that a connected, complete $n$-dimensional [Riemannian manifold](../../../../../riemannian-manifold.md), $n\ge2$, with $\operatorname{Ric}\ge(n-1)\kappa g$ for a constant $\kappa>0$ has diameter at most $\pi/\sqrt\kappa$ and is compact. Completeness is required; a pointwise positive Ricci tensor without a uniform positive lower bound would not suffice for this stated conclusion.

A [left-invariant metric](../../../../../left-invariant-metric.md) on a [Lie group](../../../../../lie-group.md) is a [Riemannian metric](../../../../../riemannian-metric.md) for which every left translation $L_a$ is an [isometry](../../../../../isometry.md), equivalently $L_a^*g=g$. It is determined by an inner product on the [Lie algebra](../../../../../lie-algebra-split.md) $\mathfrak g=T_eG$. If the metric is also right-invariant, this inner product is invariant under the adjoint action; differentiating yields

$$
\langle[X,Y],Z\rangle+\langle Y,[X,Z]\rangle=0.
$$

Use left-invariant vector fields and the permitted formula $\nabla_XY=\tfrac12[X,Y]$. The Jacobi identity gives

$$
R(X,Y)Z=\frac14\bigl([X,[Y,Z]]-[Y,[X,Z]]\bigr)-\frac12[[X,Y],Z]
=-\frac14[[X,Y],Z].
$$

Adjoint skew-symmetry then implies

$$
g(R(X,Y)Y,X)=\frac14\|[X,Y]\|^2,\qquad
\operatorname{Ric}(X,X)=\frac14\sum_i\|[X,e_i]\|^2.
$$

This is the [Ricci curvature of a bi-invariant Riemannian metric](../../../../../ricci-curvature-of-a-bi-invariant-riemannian-metric.md). The last expression vanishes precisely when $X$ belongs to the center of the [Lie algebra](../../../../../lie-algebra-split.md). If that center is zero, it is positive for every nonzero $X$. Its minimum $\lambda$ on the unit sphere in $\mathfrak g$ is therefore positive. Left invariance transfers this bound to every point: $\operatorname{Ric}\ge\lambda g$.

Work in the identity component $G^0$, since $\pi_1(G,e)=\pi_1(G^0,e)$. It is compact and hence complete. Give its [universal cover](../../../../../universal-cover.md) $\widetilde G^0$ the lifted metric. The cover is complete: a [geodesic](../../../../../geodesic.md) projects to a [geodesic](../../../../../geodesic.md) in $G^0$, extends for all time there, and its extension lifts through any prescribed starting point. The [local isometry](../../../../../local-isometry.md) also preserves [Ricci curvature](../../../../../ricci-curvature.md), so the same uniform bound holds on the cover. Applying Bonnet-Myers with $\kappa=\lambda/(n-1)$ makes $\widetilde G^0$ compact. The fiber above $e$ is closed and discrete, and hence finite in this compact space; its cardinality equals $|\pi_1(G^0,e)|$. Consequently **$\pi_1(G,e)$ is finite**. This is the [finite fundamental group from a uniform positive Ricci bound](../../../../../finite-fundamental-group-from-a-uniform-positive-ricci-bound.md). If $\dim G=0$, the identity component is a point and the conclusion is immediate; a one-dimensional [Lie algebra](../../../../../lie-algebra-split.md) cannot have zero center.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
