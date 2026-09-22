<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use compatible edge identifications: choose a [bijection](../../../../../bijection.md) between the three boundary vertices of $\tau$ and those of $\sigma$, and extend it linearly on each edge. This defines a [simplicial homeomorphism](../../../../../simplicial-homeomorphism.md) of the two boundary [circles](../../../../../circle.md). This compatibility is the usual meaning of gluing the two boundary triangles; independently chosen edge reversals need not agree at their endpoints. The classification needed here is 3(a)(iv); the printed reference to 3(a)(iii) is a source error.

Delete the two triangular [simplexes](../../../../../simplex.md) but retain all their proper [faces of a simplex](../../../../../face-of-a-simplex.md), and identify the two resulting boundary [simplicial subcomplexes](../../../../../simplicial-subcomplex.md) by this map. The result is a finite abstract [simplicial complex](../../../../../simplicial-complex.md) $L$: vertices from different sides are identified only in the boundary, and the only shared edges are boundary edges. There is no triangle consisting of all three boundary vertices after the two faces have been removed. Consequently no other [simplexes](../../../../../simplex.md) become duplicates. Its [geometric realization](../../../../../geometric-realization-of-a-simplicial-complex.md) has the specified [quotient topology](../../../../../quotient-topology.md) and is [homeomorphic](../../../../../homeomorphism.md) to $Z$.

We check the [closed combinatorial surface](../../../../../closed-combinatorial-surface.md) conditions. Away from the seam, vertex [links of a simplex](../../../../../link-of-a-simplex.md) remain [cycle graphs](../../../../../cycle-graph.md). At a boundary vertex of $X$ or $Y$, removing the face changes its link from a [cycle graph](../../../../../cycle-graph.md) to a [graph path](../../../../../path-in-a-graph.md), with endpoints corresponding to its two boundary edges. Gluing the boundaries identifies the two paths' respective endpoints, making one [cycle graph](../../../../../cycle-graph.md). Each seam edge now meets one triangle from $X$ and one from $Y$, and all other edges retain their original two incident triangles. Thus every vertex link is a [cycle graph](../../../../../cycle-graph.md) and every [simplex](../../../../../simplex.md) lies in a triangle. The [simplicial complex](../../../../../simplicial-complex.md) is [connected](../../../../../connected-space.md), since the two [connected](../../../../../connected-space.md) punctured surfaces meet along their boundary [circle](../../../../../circle.md). Hence $L$ is a [closed combinatorial surface](../../../../../closed-combinatorial-surface.md).

This construction is the [connected sum of surfaces](../../../../../connected-sum-of-surfaces.md) $T^2\mathbin\#\mathbb{RP}^2$. For completeness, compute its [Euler characteristic](../../../../../euler-characteristic.md) directly. Removing a triangular face while retaining its edges and vertices subtracts one, so

$$
\chi(X)=0-1=-1,\qquad \chi(Y)=1-1=0.
$$

Gluing identifies three vertex pairs and three edge pairs, giving

$$
\chi(Z)=\chi(X)+\chi(Y)-3+3=-1.
$$

For the explicit [triangulations](../../../../../triangulation.md) above, this is also $62-189+126=-1$.

Finally $Z$ is a [nonorientable surface](../../../../../non-orientable-surface.md). If $Z$ were [orientable](../../../../../orientable-surface.md), its [restriction](../../../../../restriction-mathematics.md) would make $Y$ [orientable](../../../../../orientable-surface.md). The consistent choices of [orientation of a simplex](../../../../../orientation-of-a-simplex.md) on its triangles extend across a capping [disc](../../../../../topological-disc.md): choose the cap's [orientation of a simplex](../../../../../orientation-of-a-simplex.md) so that the induced directions on the common boundary oppose. Capping $Y$ by $\sigma$ would therefore make the [real projective plane](../../../../../real-projective-plane.md) [orientable](../../../../../orientable-surface.md), a contradiction. The obstruction to [orientability](../../../../../orientability.md) in the [real projective plane](../../../../../real-projective-plane.md) can also be seen from a [Möbius band](../../../../../mobius-band.md) neighbourhood of a [projective line](../../../../../projective-line.md).

By the [classification theorem for closed combinatorial surfaces](../../../../../classification-theorem-for-closed-combinatorial-surfaces.md), a [nonorientable surface](../../../../../non-orientable-surface.md) with [Euler characteristic](../../../../../euler-characteristic.md) $-1$ has $2-k=-1$, hence $k=3$. Therefore

$$
\boxed{Z\cong\mathbb{RP}^2\mathbin\#\mathbb{RP}^2\mathbin\#\mathbb{RP}^2=N_3}.
$$

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the topology course of the University of Oxford](../../../../split.md)
6. [Topology course of the University of Oxford](../../../../../topology-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
