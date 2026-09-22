# Ellipsoid level sets of a positive-definite quadratic form

↑ **Parent:** [Positive definiteness](positive-definiteness.md)

For a real [positive-definite matrix](positive-definite-matrix.md) $A$ in finite [dimension](dimension-vector-space.md), write $A=Q\Lambda Q^T$ by the [spectral theorem for real symmetric matrices](spectral-theorem-for-real-symmetric-matrices.md). In the [coordinates](coordinate-linear-algebra.md) in an [orthonormal basis](orthonormal-basis.md) $w=Q^Tx$, the positive [level set](level-set.md) $q(x)=k$ becomes

$$
\sum_{j=1}^n\lambda_jw_j^2=k,\qquad \sum_{j=1}^n\frac{w_j^2}{k/\lambda_j}=1.
$$

This is an [ellipsoid](ellipsoid.md), with [semi-major and semi-minor axes](semi-major-and-semi-minor-axes.md) in two [dimensions](dimension-vector-space.md) forming an [ellipse](ellipse.md); each semi-axis has length $r_j=\sqrt{k/\lambda_j}$ and direction given by the corresponding [eigenvector](eigenvector.md). In the opening example, the shorter semi-axis is $\sqrt{k}/2$ along $e_+$, while the longer is $\sqrt{k/2}$ along $e_-$. A stiffer direction, meaning a larger [eigenvalue](eigenvalue.md), reaches the same energy at a smaller displacement. The ratio of longest to shortest semi-axis is $\sqrt{\lambda_{\max}/\lambda_{\min}}$, the square root of the [spectral condition number of a positive-definite matrix](spectral-condition-number-of-a-positive-definite-matrix.md).[§2.2.2, p. 30, equation (2.3): ellipsoids and semi-axis lengths; the book uses the inverse quadratic coefficient matrix](convex-optimization-by-stephen-boyd-and-lieven-vandenberghe.md)

Strict positivity matters because $\lambda_{\min}>0$ gives

$$
\lambda_{\min}\|x\|^2\leq q(x)\leq\lambda_{\max}\|x\|^2.
$$

Hence a fixed positive [level set](level-set.md) cannot extend arbitrarily far. The [Cholesky decomposition](cholesky-decomposition.md) $A=LL^T$ gives another view: $q(x)=\|L^Tx\|^2$, so the [ellipsoid](ellipsoid.md) is the inverse image of a [sphere](sphere.md) under an [invertible linear map](invertible-linear-map.md). A singular [positive semidefinite matrix](positive-semidefinite-matrix.md) has a nonzero [kernel](kernel-of-a-linear-map.md); adding a [kernel](kernel-of-a-linear-map.md) [vector](vector.md) preserves its [quadratic form](quadratic-form.md), so any nonempty positive [level set](level-set.md) is unbounded. These statements concern finite [dimension](dimension-vector-space.md); the [positive definite symmetric operator](positive-definite-symmetric-operator.md) entry explains why strict positivity alone need not give a uniform lower bound on an infinite-dimensional [Hilbert space](hilbert-space-split.md).

## ↑ Ancestors (9)

1. [Positive definiteness](positive-definiteness.md)
2. [Positive-definite bilinear form](positive-definite-bilinear-form.md)
3. [Symmetric bilinear form](symmetric-bilinear-form.md)
4. [Bilinear form](bilinear-form.md)
5. [Linear algebra](linear-algebra-split.md)
6. [Algebra](algebra-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)
