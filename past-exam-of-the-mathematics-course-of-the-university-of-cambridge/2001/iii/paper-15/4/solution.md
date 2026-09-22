<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [Hermitian metric](../../../../../hermitian-metric-on-a-holomorphic-vector-bundle.md) induces pointwise Hermitian inner products on the exterior powers of the complex [cotangent bundle](../../../../../cotangent-bundle.md), with different bidegrees orthogonal, and a positive volume form $dV_g$. Thus the global $L^2$ inner product on smooth [differential forms](../../../../../differential-form-split.md) of type $(p,q)$ is

$$
\langle\alpha,\beta\rangle_{L^2}=\int_M\langle\alpha(x),\beta(x)\rangle_g\,dV_g.
$$

Let $\bar\partial^*$ be the formal adjoint of the [Dolbeault operator](../../../../../dolbeault-operator.md), defined by integration by parts, and let $\Delta_{\bar\partial}=\bar\partial\bar\partial^*+\bar\partial^*\bar\partial$. This [Dolbeault Laplacian](../../../../../dolbeault-laplacian.md) preserves bidegree, is elliptic and nonnegative, and has

$$
\langle\Delta_{\bar\partial}\alpha,\alpha\rangle=\|\bar\partial\alpha\|^2+\|\bar\partial^*\alpha\|^2.
$$

On a compact Hermitian manifold without boundary, the [Dolbeault Hodge decomposition on a compact Hermitian manifold](../../../../../dolbeault-hodge-decomposition-on-a-compact-hermitian-manifold.md) says that the smooth harmonic space $\mathcal H_{\bar\partial}^{p,q}=\ker\Delta_{\bar\partial}$ is finite-dimensional and

$$
A^{p,q}=\mathcal H_{\bar\partial}^{p,q}\mathbin{\oplus^\perp}\Delta_{\bar\partial}A^{p,q}.
$$

More precisely, there are the orthogonal harmonic projection $H$ and a [Dolbeault Green operator](../../../../../dolbeault-green-operator.md) $G$ taking smooth forms to smooth forms, with $G=0$ on harmonics and $\Delta_{\bar\partial}G=G\Delta_{\bar\partial}=I-H$. Elliptic regularity ensures these are statements about smooth forms, not only $L^2$ completions. The Green operator commutes with $\bar\partial$ and $\bar\partial^*$, since the Laplacian does and its inverse is unique on the orthogonal complement of the kernel.

Expanding $\alpha=H\alpha+\Delta_{\bar\partial}G\alpha$ gives

$$
\boxed{A^{p,q}=\mathcal H_{\bar\partial}^{p,q}\oplus\bar\partial A^{p,q-1}\oplus\bar\partial^*A^{p,q+1}.}
$$

The three summands are orthogonal: harmonic forms are killed by both adjoints, and $\langle\bar\partial u,\bar\partial^*v\rangle=\langle\bar\partial^2u,v\rangle=0$. If $\alpha$ is $\bar\partial$-closed, its coexact component is orthogonal to every closed form; taking its inner product with $\alpha$ shows that component has norm zero. Conversely the first two components are closed. Thus **$\boxed{\ker\bar\partial=\mathcal H_{\bar\partial}^{p,q}\oplus\bar\partial A^{p,q-1}}$**, with out-of-range form spaces taken to be zero.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 15](../../paper-15-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
