<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $B(X,Y)=\operatorname{tr}(\operatorname{ad}X\operatorname{ad}Y)$ be the [Killing form](../../../../../../killing-form.md). A real [semisimple Lie algebra](../../../../../../semisimple-lie-algebra-split.md) has nondegenerate $B$, and its invariance gives $B([X,Y],Z)=B(X,[Y,Z])$. Translating $B$ defines a [bi-invariant pseudo-Riemannian metric](../../../../../../bi-invariant-pseudo-riemannian-metric.md) $g=B$ on the [Lie group](../../../../../../lie-group.md).

For [left-invariant vector fields](../../../../../../left-invariant-vector-field.md), all derivatives of their pairwise inner products vanish. The [Koszul formula](../../../../../../koszul-formula.md) reduces to

$$
2B(\nabla_XY,Z)=B([X,Y],Z)-B([Y,Z],X)+B([Z,X],Y)=B([X,Y],Z).
$$

Nondegeneracy gives $\nabla_XY=[X,Y]/2$. With $R(X,Y)Z=\nabla_X\nabla_YZ-\nabla_Y\nabla_XZ-\nabla_{[X,Y]}Z$, the [Jacobi identity](../../../../../../jacobi-identity.md) now gives

$$
R(X,Y)Z=-\tfrac14[[X,Y],Z].
$$

Taking the trace of $X\mapsto R(X,Y)Z=-\tfrac14\operatorname{ad}Z\operatorname{ad}Y(X)$ yields the [Ricci tensor](../../../../../../ricci-tensor.md)

$$
\boxed{\operatorname{Ric}(Y,Z)=-\tfrac14 B(Y,Z)=-\tfrac14 g(Y,Z).}
$$

Thus the [Killing-form Einstein metric](../../../../../../killing-form-einstein-metric.md) makes the group an [Einstein manifold](../../../../../../einstein-manifold.md), allowing an indefinite metric. Its [scalar curvature](../../../../../../scalar-curvature.md) in this convention is $-\dim G/4$.

For a connected compact [semisimple Lie group](../../../../../../semisimple-lie-group.md), $B$ is negative definite: the adjoint operators are skew-adjoint for an invariant positive inner product, so $B(X,X)=\operatorname{tr}((\operatorname{ad}X)^2)<0$ for $X\ne0$. The conventional positive [Riemannian metric](../../../../../../riemannian-metric.md) is instead $g_+=-B$. Its [Ricci tensor](../../../../../../ricci-tensor.md) is $g_+/4$, and its [sectional curvature](../../../../../../sectional-curvature.md) is

$$
K_{g_+}(X,Y)=\frac{\|[X,Y]\|_{g_+}^2}{4(\|X\|_{g_+}^2\|Y\|_{g_+}^2-\langle X,Y\rangle_{g_+}^2)}\geq0.
$$

It can vanish on commuting two-planes; positivity is not automatic in every direction. With the literal negative metric $B$, the corresponding sectional-curvature signs are reversed.

For a noncompact real semisimple group, a Cartan decomposition $\mathfrak g=\mathfrak k\oplus\mathfrak p$ has $B$ negative on $\mathfrak k$ and positive on $\mathfrak p$. The [Killing metric](../../../../../../killing-form-einstein-metric.md) is indefinite and cannot be made positive by an overall sign. Its Einstein constant remains $-1/4$ for $g=B$, but that does not assert a uniform sign for sectional curvature of all nondegenerate planes. For connected semisimple groups, negative-definite $B$ characterizes the compact case. Disconnected groups require a separate condition on the number of components before compactness follows.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
