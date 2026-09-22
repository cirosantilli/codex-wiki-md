<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An [affine connection](../../../../../../affine-connection.md) on $M$ is an operation $(Y,X)\mapsto\nabla_YX$ on smooth [vector fields](../../../../../../vector-field.md) that is real-bilinear, linear over $C^\infty(M)$ in the differentiating field, and satisfies

$$
\nabla_{hY}X=h\nabla_YX,\qquad
\nabla_Y(hX)=Y(h)X+h\nabla_YX.
$$

It is a [connection on a vector bundle](../../../../../../connection-vector-bundle.md) for the bundle $TM$, also called a linear connection on the manifold. Its [curvature form of a connection](../../../../../../curvature-form.md) has the operator form

$$
\boxed{R(Y,Z)X=\nabla_Y\nabla_ZX-\nabla_Z\nabla_YX-\nabla_{[Y,Z]}X.}
$$

This convention fixes its sign. Expanding the two connection product rules shows that the extra derivatives of a scalar cancel, so $R$ is linear over [smooth functions](../../../../../../smooth-function.md) in all three fields. For a [Levi-Civita connection](../../../../../../levi-civita-connection.md), this is the [Riemann curvature tensor](../../../../../../riemann-curvature-tensor.md).

The [torsion form](../../../../../../torsion-form.md) is $T(Y,Z)=\nabla_YZ-\nabla_ZY-[Y,Z]$. For a [Riemannian metric](../../../../../../riemannian-metric.md) $g$, its [Levi-Civita connection](../../../../../../levi-civita-connection.md) is the unique [torsion-free connection](../../../../../../torsion-free-connection.md) satisfying [metric compatibility](../../../../../../metric-compatibility.md)

$$
Y(g(X,Z))=g(\nabla_YX,Z)+g(X,\nabla_YZ).
$$

Existence and uniqueness follow from the [Koszul formula](../../../../../../koszul-formula.md). In coordinates its coefficients are

$$
\boxed{\Gamma^a{}_{bc}=\tfrac12g^{ad}(\partial_bg_{cd}+\partial_cg_{bd}-\partial_dg_{bc}).}
$$

Symmetry in $b,c$ gives zero torsion, and substitution verifies metric compatibility.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 115](../../../paper-115-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
