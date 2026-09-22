<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $M$ be the given closed three-dimensional [manifold](../../../../../../topological-manifold.md). It is connected by the meaning of simply connected. An [orientation](../../../../../../orientation-of-a-simplex.md) chosen at one point can be transported along paths, and its sign change around loops defines a homomorphism $\pi_1(M)\to\{\pm1\}$. Since the [fundamental group](../../../../../../fundamental-group.md) is trivial, this monodromy vanishes; thus $M$ is [orientable](../../../../../../orientable-surface.md).

The first [homology group](../../../../../../homology-group.md) is the [abelianization](../../../../../../abelianization.md) of the [fundamental group](../../../../../../fundamental-group.md), giving $H_1(M;\mathbb Z)=0$. Also $H_0(M;\mathbb Z)=\mathbb Z$. The [universal coefficient theorem for cohomology](../../../../../../universal-coefficient-theorem-for-cohomology.md) in degree one gives

$$
0\longrightarrow\operatorname{Ext}_{\mathbb Z}^1(H_0(M),\mathbb Z)
\longrightarrow H^1(M;\mathbb Z)
\longrightarrow\operatorname{Hom}(H_1(M),\mathbb Z)\longrightarrow0.
$$

Both outer groups vanish: the first because $\mathbb Z$ is free and the second because $H_1=0$. Hence $H^1=0$. Integral [Poincare duality](../../../../../../poincare-duality.md) now gives $H_2(M;\mathbb Z)\cong H^1(M;\mathbb Z)=0$ and $H_3(M;\mathbb Z)\cong H^0(M;\mathbb Z)=\mathbb Z$. Homology in degrees greater than three vanishes by the same duality with negative-degree [cohomology](../../../../../../cohomology-split.md). Consequently

$$
\boxed{H_i(M;\mathbb Z)=
\begin{cases}
\mathbb Z,&i=0,3,\\
0,&\text{otherwise}.
\end{cases}}
$$

These are precisely the [homology of a sphere](../../../../../../homology-of-a-sphere.md) for $S^3$, proving that [simply connected closed three-manifolds are homology spheres](../../../../../../simply-connected-closed-three-manifolds-are-homology-spheres.md). No [homeomorphism](../../../../../../homeomorphism.md) classification of three-manifolds is needed.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
