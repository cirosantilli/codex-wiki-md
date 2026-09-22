<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Kähler form](../../../../../../kahler-form.md) and the [Hermitian metric](../../../../../../hermitian-metric-on-a-holomorphic-vector-bundle.md) give the $L^2$ inner product on [vector-bundle-valued differential forms](../../../../../../vector-bundle-valued-differential-form.md), using volume $\omega^n/n!$. Define the [formal adjoint](../../../../../../formal-adjoint.md) $\bar\partial_E^*$ and the elliptic, self-adjoint, nonnegative [Dolbeault Laplacian](../../../../../../dolbeault-laplacian.md)

$$
\Delta''_E=\bar\partial_E\bar\partial_E^*+\bar\partial_E^*\bar\partial_E.
$$

Its harmonic space is

$$
\mathcal H^{p,q}(X,E)=\ker\Delta''_E
=\ker\bar\partial_E\cap\ker\bar\partial_E^*.
$$

The equality follows from $\langle\Delta''_E\alpha,\alpha\rangle=\|\bar\partial_E\alpha\|^2+\|\bar\partial_E^*\alpha\|^2$. On compact $X$, the bundle-valued [Dolbeault Hodge decomposition](../../../../../../dolbeault-hodge-decomposition-on-a-compact-hermitian-manifold.md) states that this space is finite dimensional and that

$$
\boxed{\mathcal A^{p,q}(X,E)=\mathcal H^{p,q}(X,E)
\oplus\bar\partial_E\mathcal A^{p,q-1}(X,E)
\oplus\bar\partial_E^*\mathcal A^{p,q+1}(X,E).}
$$

The sum is orthogonal for the $L^2$ inner product and all summands here consist of smooth forms. Every [Dolbeault cohomology](../../../../../../dolbeault-cohomology.md) class has a unique harmonic representative, giving $H^{p,q}_{\bar\partial}(X,E)\cong\mathcal H^{p,q}(X,E)$ and, by the [Dolbeault theorem](../../../../../../dolbeault-theorem.md), the corresponding [sheaf cohomology](../../../../../../sheaf-cohomology.md) isomorphism. This is a decomposition for $\bar\partial_E$, whose square is zero; it does not require the full [Chern connection](../../../../../../chern-connection.md) to be flat.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
