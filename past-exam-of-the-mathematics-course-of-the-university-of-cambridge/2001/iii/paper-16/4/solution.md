<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For $t$ [tetrahedra](../../../../../tetrahedron.md), a [normal surface](../../../../../normal-surface.md) has a vector $x\in\mathbb Z_{\geq0}^{7t}$ counting four triangle types and three quadrilateral types in each [tetrahedron](../../../../../tetrahedron.md). On every glued face, the numbers of arcs of each of its three types must agree on the two sides. These give homogeneous integer [linear equations](../../../../../linear-equation.md)

$$
Ax=0.
$$

For closed [surfaces](../../../../../topological-surface.md) the coordinates of [disks](../../../../../disk-mathematics.md) meeting an unglued [boundary](../../../../../boundary-of-a-set.md) face must also vanish. The nonnegativity and matching equations are not the whole admissibility condition: in each [tetrahedron](../../../../../tetrahedron.md) at most one of its three quadrilateral coordinates can be nonzero. Conversely, for an admissible vector, arrange the prescribed parallel [disks](../../../../../disk-mathematics.md) and glue their face arcs in order. This reconstructs an embedded [normal surface](../../../../../normal-surface.md), unique up to normal [isotopy](../../../../../isotopy.md).

A [fundamental normal surface](../../../../../fundamental-normal-surface.md) corresponds to a nonzero admissible vector which cannot be written as $y+z$ with both $y$ and $z$ nonzero admissible vectors. These indecomposable vectors form a fundamental set: every admissible vector is their finite sum. To find them, fix which quadrilateral type is allowed in each [tetrahedron](../../../../../tetrahedron.md). This leaves the integer points of a rational polyhedral cone $Ax=0,\ x\geq0$, with some coordinates set to zero. Compute its [Hilbert basis of a rational cone](../../../../../hilbert-basis-of-a-rational-cone.md), for example by subdividing into rational simplicial cones and enumerating the lattice points in their fundamental parallelepipeds along with their integral ray generators, then removing decomposable generators. Repeat the finite list of quadrilateral choices, remove duplicates, and remove vectors decomposable in their compatible sector. Finiteness follows because each of these pointed rational cones has a finite Hilbert basis.

Let $E$ be the [link exterior](../../../../../link-exterior.md). By [Alexander duality](../../../../../alexander-duality.md), for a two-component link

$$
H_2(E;\mathbb F_2)\cong\mathbb F_2.
$$

An embedded [connected](../../../../../connected-space.md) closed [surface](../../../../../topological-surface.md) separates $S^3$; its mod-two class is nonzero exactly when the two link components lie on different sides. The connectedness qualification matters: two parallel splitting [spheres](../../../../../sphere.md) form a disconnected [surface](../../../../../topological-surface.md) with zero total class. We use the criterion only for [connected](../../../../../connected-space.md) [surfaces](../../../../../topological-surface.md).

Normalize a splitting [sphere](../../../../../sphere.md) by [isotopy](../../../../../isotopy.md), [disk](../../../../../disk-mathematics.md) compressions and removal of components lying inside [tetrahedra](../../../../../tetrahedron.md). A compression replaces a [sphere](../../../../../sphere.md) by two [spheres](../../../../../sphere.md) whose mod-two classes add to the old class; at least one is still a splitting [sphere](../../../../../sphere.md). The discarded tetrahedral [spheres](../../../../../sphere.md) have zero class. Thus there is a normal splitting [sphere](../../../../../sphere.md). Choose one, $S$, of least [normal surface weight](../../../../../normal-surface-weight.md).

Suppose its vector is decomposable. Realize $S=A+B$ as a [Haken sum](../../../../../haken-sum.md), choosing a decomposition with the least possible number of intersection curves. Two elementary exchange observations are useful. First, $A$ and $B$ can be taken [connected](../../../../../connected-space.md). If their total union has more than two components, perform regular exchanges connecting components until exactly two embedded groups remain, resolving any intersections within each group. Since the final sum is [connected](../../../../../connected-space.md), this can be done before the last joining exchange; it uses up at least one of the old intersection curves. The resulting two [normal surfaces](../../../../../normal-surface.md) still have total vector $x(S)$, contradicting minimality. Second, no intersection curve separates both $A$ and $B$. If it did, resolve that curve first: the two separated sides give two groups. Resolve any remaining self-intersections within each group and continue exchanges between groups only while the result remains disconnected. Just before the exchange making the final [connected](../../../../../connected-space.md) [surface](../../../../../topological-surface.md), there are again exactly two embedded normal groups with fewer intersection curves. Both assertions follow from the local four-bank resolution at an intersection circle; internal crossings are resolved before regarding a group as one embedded summand.

Every closed embedded [surface](../../../../../topological-surface.md) in $S^3$ is [orientable](../../../../../orientable-surface.md). Additivity of [Euler characteristic](../../../../../euler-characteristic.md) in the [Haken sum](../../../../../haken-sum.md) gives

$$
2=\chi(S)=\chi(A)+\chi(B).
$$

For [connected](../../../../../connected-space.md) [orientable](../../../../../orientable-surface.md) closed [surfaces](../../../../../topological-surface.md) the positive [Euler characteristic](../../../../../euler-characteristic.md) is $2$, and the only zero [Euler characteristic](../../../../../euler-characteristic.md) is that of a [torus](../../../../../torus.md). Thus one summand, say $A$, is a [sphere](../../../../../sphere.md) and the other $B$ is a [torus](../../../../../torus.md). Both have smaller weight than $S$. The [sphere](../../../../../sphere.md) $A$ cannot split the link by minimality, so

$$
[A]=0,\qquad [B]=[S]\neq0.
$$

Each intersection circle separates the [sphere](../../../../../sphere.md) $A$, so the second exchange observation makes it nonseparating on $B$. In particular, these circles are essential parallel curves on the [torus](../../../../../torus.md).

Cut $A$ along the intersection circles. There are at least two innermost [disk](../../../../../disk-mathematics.md) patches. Choose one of smallest weight, $D$; then $2w(D)\leq w(A)$. Its interior misses $B$, and its [boundary](../../../../../boundary-of-a-set.md) is essential on $B$. Compress the [torus](../../../../../torus.md) along two slightly separated copies of $D$. The result is a [sphere](../../../../../sphere.md) $C$, and the compression takes place in the exterior, so

$$
[C]=[B]\neq0,\qquad w(C)\leq w(B)+2w(D)\leq w(S).
$$

Thus $C$ is a splitting [sphere](../../../../../sphere.md).

This alone is not quite a contradiction if the last weight inequality is equality: $C$ need not yet be normal. At the compression seam it uses the alternative, rather than regular, exchange between the [disk](../../../../../disk-mathematics.md) patch and the [torus](../../../../../torus.md). An intersection circle of normal [disk](../../../../../disk-mathematics.md) sheets must cross a tetrahedral face; it cannot be a closed curve entirely in two [disk](../../../../../disk-mathematics.md) interiors in one [tetrahedron](../../../../../tetrahedron.md), which can be put in standard position with only intersection arcs. In a face, parallel arcs of the same type do not cross. At a crossing of different normal arc types, the alternative exchange joins two endpoints on the same edge, producing a returning arc. Pushing across its edge bigon strictly reduces weight. Normalize the resulting [surface](../../../../../topological-surface.md), retaining a nonzero-class [sphere](../../../../../sphere.md) at each compression as before. We obtain a normal splitting [sphere](../../../../../sphere.md) of weight strictly less than $w(S)$, a contradiction. Therefore

$$
\boxed{\text{a least-weight normal splitting sphere is fundamental}.}
$$

The [algorithm](../../../../../algorithm.md) is now finite. Triangulate the exterior from a link diagram, enumerate its fundamental admissible vectors with the closed-surface [boundary](../../../../../boundary-of-a-set.md) condition, reconstruct their [surfaces](../../../../../topological-surface.md), and inspect the [connected](../../../../../connected-space.md) components and [Euler characteristics](../../../../../euler-characteristic.md). A fundamental vector yields a [connected](../../../../../connected-space.md) [surface](../../../../../topological-surface.md), since otherwise its component vectors decompose it. A [connected](../../../../../connected-space.md) closed [surface](../../../../../topological-surface.md) in $S^3$ with [Euler characteristic](../../../../../euler-characteristic.md) two is a [sphere](../../../../../sphere.md). Compute its mod-two class in the finite simplicial [chain complex](../../../../../chain-complex.md), or equivalently check which link [boundary](../../../../../boundary-of-a-set.md) tori lie on either side. Answer yes exactly when such a [sphere](../../../../../sphere.md) has nonzero class. The argument proves that every split link is detected, and every detected [sphere](../../../../../sphere.md) witnesses splitting. For more than two components, $H_2(E;\mathbb F_2)\cong\mathbb F_2^{\ell-1}$ and a nonzero [sphere](../../../../../sphere.md) class separates a nonempty proper subset of the components; the same least-weight argument and finite enumeration apply.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 16](../../paper-16-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
