<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

An [orthogonal structure on a real vector bundle](../../../../../orthogonal-structure-on-a-real-vector-bundle.md) $E$ of rank $r$ is a choice of local frames whose transition matrices lie in the [orthogonal group](../../../../../orthogonal-group.md) $O(r)$. In such frames declare

$$
h\left(\sum_i a_ie_i,\sum_i b_ie_i\right)=\sum_i a_ib_i.
$$

Orthogonal transitions preserve this expression, so it defines a smooth positive-definite [fiber metric](../../../../../fiber-metric.md). Conversely, a [fiber metric](../../../../../fiber-metric.md) turns any local frame into a smooth orthonormal frame by the [Gram-Schmidt process](../../../../../gram-schmidt-process.md); the resulting transition matrices are orthogonal. The two constructions are inverse, giving the required equivalence.

An [orthogonal local trivialization](../../../../../orthogonal-local-trivialization.md) $E|_U\cong U\times\mathbb R^r$ identifies each fiber isometrically with standard Euclidean space. Equivalently, its coordinate frame satisfies $h(e_i,e_j)=\delta_{ij}$. This is local and does not assert the existence of a global frame.

Every real [vector bundle](../../../../../vector-bundle.md) over a [smooth manifold](../../../../../smooth-manifold.md) admits a [fiber metric](../../../../../fiber-metric.md). Choose a trivializing open cover and local Euclidean metrics $h_i$. The [partition of unity](../../../../../partition-of-unity.md) theorem for a Hausdorff second-countable smooth manifold supplies nonnegative smooth functions $\rho_i$, with locally finite supports contained in the respective cover members, such that $\sum_i\rho_i=1$. Set

$$
h=\sum_i\rho_i h_i,
$$

extending each weighted metric by zero off its chart. Local finiteness makes this smooth. For every nonzero fiber vector $v$, at least one positive weight gives $h(v,v)=\sum_i\rho_i h_i(v,v)>0$. Thus $h$ is a [fiber metric](../../../../../fiber-metric.md) and provides an [orthogonal structure](../../../../../orthogonal-structure-on-a-real-vector-bundle.md).

One definition of an [orthogonal connection](../../../../../metric-connection.md) is that its [covariant derivative](../../../../../covariant-derivative.md) preserves the [fiber metric](../../../../../fiber-metric.md):

$$
X\bigl(h(s,t)\bigr)=h(\nabla_Xs,t)+h(s,\nabla_Xt)
$$

for all [vector fields](../../../../../vector-field.md) $X$ and smooth [sections of a vector bundle](../../../../../section-of-a-vector-bundle.md) $s,t$. Another is that its [parallel transport](../../../../../parallel-transport.md) along every smooth curve is an [isometry](../../../../../isometry.md) between the endpoint fibers.

For the first implication, take parallel sections $s,t$ along a curve. Their covariant derivatives vanish, so the displayed identity makes $h(s,t)$ constant: [parallel transport preserves a fibre metric](../../../../../parallel-transport-preserves-a-fibre-metric.md). Conversely, if parallel transport preserves the [inner product](../../../../../inner-product.md), choose parallel extensions of arbitrary initial fiber vectors along a curve with prescribed initial tangent $X$. Differentiating their constant inner product gives $(\nabla_Xh)(s,t)=0$ at the initial point. Since $X,s,t$ were arbitrary, the connection is [metric-compatible](../../../../../metric-connection.md).

The equivalent local description is that the [connection matrix in an orthonormal frame is skew-symmetric](../../../../../connection-matrix-in-an-orthonormal-frame-is-skew-symmetric.md). Writing $\nabla e_j=\sum_i A^i{}_j e_i$ in an [orthogonal trivialization](../../../../../orthogonal-local-trivialization.md), differentiate $h(e_i,e_j)=\delta_{ij}$ to obtain

$$
\boxed{A^i{}_j+A^j{}_i=0,\qquad A^T=-A}.
$$

Conversely this matrix identity gives the metric-preservation formula by expanding arbitrary sections. It is the [orthogonal group](../../../../../orthogonal-group.md) connection description of the same condition.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 15](../../paper-15-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
