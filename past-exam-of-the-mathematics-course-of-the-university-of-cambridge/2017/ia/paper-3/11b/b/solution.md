<h1 id="11b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $F=|\mathbf F|>0$ and choose an orientation of a [regular curve](../../../../../../regular-curve.md) following the [vector field](../../../../../../vector-field.md). Its [unit tangent vector](../../../../../../unit-tangent-vector.md) is $t=\sigma\mathbf F/F$, where $\sigma=\pm1$ is constant along a connected regular segment. [Arc length](../../../../../../arc-length.md) differentiation along that [curve](../../../../../../curve.md) is $d/ds=(\sigma\mathbf F/F)\cdot\nabla$. Therefore

$$
\frac{dt}{ds}
=\frac1F(\mathbf F\cdot\nabla)\left(\frac{\mathbf F}{F}\right)
=\frac{(\mathbf F\cdot\nabla)\mathbf F}{F^2}
-\frac{\mathbf F(\mathbf F\cdot\nabla)F}{F^3}.
$$

Taking the [cross product](../../../../../../cross-product.md) with $t$ removes the term parallel to $\mathbf F$:

$$
t\times\frac{dt}{ds}
=\sigma\frac{\mathbf F\times(\mathbf F\cdot\nabla)\mathbf F}{F^3}.
$$

Where the [Frenet frame](../../../../../../frenet-frame.md) exists, $t\times t'=\kappa(t\times n)=\kappa b$. Thus

$$
\boxed{\frac{\mathbf F\times(\mathbf F\cdot\nabla)\mathbf F}{F^3}
=\sigma\kappa b.}
$$

The printed sign corresponds to orientation along or against the field. Taking magnitudes gives the orientation-independent [curvature of an integral curve of a vector field](../../../../../../curvature-of-an-integral-curve-of-a-vector-field.md), $\kappa=|\mathbf F\times(\mathbf F\cdot\nabla)\mathbf F|/F^3$. This [scalar](../../../../../../scalar.md) formula also applies at zero curvature, where $b$ itself may be undefined.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [11B](../../11b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
