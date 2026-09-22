# Weighted Euclidean inner product

↑ **Parent:** [Weighted inner product](weighted-inner-product.md)

A [symmetric positive-definite matrix](symmetric-positive-definite-matrix.md) $M$ defines an [inner product](inner-product.md) on real coordinate [vectors](vector.md) by

$$
\langle u,v\rangle_M=u^TMv,\qquad \|u\|_M^2=u^TMu.
$$

For diagonal $M$, positive diagonal entries weight the squared coordinate errors. This is the finite-coordinate version of a [weighted inner product](weighted-inner-product.md); the positive-definite matrix example appears in [Francis Narcowich, Inner Products and Norms, standard inner products, example 8](https://people.tamu.edu/~f-narcowich/m641/m641_notes/inner_products.html).

For $M=\operatorname{diag}(4,1)$, the squared [norm](norm.md) of $(a,b)^T$ is $4a^2+b^2$. A first-coordinate error of one costs as much as a second-coordinate error of two. The [unit sphere](unit-sphere.md) is the [ellipse](ellipse.md) $4a^2+b^2=1$, and [orthogonality](orthogonal-vectors.md) means $4u_1v_1+u_2v_2=0$. Thus “closest” and “perpendicular” depend on the chosen [inner product](inner-product.md). The [orthogonal projection residual](orthogonal-projection-residual.md) example shows how this changes a best approximation.

## ↑ Ancestors (7)

1. [Weighted inner product](weighted-inner-product.md)
2. [Inner product](inner-product.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Orthogonal projection matrix](orthogonal-projection-matrix.md)
- [Orthogonal projection residual](orthogonal-projection-residual.md)
- [Weighted inner product](weighted-inner-product.md)
