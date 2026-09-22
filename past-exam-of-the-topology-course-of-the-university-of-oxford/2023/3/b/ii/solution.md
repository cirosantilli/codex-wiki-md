<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the same $4\times4$ square grid with four centre-based triangles per small square, but identify boundary points by

$$
(x,y)\sim(1-x,1-y)\qquad\text{for }(x,y)\in\partial Q.
$$

This gives the [real projective plane](../../../../../real-projective-plane.md). To see the model explicitly, a radial [homeomorphism](../../../../../homeomorphism.md) from the square, centred at $(1/2,1/2)$, to the [closed disc](../../../../../closed-disc.md) carries the boundary involution to the [antipodal map](../../../../../antipodal-map.md). The map from that disc to the [projective plane](../../../../../projective-plane.md)

$$
(u,v)\longmapsto [u:v:\sqrt{1-u^2-v^2}]
$$

is [continuous](../../../../../continuous-function.md) and [surjective](../../../../../surjective-function.md): every one-dimensional [vector subspace](../../../../../vector-subspace.md) of $\mathbb R^3$ has a [unit vector](../../../../../unit-vector.md) representative in the closed upper hemisphere. Its only identifications are antipodal boundary points. The [compact-to-Hausdorff continuous bijection theorem](../../../../../compact-to-hausdorff-continuous-bijection-theorem.md) therefore identifies this disc [quotient space](../../../../../quotient-topological-space.md) with $\mathbb{RP}^2$.

The square [triangulation](../../../../../triangulation.md) descends to an abstract [simplicial complex](../../../../../simplicial-complex.md) $K_2$. Small-square centres remain distinct interior vertices; each triangle has one centre and two adjacent grid vertices. Boundary pairings identify whole grid edges, while preserving distinct vertices in each triangle, so this is a finite [triangulation](../../../../../triangulation.md) of the [real projective plane](../../../../../real-projective-plane.md). Its counts are $33$ vertices, $96$ edges and $64$ triangles, giving [Euler characteristic](../../../../../euler-characteristic.md) one.

Choose $\sigma$ to be the interior triangle with vertices $(1/4,1/4)$, $(1/2,1/4)$ and $(3/8,3/8)$. Removing its [relative interior](../../../../../relative-interior.md) and cutting from $(0,0)$ to $(1/4,1/4)$ gives the same nine-sided cut disc as before. Parametrize it by a [convex polygon](../../../../../convex-polygon.md), transporting the boundary identifications. Its boundary word is now

$$
\boxed{a\,b\,a\,b\,c\,d\,e\,f\,c^{-1}}.
$$

The boundary involution pairs the two $a$ sides and the two $b$ sides in matching traversal directions; the $c$ pair restores the slit. Leave $d,e,f$ unpaired. The [quotient space](../../../../../quotient-topological-space.md) is

$$
Y=|K_2|\setminus\operatorname{inside}(\sigma),
$$

the [real projective plane](../../../../../real-projective-plane.md) with an open disc removed. In particular it is a [compact](../../../../../compact-space.md) [connected](../../../../../connected-space.md) [surface with boundary](../../../../../surface-with-boundary.md) consisting of one three-edge [circle](../../../../../circle.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
