<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $\overline{\mathbf r}=a^2\mathbf r/r^2$ and $\widehat{\mathbf r}=\mathbf r/r$. Its Jacobian is

$$
\frac{\partial\overline r_i}{\partial r_j}
=\frac{a^2}{r^2}(\delta_{ij}-2\widehat r_i\widehat r_j).
$$

The [chain rule](../../../../../chain-rule.md) therefore yields

$$
\nabla_{\mathbf r}
=\frac{a^2}{r^2}
\left[\nabla_{\overline{\mathbf r}}
-2\widehat{\mathbf r}(\widehat{\mathbf r}\cdot\nabla_{\overline{\mathbf r}})\right].
$$

Taking its [cross product](../../../../../cross-product.md) with $\mathbf r$ kills the radial term and proves that [spherical inversion preserves angular derivatives](../../../../../spherical-inversion-preserves-angular-derivatives.md):

$$
\boxed{\mathbf r\times\nabla_{\mathbf r}
=\frac{a^2}{r^2}\mathbf r\times\nabla_{\overline{\mathbf r}}
=\overline{\mathbf r}\times\nabla_{\overline{\mathbf r}}.}
$$

This is also the invariance of the differential expression underlying the [angular momentum operator](../../../../../angular-momentum-operator.md).

A scalar [spherical harmonic](../../../../../spherical-harmonic.md) $Y$ depends only on direction, so $Y(\widehat{\mathbf r})=Y(\widehat{\overline{\mathbf r}})$ and its gradient is tangential. Thus $\widehat{\mathbf r}\cdot\nabla_{\overline{\mathbf r}}Y=0$, and

$$
r\nabla_{\mathbf r}Y=\overline r\nabla_{\overline{\mathbf r}}Y,
\qquad \widehat{\mathbf r}=\widehat{\overline{\mathbf r}}.
$$

Each of the three normalized [vector spherical harmonic](../../../../../vector-spherical-harmonic.md) families is consequently unchanged as an angular basis function:

$$
\boxed{\mathbf P(\overline{\mathbf r})=\mathbf P(\mathbf r),
\qquad \mathbf B(\overline{\mathbf r})=\mathbf B(\mathbf r),
\qquad \mathbf C(\overline{\mathbf r})=\mathbf C(\mathbf r).}
$$

The normalization requires $n\geq1$ for $\mathbf B$ and $\mathbf C$; at $n=0$ the gradient vanishes and only $\mathbf P$ remains.

This substitution into the basis functions is distinct from the [pushforward of a vector field](../../../../../pushforward-of-a-vector-field.md) of a physical vector field by inversion. Under that Jacobian map the radial vector picks up $-a^2/r^2$ and the two tangential vectors pick up $+a^2/r^2$. Likewise, the weighted [Kelvin transform](../../../../../kelvin-transform.md) of a scalar includes the extra factor $a/r$. Neither operation changes the angular differential identity just proved.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 76](../../paper-76-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
