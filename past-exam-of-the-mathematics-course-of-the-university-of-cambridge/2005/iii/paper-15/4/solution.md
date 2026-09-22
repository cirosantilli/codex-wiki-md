<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $D$ be the ambient [Levi-Civita connection](../../../../../levi-civita-connection.md) and $\nabla$ the one for the [induced metric](../../../../../induced-metric.md) on $M$. The [Gauss formula](../../../../../gauss-formula.md) is

$$
D_XY=\nabla_XY+II(X,Y),
$$

where the [second fundamental form](../../../../../second-fundamental-form-split.md) $II(X,Y)=(D_XY)^\perp$ is normal. The tangential part of $D$ is [metric-compatible](../../../../../metric-connection.md) and [torsion-free](../../../../../torsion-free-connection.md), so the [existence and uniqueness of the Levi-Civita connection](../../../../../existence-and-uniqueness-of-the-levi-civita-connection.md) identifies it with $\nabla$.

For a normal field $\xi$, the [Weingarten formula](../../../../../weingarten-formula.md) defines the [shape operator in a normal direction](../../../../../shape-operator-in-a-normal-direction.md) $A_\xi$ and the [normal connection](../../../../../normal-connection.md) by

$$
D_X\xi=-A_\xi X+\nabla_X^\perp\xi.
$$

Differentiate $\langle\xi,Y\rangle=0$ using metric compatibility to get

$$
\langle A_\xi X,Y\rangle=\langle II(X,Y),\xi\rangle.
$$

The [symmetry of the second fundamental form](../../../../../symmetry-of-the-second-fundamental-form.md) follows from the ambient torsion-free condition:

$$
II(X,Y)-II(Y,X)=\bigl(D_XY-D_YX-[X,Y]\bigr)^\perp=0,
$$

since the [Lie bracket of vector fields](../../../../../lie-bracket-of-vector-fields.md) tangent to $M$ is tangent. Therefore

$$
\boxed{\langle A_\xi X,Y\rangle=\langle X,A_\xi Y\rangle},
$$

so every normal-direction [shape operator](../../../../../shape-operator.md) is [self-adjoint](../../../../../self-adjoint-operator.md).

The paper uses $R(X,Y)=D_{[X,Y]}-[D_X,D_Y]$, so use the [Gauss equation with reversed curvature convention](../../../../../gauss-equation-with-reversed-curvature-convention.md). Applying the [Gauss formula](../../../../../gauss-formula.md) and [Weingarten formula](../../../../../weingarten-formula.md) twice gives

$$
(D_XD_YZ)^\top=\nabla_X\nabla_YZ-A_{II(Y,Z)}X.
$$

Subtracting in the stated curvature order yields

$$
(R^V(X,Y)Z)^\top=R^M(X,Y)Z+A_{II(Y,Z)}X-A_{II(X,Z)}Y.
$$

Pair with a tangent field $W$ and use the defining relation for the [shape operator in a normal direction](../../../../../shape-operator-in-a-normal-direction.md):

$$
\boxed{\langle R^M(X,Y)Z,W\rangle
=\langle R^V(X,Y)Z,W\rangle
-\langle II(X,W),II(Y,Z)\rangle
+\langle II(Y,W),II(X,Z)\rangle}.
$$

This is the [Gauss equation](../../../../../gauss-equation.md) in the supplied sign convention. If one defines curvature by $[D_X,D_Y]-D_{[X,Y]}$ instead, the two quadratic terms have the opposite signs.

For an [orthonormal frame](../../../../../orthonormal-frame-in-spacetime.md) $X,Y$ on a surface, positive [Gaussian curvature](../../../../../gaussian-curvature.md) with the convention here is $K=\langle R^M(X,Y)X,Y\rangle$. If the ambient space is Euclidean and $\xi$ is a unit normal, the equation becomes

$$
K=\langle II(X,X),II(Y,Y)\rangle-\|II(X,Y)\|^2
=\boxed{\det A_\xi}.
$$

The [Koszul formula](../../../../../koszul-formula.md) determines $\nabla$ from the [induced metric](../../../../../induced-metric.md), and hence determines its [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) and $K$. Therefore the [Gaussian curvature](../../../../../gaussian-curvature.md) depends only on that metric, even though its expression as a product of [principal curvatures](../../../../../principal-curvature.md) appears extrinsic. This is [Theorema Egregium](../../../../../theorema-egregium.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 15](../../paper-15-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
