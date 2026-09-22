<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [principal bundle](../../../../../principal-bundle.md) $\pi:P\to B$ with structure group $G$ has a smooth free right $G$-action, each fibre is a single orbit, and it is locally equivariantly isomorphic to $U\times G\to U$. A representation $\rho:G\to GL(V)$ defines the [associated vector bundle](../../../../../associated-vector-bundle.md)

$$
E=P\times_\rho V=(P\times V)/\sim,\qquad
(p,v)\sim(pg,\rho(g)^{-1}v).
$$

Local sections of $P$ identify $E$ with $U\times V$, and changes of section act by $\rho$ on the fibre coordinates.

A [principal bundle](../../../../../principal-bundle.md) is **trivial if and only if it has a global smooth section**. Given $s:B\to P$, the map $(b,g)\mapsto s(b)g$ is an equivariant isomorphism $B\times G\to P$: freeness and transitivity give its unique inverse on each fibre, and local trivializations make that inverse smooth. Conversely a product bundle has section $b\mapsto(b,e)$. This proves [principal bundle trivialization by a global section](../../../../../principal-bundle-trivialization-by-a-global-section.md). A contractible paracompact base is a sufficient condition for triviality of such a bundle; local sections alone are insufficient on a general base.

A manifold is [parallelizable](../../../../../parallelizable-manifold.md) when its [tangent bundle](../../../../../tangent-bundle.md) is trivial, equivalently when it possesses a global smooth frame. The circle $S^1$ is an example, with its nowhere-vanishing unit tangent field. The sphere $S^3$ is another: regard it as the [unit quaternions](../../../../../unit-quaternion.md). At a [unit quaternion](../../../../../unit-quaternion.md) $q$, the three tangent vectors $qi,qj,qk$ are independent and smoothly depend on $q$. [Quaternion](../../../../../quaternion.md) multiplication preserves the [norm](../../../../../norm.md), so these form an orthonormal frame. This gives the [quaternionic left-invariant frame on the three-sphere](../../../../../quaternionic-left-invariant-frame-on-the-three-sphere.md).

For any [Lie group](../../../../../lie-group.md) $G$ of dimension $n$, choose a [basis](../../../../../basis.md) $E_1,\ldots,E_n$ of $T_eG$. [Left translations](../../../../../left-and-right-translation-on-a-lie-group.md) define

$$
X_i(g)=(dL_g)_eE_i.
$$

These fields are smooth; at every $g$, the differential of the [diffeomorphism](../../../../../diffeomorphism.md) $L_g$ is invertible, so they are a [basis](../../../../../basis.md) of $T_gG$. Hence **every [Lie group](../../../../../lie-group.md) manifold is [parallelizable](../../../../../parallelizable-manifold.md)**, as in [parallelization of a Lie group by left translations](../../../../../parallelization-of-a-lie-group-by-left-translations.md).

For a real [semisimple Lie group](../../../../../semisimple-lie-group.md), let $B(X,Y)=\operatorname{tr}(\operatorname{ad}X\operatorname{ad}Y)$ be the [Killing form](../../../../../killing-form.md). It is nondegenerate and invariant under the adjoint action. Left translating $B$ gives a [bi-invariant pseudo-Riemannian metric](../../../../../bi-invariant-pseudo-riemannian-metric.md). For left-invariant fields, the [Koszul formula](../../../../../koszul-formula.md) reduces to

$$
2B(\nabla_XY,Z)
=B([X,Y],Z)-B([Y,Z],X)+B([Z,X],Y)
=B([X,Y],Z).
$$

Thus $\nabla_XY=[X,Y]/2$. The curvature convention of Question 1 gives

$$
\begin{aligned}
R(X,Y)Z
&=\frac14[X,[Y,Z]]-\frac14[Y,[X,Z]]-\frac12[[X,Y],Z]\\
&=-\frac14[[X,Y],Z].
\end{aligned}
$$

To obtain the [Ricci tensor](../../../../../ricci-tensor.md), trace the [linear map](../../../../../linear-map.md) $X\mapsto R(X,Y)Z$. Since $[[X,Y],Z]=\operatorname{ad}Z\,\operatorname{ad}Y\,X$,

$$
\boxed{\operatorname{Ric}(Y,Z)=-\frac14B(Y,Z)=-\frac14g(Y,Z).}
$$

This proves the [Killing-form Einstein metric](../../../../../killing-form-einstein-metric.md) construction for every real [semisimple group](../../../../../semisimple-lie-group.md). If $G$ is compact semisimple, $-B$ is positive definite and its [Ricci tensor](../../../../../ricci-tensor.md) is $-\tfrac14B=\tfrac14g$, giving a Riemannian [Einstein metric](../../../../../einstein-metric.md). For a noncompact [semisimple group](../../../../../semisimple-lie-group.md) the general Killing-form construction is indefinite. Thus the unrestricted assertion is understood in the pseudo-Riemannian sense appropriate here; positive definiteness is not obtained by simply taking $-B$ in the noncompact case.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 64](../../paper-64-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
