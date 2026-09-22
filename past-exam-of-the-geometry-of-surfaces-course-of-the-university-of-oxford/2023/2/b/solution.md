<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Every nonidentity [biholomorphism](../../../../biholomorphism.md) in the finite [group](../../../../group-split.md) $G$ has only finitely many fixed points, by the [identity theorem on a Riemann surface](../../../../identity-theorem-on-a-riemann-surface.md) and [compactness](../../../../compact-space.md). Because the [group action](../../../../group-action-split.md) is a [faithful group action](../../../../faithful-group-action.md), the union of these finite sets does not exhaust $X$. A point outside this union has trivial [stabilizer subgroup](../../../../stabilizer-subgroup.md), so its [group orbit](../../../../orbit-group-theory.md) has $|G|$ points by the [orbit-stabilizer theorem](../../../../orbit-stabilizer-theorem.md). The generic [fiber of a function](../../../../fiber-of-a-function.md) of the projection is such an [group orbit](../../../../orbit-group-theory.md), giving

$$
\boxed{\deg f=|G|.}
$$

More precisely, put $H=G_x$ and $m=|H|$. Differentiation at $x$ gives a [group homomorphism](../../../../group-homomorphism.md) $H\to\mathbb C^\times$. It is [injective](../../../../injective-function.md): if a nonidentity finite-order germ had the form $h(z)=z+a_kz^k+O(z^{k+1})$ with $k\geq2$ and $a_k\ne0$, then its $q$th iterate would begin $z+qa_kz^k$, so no positive iterate could be the identity. A germ equal to the identity gives the identity on $X$ by the [identity theorem on a Riemann surface](../../../../identity-theorem-on-a-riemann-surface.md). Thus $H$ is a [cyclic group](../../../../cyclic-group.md), with derivative image the $m$th [roots of unity](../../../../root-of-unity.md).

For completeness, an explicit local coordinate linearizing $H$ is

$$
w(p)=\frac1m\sum_{h\in H}h'(x)^{-1}z(hp).
$$

It has $w'(x)=1$, and reindexing the sum gives $w(hp)=h'(x)w(p)$. Therefore a coordinate on the local [quotient space](../../../../quotient-topological-space.md) is $w^m$. Other translates of a sufficiently small [neighbourhood](../../../../neighbourhood-mathematics.md) of $x$ are disjoint unless their translating element lies in $H$, so this local [quotient space](../../../../quotient-topological-space.md) is also a chart for $X/G$. The [local cyclic quotient of a Riemann surface](../../../../local-cyclic-quotient-of-a-riemann-surface.md) consequently gives

$$
\boxed{\nu_f(x)=|G_x|.}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the geometry of surfaces course of the University of Oxford](../../../split.md)
5. [Geometry of surfaces course of the University of Oxford](../../../../geometry-of-surfaces-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
