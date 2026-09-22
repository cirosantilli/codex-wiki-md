<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a [smooth manifold](../../../../../smooth-manifold.md) $M$ of dimension $n$, the [tangent space](../../../../../tangent-space.md) $T_pM$ can be defined as the space of derivations at $p$: linear maps $v$ on germs of smooth real functions satisfying $v(fg)=f(p)v(g)+g(p)v(f)$. Equivalently, $v$ is the velocity of a [smooth curve](../../../../../smooth-curve.md) through $p$, with curves identified when their coordinate velocities agree. A chart $(x^1,\ldots,x^n)$ supplies the basis $\partial_i|_p$, so $v=v^i\partial_i|_p$.

The [tangent bundle](../../../../../tangent-bundle.md) is the disjoint union $TM=\coprod_{p\in M}T_pM$, with projection $\pi(v)=p$. Its smooth structure is defined by the local [local trivializations](../../../../../local-trivialization.md)

$$
\pi^{-1}(U)\longrightarrow x(U)\times\mathbb R^n,\qquad (p,v)\longmapsto(x(p),v^1,\ldots,v^n).
$$

On overlapping charts, the change of trivialization is

$$
(x,v)\longmapsto\bigl(y(x),Dy(x)v\bigr).
$$

These are smooth changes of coordinates on a $2n$-dimensional [smooth manifold](../../../../../smooth-manifold.md), linear and invertible in each fibre. Thus $TM$ is a rank-$n$ [vector bundle](../../../../../vector-bundle.md), and its projection is a [submersion](../../../../../submersion.md). Fibrewise addition, scalar multiplication and the zero section are smooth. A smooth [section of a vector bundle](../../../../../section-of-a-vector-bundle.md) $X:M\to TM$, satisfying $\pi\circ X=\operatorname{id}_M$, is exactly a [vector field](../../../../../vector-field.md); locally $X=X^i\partial_i$, with components transforming by the displayed [Jacobian matrix](../../../../../jacobian-matrix.md). Its action on functions is a derivation, and the commutator of two such derivations is their [Lie bracket](../../../../../lie-bracket.md).

The [dual bundle](../../../../../dual-bundle.md) of $TM$ is the [cotangent bundle](../../../../../cotangent-bundle.md) $T^*M$. Its smooth [sections of a vector bundle](../../../../../section-of-a-vector-bundle.md) are [differential 1-forms](../../../../../one-form.md), locally $\alpha=\alpha_i\,dx^i$. The coefficient transformation is the inverse transpose of that for tangent vectors, ensuring that $\alpha(X)$ is a well-defined smooth function. Tensoring these two bundles gives the [tensor bundles](../../../../../tensor-bundle.md)

$$
T^r_sM=(TM)^{\otimes r}\otimes(T^*M)^{\otimes s}.
$$

Their [sections of a vector bundle](../../../../../section-of-a-vector-bundle.md) are [tensor fields](../../../../../tensor-field.md); their [transition functions of a vector bundle](../../../../../transition-function-of-a-vector-bundle.md) are the corresponding tensor products of the tangent and cotangent transformations. For example, the bundle $\operatorname{End}(TM)=TM\otimes T^*M$ contains fields of linear endomorphisms, while $S^2T^*M$ contains symmetric bilinear fields. Taking alternating covariant tensors gives $\Lambda^kT^*M$, whose sections are [differential forms](../../../../../differential-form-split.md). The [wedge product](../../../../../exterior-product.md), [exterior derivative](../../../../../exterior-derivative.md) and [pullback of a differential form](../../../../../pullback-of-a-differential-form.md) make these bundles central to integration, [Generalized Stokes theorem](../../../../../generalized-stokes-theorem.md) and [de Rham cohomology](../../../../../de-rham-cohomology.md).

A nowhere-vanishing section of $\Lambda^nT^*M$ chooses an [orientation of a smooth manifold](../../../../../orientation-of-a-smooth-manifold.md); such a section exists exactly when $M$ is orientable. Without an [orientation of a smooth manifold](../../../../../orientation-of-a-smooth-manifold.md), one can still integrate sections of the [density bundle](../../../../../density-bundle.md) $|\Lambda^nT^*M|$, whose coordinate changes use the absolute [Jacobian determinant](../../../../../jacobian-determinant.md). A [Riemannian metric](../../../../../riemannian-metric.md) is a positive-definite section $g$ of $S^2T^*M$. It identifies $TM$ with $T^*M$ by the [musical isomorphisms](../../../../../musical-isomorphism.md) $X\mapsto g(X,\cdot)$ and gives the [Riemannian volume density](../../../../../riemannian-volume-density.md)

$$
\sqrt{\det(g_{ij})}\,|dx^1\cdots dx^n|.
$$

On an oriented [smooth manifold](../../../../../smooth-manifold.md), this density corresponds to a [volume form](../../../../../volume-form.md).

Another organizing construction is the [frame bundle](../../../../../frame-bundle.md) $FM$. A frame over $p$ is a linear isomorphism $u:\mathbb R^n\to T_pM$, and the right action $u\cdot A=u\circ A$ makes $FM$ a [principal bundle](../../../../../principal-bundle.md) with [general linear group](../../../../../general-linear-group.md) $GL(n,\mathbb R)$ as its structure group. Given a [group representation](../../../../../group-representation.md) $\rho:GL(n,\mathbb R)\to GL(V)$, the [associated bundle](../../../../../associated-bundle.md) $FM\times_\rho V$ is obtained from pairs $(u,v)$ by the relation $(uA,v)\sim(u,\rho(A)v)$. The standard representation reconstructs $TM$; dual, tensor and exterior representations reconstruct the associated bundles described above. A [Riemannian metric](../../../../../riemannian-metric.md) reduces the [frame bundle](../../../../../frame-bundle.md) to the [orthonormal frame bundle](../../../../../orthonormal-frame-bundle.md), with [orthogonal group](../../../../../orthogonal-group.md) $O(n)$ as structure group; an [orientation of a smooth manifold](../../../../../orientation-of-a-smooth-manifold.md) reduces it further to the [special orthogonal group](../../../../../special-orthogonal-group.md) $SO(n)$. A global section of $FM$ is a global frame, so it exists exactly when $M$ is a [parallelizable manifold](../../../../../parallelizable-manifold.md). Local triviality does not imply a global trivialization: the [Hairy ball theorem](../../../../../hairy-ball-theorem.md) prevents even one nowhere-zero [vector field](../../../../../vector-field.md) on $S^2$.

A [connection on a vector bundle](../../../../../connection-vector-bundle.md) differentiates its sections in tangent directions and defines [parallel transport](../../../../../parallel-transport.md). For $TM$, the [Levi-Civita connection](../../../../../levi-civita-connection.md) is distinguished by compatibility with a [Riemannian metric](../../../../../riemannian-metric.md) and vanishing [torsion tensor](../../../../../torsion-tensor.md). Its coefficients are not tensor components, because a coordinate change introduces second derivatives; the difference of two connections is a section of $T^*M\otimes\operatorname{End}(TM)$. The [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) is a genuine tensor measuring the failure of covariant derivatives to commute.

Finally, a smooth map $f:M\to N$ gives the [pullback tangent bundle](../../../../../pullback-tangent-bundle.md) $f^*TN$. Its sections are [vector fields along a map](../../../../../vector-field-along-a-map.md), including the velocity of a [curve](../../../../../curve.md) and [Jacobi fields](../../../../../jacobi-field.md) along a [geodesic](../../../../../geodesic.md). For an embedded [submanifold](../../../../../submanifold.md) $i:M\hookrightarrow N$, the derivative identifies $TM$ with a subbundle of $i^*TN$, and the quotient is the [normal bundle](../../../../../normal-bundle.md). With an ambient [Riemannian metric](../../../../../riemannian-metric.md), the [normal bundle](../../../../../normal-bundle.md) is identified with the orthogonal complement of $TM$ in $i^*TN$; the [second fundamental form](../../../../../second-fundamental-form-split.md) records the normal component of the ambient derivative of tangent fields. These constructions connect the bundle description to both intrinsic and extrinsic [differential geometry](../../../../../differential-geometry-split.md).

**The tangent bundle is a rank-$n$ smooth vector bundle over an $n$-manifold; its dual, tensor, exterior, frame and pullback constructions encode the principal geometric fields and their natural operations.**

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
