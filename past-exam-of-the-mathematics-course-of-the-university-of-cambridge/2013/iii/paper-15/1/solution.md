<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

An $n$-dimensional [smooth manifold](../../../../../smooth-manifold.md) is a [Hausdorff space](../../../../../hausdorff-space.md) with a countable topological base, equipped with a [smooth atlas](../../../../../smooth-atlas.md) of [homeomorphisms](../../../../../homeomorphism.md) from open subsets onto open subsets of $\mathbb R^n$, whose overlap maps are smooth [diffeomorphisms](../../../../../diffeomorphism.md). The smooth structure is the maximal [smooth atlas](../../../../../smooth-atlas.md) compatible with these [manifold charts](../../../../../manifold-chart.md). Here manifolds have no boundary unless specified otherwise.

For a space with all the requested topological properties but no such atlas, take the [topological tripod](../../../../../topological-tripod.md): three closed intervals joined at one endpoint. It is a [compact](../../../../../compact-space.md) [connected](../../../../../connected-space.md) subspace of the plane with its induced metric. A countable base of planar rational balls restricts to a countable base, the metric makes it [Hausdorff](../../../../../hausdorff-space.md), and [compactness](../../../../../compact-space.md) gives a finite subcover of every open cover, hence a locally finite refinement and paracompactness.

At an interior point of any arm, arbitrarily small neighborhoods are intervals. A coordinate ball in [dimension](../../../../../dimension-vector-space.md) at least two would remain [connected](../../../../../connected-space.md) after deleting its center; an interval does not. [Dimension](../../../../../dimension-vector-space.md) zero would make the space discrete. Thus any possible [connected](../../../../../connected-space.md) manifold structure would have [dimension](../../../../../dimension-vector-space.md) one. But a sufficiently small neighborhood of the junction, minus the junction, has three components, whereas an interval chart has two. This contradiction rules out even a [topological manifold](../../../../../topological-manifold.md) structure, and hence any smooth one.

The [product smooth structure](../../../../../product-manifold.md) uses [manifold charts](../../../../../manifold-chart.md) $(\phi,\psi):U\times V\to\phi(U)\times\psi(V)\subset\mathbb R^{m+n}$. Transition maps act separately in the two coordinate blocks and are smooth with smooth inverses. Products of countable bases give a countable base, and the product remains [Hausdorff](../../../../../hausdorff-space.md). Therefore $\boxed{\dim(M\times N)=\dim M+\dim N}$ with this natural smooth structure.

Define the [tangent space by point derivations](../../../../../tangent-space-by-point-derivations.md): a tangent vector at $x$ is an $\mathbb R$-linear map $D$ on [germs](../../../../../germ-of-a-sheaf-section.md) of smooth functions at $x$, satisfying $D(ab)=a(x)D(b)+b(x)D(a)$. Addition and scalar multiplication preserve this rule, so these [derivations](../../../../../derivation-of-an-algebra.md) form a [vector space](../../../../../vector-space-split.md). In coordinates $u^1,\ldots,u^n$, the local identity

$$
h(u)-h(u(x))=\sum_i(u^i-u^i(x))h_i(u),\qquad h_i(u(x))=\partial_i h(u(x))
$$

follows by integrating the [derivative](../../../../../derivative.md) of $h$ along the coordinate line segment. [Derivations](../../../../../derivation-of-an-algebra.md) annihilate constants, so it gives $Dh=\sum_iD(u^i)\partial_i h(u(x))$. The coordinate [derivations](../../../../../derivation-of-an-algebra.md) $\partial_i|_x$ are independent since they evaluate the coordinate functions as $\delta_i^j$. Thus

$$
\boxed{T_xM=\operatorname{span}\{\partial_1|_x,\ldots,\partial_n|_x\},\qquad\dim T_xM=n}.
$$

For a [smooth map](../../../../../smooth-map-between-manifolds.md), define the [differential of a smooth map](../../../../../differential-of-a-smooth-map.md) intrinsically by $(f_*D)(h)=D(h\circ f)$. It is again linear and satisfies the [derivation](../../../../../derivation-of-an-algebra.md) rule at $f(x)$, so it maps $T_xM$ into $T_{f(x)}N$. Its coordinate matrix is the Jacobian of the coordinate expression of $f$, independently of the charts by the intrinsic definition and [chain rule](../../../../../chain-rule.md).

Finally, a zero differential forces each target coordinate function to have all [derivatives](../../../../../derivative.md) zero on a small [connected](../../../../../connected-space.md) source coordinate ball mapping into one target chart. Integration on straight segments makes those functions constant there. Hence $f$ is locally constant. Each nonempty fiber is both open and closed, so [connectedness](../../../../../connected-space.md) gives the [zero-differential constancy theorem](../../../../../zero-differential-constancy-theorem.md), $\boxed{f\text{ is constant}}$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 15](../../paper-15-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
