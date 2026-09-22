<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The possible ranks and the corresponding [homeomorphism](../../../../../homeomorphism.md) types are

$$
\boxed{n=0:\ S^3;\qquad n=1:\ S^2\times S^1;\qquad n=3:\ T^3.}
$$

There is no example for $n=2$ or $n\geq4$. The uniqueness here is topological, not uniqueness of a [Riemannian metric](../../../../../riemannian-metric.md).

To see the restrictions, use the [prime decomposition of a closed orientable three-manifold](../../../../../prime-decomposition-of-a-closed-orientable-three-manifold.md). Its [fundamental group](../../../../../fundamental-group.md) is the [free product](../../../../../free-product.md) of the [prime three-manifold](../../../../../prime-three-manifold.md) groups. A [free product](../../../../../free-product.md) of two nontrivial groups is nonabelian, so at most one summand can have nontrivial [fundamental group](../../../../../fundamental-group.md). The remaining [simply connected](../../../../../simply-connected-space.md) summands are three-spheres by the [Poincaré conjecture](../../../../../poincare-conjecture.md). If the nontrivial summand is not irreducible, it is $S^2\times S^1$, giving rank one. If it is irreducible and has infinite [fundamental group](../../../../../fundamental-group.md), the [sphere theorem for three-manifolds](../../../../../sphere-theorem-for-three-manifolds.md) makes it [aspherical](../../../../../aspherical-space.md). Its [fundamental group](../../../../../fundamental-group.md) is then a dimension-three [Poincare duality group](../../../../../poincare-duality-group.md). But $\mathbb Z^n$ is a duality group of dimension $n$, as seen from the [torus](../../../../../torus.md) classifying space or its [Koszul resolution](../../../../../koszul-resolution.md), so $n=3$.

For rank three, the flat case of the [geometrization theorem](../../../../../geometrization-conjecture.md) says that a closed irreducible orientable [three-manifold](../../../../../3-manifold.md) with [fundamental group](../../../../../fundamental-group.md) $\mathbb Z^3$ admits a flat metric. Write it as $\mathbb R^3/\Gamma$. By the [Bieberbach theorem](../../../../../bieberbach-theorem.md), $\Gamma$ contains a full-rank translation lattice $\Lambda$. If $g=(R,v)\in\Gamma$ commutes with translation by each $\lambda\in\Lambda$, then $R\lambda=\lambda$ for every lattice vector, forcing $R=I$. Since $\Gamma$ itself is abelian, it consists entirely of translations. Its quotient is therefore the three-torus. Rank zero follows directly from the [Poincaré conjecture](../../../../../poincare-conjecture.md), and rank one was already determined by the [prime decomposition of a closed orientable three-manifold](../../../../../prime-decomposition-of-a-closed-orientable-three-manifold.md). Historically, before the Poincare theorem, the uniqueness conclusions were phrased allowing [connected sums](../../../../../connected-sum-of-oriented-manifolds.md) with [homotopy](../../../../../homotopy.md) three-spheres; the modern theorem removes that ambiguity.

The six flat types below mean the six **closed orientable** flat [three-manifold](../../../../../3-manifold.md) types. There are infinitely many individual flat metrics and there are additional noncompact [flat Riemannian manifolds](../../../../../flat-manifold.md). In each closed case the [universal cover](../../../../../universal-cover.md) is [Euclidean space](../../../../../euclidean-norm.md) and the [deck transformation group](../../../../../deck-transformation-group.md) is a torsion-free crystallographic group. The [holonomy groups of closed orientable flat three-manifolds](../../../../../holonomy-groups-of-closed-orientable-flat-three-manifolds.md) are $1,C_2,C_3,C_4,C_6,C_2\times C_2$.

The first is a [flat torus](../../../../../flat-torus.md) $\mathbb R^3/\Lambda$, with trivial holonomy. For each cyclic case choose a planar lattice $L$ admitting the relevant rotation $R_m$, and generate the [deck transformation group](../../../../../deck-transformation-group.md) by translations in $L$ and the screw

$$
s_m(v,z)=(R_mv,z+1/m),\qquad m=2,3,4,6.
$$

Its $m$th power is unit translation along the axis. A nontrivial holonomy element has nonzero axial displacement modulo integers, so has no fixed point. All transformations preserve orientation. A compact prism [fundamental domain](../../../../../fundamental-domain.md) gives compactness. Equivalently, the manifold is a [torus](../../../../../torus.md) [mapping torus](../../../../../mapping-torus.md) with finite-order [monodromy](../../../../../monodromy.md). In planar lattice bases one may take

$$
R_2=-I,\quad
R_3=\begin{pmatrix}-1&-1\\1&0\end{pmatrix},\quad
R_4=\begin{pmatrix}0&-1\\1&0\end{pmatrix},\quad
R_6=\begin{pmatrix}0&-1\\1&1\end{pmatrix}.
$$

The half-turn uses any planar lattice, the quarter-turn a square lattice, and the third- and sixth-turns a hexagonal lattice. These give respectively the [half-turn flat three-manifold](../../../../../half-turn-flat-three-manifold.md), [third-turn flat three-manifold](../../../../../third-turn-flat-three-manifold.md), [quarter-turn flat three-manifold](../../../../../quarter-turn-flat-three-manifold.md), and [sixth-turn flat three-manifold](../../../../../sixth-turn-flat-three-manifold.md). Their holonomies have orders $2,3,4,6$, and their first [Betti numbers](../../../../../betti-number.md) are all one, since the only fixed direction of holonomy is the screw axis.

The sixth type is the [Hantzsche-Wendt manifold](../../../../../hantzsche-wendt-manifold.md). A concrete group is generated by

$$
\alpha(x,y,z)=(x+1/2,-y,-z),\qquad
\beta(x,y,z)=(-x,y+1/2,-z+1/2).
$$

Their linear parts are commuting half-turns about perpendicular axes. Moreover $\alpha^2$, $\beta^2$ and $(\alpha\beta)^2$ are translations by $(1,0,0)$, $(0,1,0)$ and $(0,0,-1)$. Their translation subgroup is the unit cubic lattice and their linear quotient is $C_2\times C_2$. In each nontranslation coset, the displacement along the fixed axis is a half-integer, so the action is free. The quotient is compact and orientable. No vector is fixed by both linear parts, so its first [Betti number](../../../../../betti-number.md) is zero. Bieberbach classification gives precisely these six affine types; the explicit screw descriptions distinguish them without identifying arbitrary finite quotients with holonomy.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 28](../../paper-28-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
