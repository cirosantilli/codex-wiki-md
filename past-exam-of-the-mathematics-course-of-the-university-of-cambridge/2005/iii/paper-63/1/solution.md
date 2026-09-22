<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A smooth [fiber bundle](../../../../../fiber-bundle-split.md) $\pi:E\to M$ with typical fiber $F$ is locally a product: every base point has a neighborhood $U$ and a [local trivialization](../../../../../local-trivialization.md) $\pi^{-1}(U)\cong U\times F$ commuting with projection to $U$. Its overlap maps act smoothly on $F$. A [principal bundle](../../../../../principal-bundle.md) with structure [Lie group](../../../../../lie-group.md) $G$ has a free right $G$-action, each fiber is one orbit, and the [local trivializations](../../../../../local-trivialization.md) are equivariant for right multiplication on $G$. A smooth [section of a fiber bundle](../../../../../section-fiber-bundle.md) is a map $s:M\to E$ with $\pi\circ s=\operatorname{id}_M$.

For a [principal bundle](../../../../../principal-bundle.md), a global [section of a fiber bundle](../../../../../section-fiber-bundle.md) gives the map

$$
\Phi:M\times G\longrightarrow P,\qquad\Phi(x,g)=s(x)g.
$$

The free transitive action on each fiber makes $\Phi$ bijective. In a local trivialization, write $s(x)=(x,a(x))$; then $\Phi(x,g)=(x,a(x)g)$ and its inverse is $(x,k)\mapsto(x,a(x)^{-1}k)$. Both are smooth and $\Phi$ is equivariant. Conversely, a product [principal bundle](../../../../../principal-bundle.md) has the section $x\mapsto(x,e)$. This proves **a principal bundle is trivial exactly when it has a global section**. The argument depends on the free transitive action: an arbitrary bundle section need not trivialize its bundle.

For an $n$-dimensional [smooth manifold](../../../../../smooth-manifold.md), the [frame bundle](../../../../../frame-bundle.md) has fiber over $x$ consisting of ordered bases of $T_xM$, equivalently linear [isomorphisms](../../../../../isomorphism.md) $u:\mathbb R^n\to T_xM$. Right composition by $GL(n,\mathbb R)$ makes it a [principal bundle](../../../../../principal-bundle.md). If a metric has signature $(p,q)$, its [pseudo-orthonormal frame bundle](../../../../../orthonormal-frame-bundle.md) consists of the isometries $u:\mathbb R^{p,q}\to T_xM$, with structure group $O(p,q)$. In the positive-definite case this is the usual [orthonormal frame bundle](../../../../../orthonormal-frame-bundle.md). Choosing space and time orientations reduces the Lorentzian structure group to its corresponding connected subgroup.

For [Minkowski spacetime](../../../../../minkowski-spacetime.md), use a fixed origin and a standard Lorentzian frame. Every pair consisting of a point and a pseudo-orthonormal frame is the image of this reference pair under a unique affine isometry. Thus, for the full groups,

$$
\boxed{\operatorname{Fr}_\eta(\mathbb R^{1,3})\cong ISO(1,3)=\mathbb R^{1,3}\rtimes O(1,3),\qquad\mathbb R^{1,3}\cong ISO(1,3)/O(1,3).}
$$

Here the first expression denotes the total space of the [orthonormal frame bundle](../../../../../orthonormal-frame-bundle.md), not merely the Lorentz group. Projection sends an affine isometry to the image of the reference point, and the right action of the stabilizer changes its frame.

Realize [de Sitter spacetime](../../../../../de-sitter-spacetime.md) of radius $\ell$ as $\eta_{AB}X^AX^B=\ell^2$ in $\mathbb R^{1,4}$. The ambient [orthogonal group](../../../../../orthogonal-group.md) is transitive on this hyperboloid. Its point stabilizer acts on the Lorentzian tangent space as $O(1,3)$; choosing a tangent orthonormal frame removes that stabilizer completely. Consequently

$$
\boxed{dS_4\cong O(1,4)/O(1,3),\qquad O(dS_4)\cong O(1,4)\longrightarrow dS_4.}
$$

For oriented, time-oriented frames, replace these groups by $SO_0(1,4)$ and $SO_0(1,3)$, and similarly use the proper orthochronous Poincaré group for [Minkowski spacetime](../../../../../minkowski-spacetime.md). The isometries are uniquely determined by their action on a point and its frame, which explains these bundle identifications.

Finally, choose a basis $v_1,\ldots,v_n$ of the [Lie algebra](../../../../../lie-algebra-split.md) $T_eG$. The [left-invariant vector fields](../../../../../left-invariant-vector-field.md) $X_i(g)=(dL_g)_ev_i$ form a basis at every $g$, because $L_g$ is a [diffeomorphism](../../../../../diffeomorphism.md). They give a global [section of a fiber bundle](../../../../../section-fiber-bundle.md) of the [frame bundle](../../../../../frame-bundle.md), so that bundle is trivial. More explicitly,

$$
\boxed{TG\cong G\times\mathfrak g,\qquad(g,v)\longmapsto(dL_g)_ev.}
$$

Thus every [Lie group](../../../../../lie-group.md) is a [parallelizable manifold](../../../../../parallelizable-manifold.md); connectedness is not needed for this construction.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 63](../../paper-63-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
