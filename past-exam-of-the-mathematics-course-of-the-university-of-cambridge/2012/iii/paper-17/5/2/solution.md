<h1 id="5/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [Levi-Civita connection](../../../../../../levi-civita-connection.md) is the unique [connection on a vector bundle](../../../../../../connection-vector-bundle.md) $TM$ that is [torsion-free](../../../../../../torsion-free-connection.md) and [metric-compatible](../../../../../../metric-connection.md). These conditions are

$$
\nabla_XY-\nabla_YX=[X,Y],
\qquad
X(g(Y,Z))=g(\nabla_XY,Z)+g(Y,\nabla_XZ).
$$

Existence and uniqueness follow from the [Koszul formula](../../../../../../koszul-formula.md); equivalently, these are the defining properties that characterize the connection.

Define the correction tensor

$$
A(X,Y)=X(\sigma)Y+Y(\sigma)X-g(X,Y)V_\sigma
$$

and set $D_XY=\nabla_XY+A(X,Y)$. All terms of $A$ are $C^\infty(M)$-linear in both $X$ and $Y$, so $D$ is a connection. The symmetry $A(X,Y)=A(Y,X)$ preserves vanishing of the [torsion tensor](../../../../../../torsion-tensor.md).

To check compatibility with $\widetilde g$, compute

$$
X(\widetilde g(Y,Z))
=e^{2\sigma}\bigl(2X(\sigma)g(Y,Z)+g(\nabla_XY,Z)+g(Y,\nabla_XZ)\bigr).
$$

On the other hand,

$$
\begin{aligned}
g(A(X,Y),Z)
&=X(\sigma)g(Y,Z)+Y(\sigma)g(X,Z)-g(X,Y)Z(\sigma),\\
g(Y,A(X,Z))
&=X(\sigma)g(Y,Z)+Z(\sigma)g(X,Y)-g(X,Z)Y(\sigma).
\end{aligned}
$$

The cross terms cancel, so their sum is $2X(\sigma)g(Y,Z)$. Multiplying by $e^{2\sigma}$ proves $X(\widetilde g(Y,Z))=\widetilde g(D_XY,Z)+\widetilde g(Y,D_XZ)$. Hence $D$ is torsion-free and compatible with $\widetilde g$, so uniqueness of the [Levi-Civita connection](../../../../../../levi-civita-connection.md) gives

$$
\boxed{\widetilde\nabla_XY
=\nabla_XY+X(\sigma)Y+Y(\sigma)X-g(X,Y)\operatorname{grad}_g\sigma.}
$$

This is the [Levi-Civita connection under conformal rescaling](../../../../../../levi-civita-connection-under-conformal-rescaling.md).

On a nonempty compact manifold without boundary, $\sigma$ attains a maximum at some $p$. The derivative of a smooth function vanishes at an interior extremum, so $(d\sigma)_p=0$ and $(V_\sigma)_p=0$. The correction tensor therefore vanishes at $p$, giving

$$
\boxed{(\widetilde\nabla_XY)_p=(\nabla_XY)_p\quad\text{for every }X,Y.}
$$

This is equality for all vector fields at the same point, not an assertion that either connection vanishes there. More generally, the two connections agree at any [critical point](../../../../../../critical-point.md) of $\sigma$. Conversely, if their correction vanishes for all $X,Y$ at a point of positive dimension, evaluating $g(A(v,v),v)=g(v,v)d\sigma(v)$ for every $v$ shows that the point is critical. This is the [critical-point criterion for equal conformal connections](../../../../../../critical-point-criterion-for-equal-conformal-connections.md).

The boundaryless hypothesis is the usual convention for “manifold” here. If manifolds with boundary were included, compactness alone would not suffice: on $[0,1]$ with $g=dx^2$ and $\sigma=x$, one has $\widetilde\nabla_{\partial_x}\partial_x=\partial_x$ everywhere while $\nabla_{\partial_x}\partial_x=0$. An extremum at the boundary need not be a critical point.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [5](../../5.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
