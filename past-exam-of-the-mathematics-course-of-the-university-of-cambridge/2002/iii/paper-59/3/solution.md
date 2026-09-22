<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [solid body transform](../../../../../rigid-transformation.md) is a [rigid transformation](../../../../../rigid-transformation.md): it preserves distances within the object. In three-dimensional coordinates it has the form $T(x)=Rx+b$, with translation $b\in\mathbb R^3$ and an [orthogonal matrix](../../../../../orthogonal-matrix.md) $R$. For a proper physical rotation, the coefficient constraints are

$$
\boxed{R^TR=I,\qquad\det R=1.}
$$

Equivalently the columns of $R$ are an [orthonormal basis](../../../../../orthonormal-basis.md) with positive orientation. A reflection also preserves distance but has $\det R=-1$ and is excluded when “solid-body motion” means a rotation and translation. There are three rotational and three translational degrees of freedom, not twelve independent matrix coefficients.

Computationally use the [homogeneous coordinates](../../../../../homogeneous-coordinate.md) representation

$$
\begin{pmatrix}T(x)\\1\end{pmatrix}
=\begin{pmatrix}R&b\\0&1\end{pmatrix}\begin{pmatrix}x\\1\end{pmatrix}.
$$

The last row is $(0,0,0,1)$; matrix multiplication composes transforms. Alternatively store a unit [quaternion](../../../../../quaternion.md) together with $b$, maintaining its unit norm. A transpose gives the rotational inverse: $T^{-1}(y)=R^T(y-b)$.

Write the cubic [Bézier curve](../../../../../bezier-curve.md) as $P(t)=\sum_{i=0}^3B_i^3(t)p_i$, where $B_i^3(t)=\binom3i(1-t)^{3-i}t^i$. The [binomial theorem](../../../../../binomial-theorem.md) gives $\sum_iB_i^3(t)=1$. Transforming the controls produces

$$
\begin{aligned}
\widetilde P(t)&=\sum_{i=0}^3B_i^3(t)(Rp_i+b)\\
&=R\sum_{i=0}^3B_i^3(t)p_i+b\sum_{i=0}^3B_i^3(t)\\
&=\boxed{RP(t)+b=T(P(t)).}
\end{aligned}
$$

This proves pointwise equivariance, including the original parameter values; it is stronger than a statement that the two curves merely have the same shape.

Orthogonality was not used in the calculation. The identical proof applies to **every [affine map](../../../../../affine-map.md) $T(x)=Ax+b$**, including scales, shears and even singular affine maps. It applies to every representation $P(u)=\sum_i\phi_i(u)p_i$ with scalar, control-independent [partition of unity](../../../../../partition-of-unity.md) basis functions: [Bézier curves](../../../../../bezier-curve.md) of every degree, [B-splines](../../../../../b-spline.md), surfaces built on a [tensor-product surface basis](../../../../../tensor-product-surface-basis.md), [triangular Bézier patches](../../../../../triangular-bezier-patch.md), and more general linear control-point representations. Positivity is not needed for [affine equivariance of a geometric basis](../../../../../affine-equivariance-of-a-geometric-basis.md). For linear stationary [subdivision matrices](../../../../../subdivision-matrix.md) with row sums one, each refinement step commutes with the affine transformation; taking a convergent limit proves the corresponding assertion for [subdivision curves](../../../../../subdivision-curve.md) and [subdivision surfaces](../../../../../subdivision-surface.md). Rules with geometry-dependent nonlinear weights require separate equivariance tests and are not covered automatically.

The affine class is the largest class that preserves every such Euclidean-control construction with unchanged basis weights, under the usual continuity assumption. In fact the degree-one case would force

$$
T((1-t)x+ty)=(1-t)T(x)+tT(y)
$$

for all $x,y$ and $0\le t\le1$. This segment identity, followed by continuity, forces $T$ to be affine. Nonlinear transforms such as perspective division generally fail it.

There is a further extension when the representation itself is enlarged: apply a [projective transformation](../../../../../projective-linear-transformation.md) linearly to homogeneous controls $(w_ip_i,w_i)$, then dehomogenize the weighted sum. The transformed objects are rational [Bézier curves](../../../../../bezier-curve.md) or [non-uniform rational B-splines](../../../../../non-uniform-rational-b-spline.md), with transformed weights as well as transformed Euclidean controls. This works wherever the new denominator is nonzero. It does not assert projective invariance of ordinary polynomial [Bézier curves](../../../../../bezier-curve.md) with their old weights.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 59](../../paper-59-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
