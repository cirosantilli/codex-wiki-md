<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $R_t$ be the horizontal [rotation matrix](../../../../rotation-matrix.md) through [angle](../../../../angle.md) $t$. Define the [screw motion](../../../../screw-motion.md)

$$
\boxed{\Phi_t(x,y,z)=(x\cos t-y\sin t,\ x\sin t+y\cos t,\ z+t).}
$$

Its linear part is an orthogonal [matrix](../../../../matrix.md) with [determinant](../../../../determinant.md) one, and its remaining part is a translation. Thus it is a [proper Euclidean motion of Euclidean three-space](../../../../proper-euclidean-motion-of-euclidean-three-space.md), with $\Phi_s\Phi_t=\Phi_{s+t}$.

In horizontal-vector notation the given [parametric surface](../../../../parametric-surface.md) satisfies $\mathbf r(u,v)=(R_v(1+\cos u,\sin u),v)$. Therefore

$$
\Phi_t(\mathbf r(u,v))=\mathbf r(u,v+t).
$$

The defining circle in each horizontal plane is entirely parametrized by $u$, so $\mathbf r$ covers $X$. The displayed equality and $\Phi_{-t}=\Phi_t^{-1}$ prove $\Phi_t(X)=X$. This [one-parameter subgroup](../../../../one-parameter-subgroup.md) preserves the [dot products](../../../../dot-product.md) and [cross products](../../../../cross-product.md) defining $I$, $II$ and the chosen [unit normal](../../../../unit-normal.md). Consequently their coordinate coefficients, and the [Gaussian curvature](../../../../gaussian-curvature.md), depend only on $u$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
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
