<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Three useful geometric properties, with their concrete consequences here, are:

- **Endpoint interpolation.** $F(0)=A=(-2,0)$ and $F(1)=C=(0,0)$. The middle [control point](../../../../../control-point.md) $B$ is a handle, not an interpolated [point](../../../../../point-geometry.md): $F_y(t)\le1/2$, so the [curve](../../../../../curve.md) never reaches $B=(0,1)$.
- **Endpoint tangents.** $F'(0)=2(B-A)=(4,2)$ and $F'(1)=2(C-B)=(0,-2)$. Thus the [tangent lines](../../../../../tangent-line.md) are parallel to the first and last sides of the [control polygon](../../../../../control-polygon.md), respectively; both endpoint [derivatives](../../../../../derivative.md) are nonzero.
- **Convex-hull containment.** The three [Bernstein basis](../../../../../bernstein-basis.md) weights are nonnegative and sum to one on $[0,1]$. Every $F(t)$ is therefore a [convex combination](../../../../../convex-combination.md) of $A,B,C$, so the entire [Bézier curve](../../../../../bezier-curve.md) lies in their filled [triangle](../../../../../triangle.md).

These give the compact answer

$$
\boxed{\text{endpoint interpolation; control-edge endpoint tangents; convex-hull containment}.}
$$

The same sum-to-one calculation also explains [affine equivariance of a geometric basis](../../../../../affine-equivariance-of-a-geometric-basis.md): applying an [affine map](../../../../../affine-map.md) to the handles applies that map to the [curve](../../../../../curve.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Geometric modelling](../../../geometric-modelling-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
