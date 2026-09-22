<h1 id="19g/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Take any positive definite [inner product](../../../../../../inner-product.md) $\langle\ ,\ \rangle_0$ on $U$ and define the [inner product adapted to an idempotent linear map](../../../../../../inner-product-adapted-to-an-idempotent-linear-map.md)

$$
\boxed{\langle u,v\rangle_{\phi}=\langle\phi u,\phi v\rangle_0+\langle(I-\phi)u,(I-\phi)v\rangle_0.}
$$

It is symmetric and bilinear. If its quadratic value at $u$ is zero, positive definiteness of the original [inner product](../../../../../../inner-product.md) forces both $\phi u=0$ and $(I-\phi)u=0$, hence $u=0$. Thus it is positive definite.

Using $\phi^2=\phi$ and $(I-\phi)\phi=0$ gives

$$
\langle\phi u,v\rangle_{\phi}=\langle\phi u,\phi v\rangle_0=\langle u,\phi v\rangle_{\phi}.
$$

The map is therefore [self-adjoint](../../../../../../self-adjoint-operator.md) for this new [inner product](../../../../../../inner-product.md) and remains idempotent, so **it is an orthogonal projection for the explicitly constructed inner product**. Geometrically the construction makes its complementary [kernel](../../../../../../kernel-of-a-linear-map.md) and [image](../../../../../../image-of-a-function.md) orthogonal.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [19G](../../19g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
