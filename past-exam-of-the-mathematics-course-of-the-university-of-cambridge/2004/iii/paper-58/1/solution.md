<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For the [Lie algebra](../../../../../lie-algebra-split.md) $\mathfrak g$ of a [Lie group](../../../../../lie-group.md) $G$, let $\operatorname{ad}_X(Y)=[X,Y]$. The [Killing form](../../../../../killing-form.md) is the symmetric [bilinear form](../../../../../bilinear-form.md)

$$
B(X,Y)=\operatorname{tr}(\operatorname{ad}_X\operatorname{ad}_Y).
$$

For a finite-dimensional real [Lie algebra](../../../../../lie-algebra-split.md), the [Cartan criterion for semisimplicity](../../../../../cartan-criterion-for-semisimplicity.md) says that $B$ is nondegenerate precisely when $\mathfrak g$ is a [semisimple Lie algebra](../../../../../semisimple-lie-algebra-split.md). Thus a [semisimple Lie group](../../../../../semisimple-lie-group.md) supplies the required condition. Compactness alone is insufficient: an abelian [Lie algebra](../../../../../lie-algebra-split.md), including that of a torus, has zero [Killing form](../../../../../killing-form.md).

The [Jacobi identity](../../../../../jacobi-identity.md) gives $\operatorname{ad}_{[Z,X]}=[\operatorname{ad}_Z,\operatorname{ad}_X]$. Cyclic invariance of the [trace](../../../../../matrix-trace.md) therefore gives

$$
B([Z,X],Y)+B(X,[Z,Y])=0.
$$

There is also invariance under the full [Adjoint representation of a Lie group](../../../../../adjoint-representation-of-a-lie-group.md): $\operatorname{ad}_{\operatorname{Ad}_aX}=\operatorname{Ad}_a\operatorname{ad}_X\operatorname{Ad}_{a^{-1}}$, so $B(\operatorname{Ad}_aX,\operatorname{Ad}_aY)=B(X,Y)$.

Define a [pseudo-Riemannian metric](../../../../../pseudo-riemannian-metric.md) by translating $B$ from the identity:

$$
g_a\big((L_a)_*X,(L_a)_*Y\big)=B(X,Y).
$$

It is smooth and nondegenerate. Left translations preserve it by construction. Right translation, expressed in left-translated tangent coordinates, acts by $\operatorname{Ad}_{b^{-1}}$, so it also preserves the metric. This constructs a [bi-invariant pseudo-Riemannian metric](../../../../../bi-invariant-pseudo-riemannian-metric.md).

For [left-invariant vector fields](../../../../../left-invariant-vector-field.md), the derivative terms in the [Koszul formula](../../../../../koszul-formula.md) vanish. Invariance of $B$ then gives

$$
2g(\nabla_XY,Z)=g([X,Y],Z)-g([Y,Z],X)+g([Z,X],Y)=g([X,Y],Z),
\qquad \nabla_XY=\tfrac12[X,Y].
$$

Use the [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) convention $R(X,Y)Z=\nabla_X\nabla_YZ-\nabla_Y\nabla_XZ-\nabla_{[X,Y]}Z$. Substituting the [Levi-Civita connection](../../../../../levi-civita-connection.md) and using the [Jacobi identity](../../../../../jacobi-identity.md) yields

$$
R(X,Y)Z=\tfrac14\big([X,[Y,Z]]-[Y,[X,Z]]\big)-\tfrac12[[X,Y],Z]
=-\tfrac14[[X,Y],Z].
$$

The [Ricci tensor](../../../../../ricci-tensor.md) is the trace of $X\mapsto R(X,Y)Z$. Since $[[X,Y],Z]=\operatorname{ad}_Z\operatorname{ad}_Y X$, it follows that

$$
\boxed{\operatorname{Ric}(Y,Z)=-\tfrac14B(Y,Z)=-\tfrac14g(Y,Z).}
$$

This is the [Killing-form Einstein metric](../../../../../killing-form-einstein-metric.md). Rescaling to $g=cB$, with nonzero constant $c$, gives [Einstein metric](../../../../../einstein-metric.md) constant $-1/(4c)$.

For a compact [semisimple Lie group](../../../../../semisimple-lie-group.md), $B$ is negative definite and $-B$ is a positive-definite [bi-invariant Riemannian metric](../../../../../bi-invariant-riemannian-metric.md). For example, $SU(2)$ has topology $S^3$ and [metric signature](../../../../../metric-signature.md) $(0,3)$ for $B$, while $SO(3)$ has the same [Lie algebra](../../../../../lie-algebra-split.md) and [metric signature](../../../../../metric-signature.md), but topology $\mathbb{RP}^3$. The [special linear group](../../../../../special-linear-group.md) $SL(2,\mathbb R)$ has [metric signature](../../../../../metric-signature.md) $(2,1)$ and topology $S^1\times\mathbb R^2$; its [universal covering Lie group](../../../../../universal-covering-lie-group.md) has topology $\mathbb R^3$ and the same [Killing form](../../../../../killing-form.md). The real [Lie algebra](../../../../../lie-algebra-split.md) of $SL(2,\mathbb C)$ has [metric signature](../../../../../metric-signature.md) $(3,3)$, and the group has topology $S^3\times\mathbb R^3$. Thus the [Killing form](../../../../../killing-form.md) distinguishes compact from noncompact directions in these semisimple examples, but does not determine global topology or distinguish different covering groups.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 58](../../paper-58-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
