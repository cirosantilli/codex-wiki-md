<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $a$ be an arbitrary constant [vector](../../../../../../vector.md). By the cyclic identity for the [scalar triple product](../../../../../../scalar-triple-product.md),

$$
a\cdot\oint_{\partial\Sigma}d\mathbf r\times\mathbf F
=\oint_{\partial\Sigma}(\mathbf F\times a)\cdot d\mathbf r.
$$

Apply [Stokes theorem](../../../../../../stokes-theorem.md) to $\mathbf F\times a$. Since $a$ is constant, the [curl](../../../../../../curl.md) product identity gives

$$
\nabla\times(\mathbf F\times a)
=(a\cdot\nabla)\mathbf F-a(\nabla\cdot\mathbf F).
$$

Consequently

$$
\begin{aligned}
a\cdot\oint_{\partial\Sigma}d\mathbf r\times\mathbf F
&=\iint_\Sigma\left[\mathbf n\cdot(a\cdot\nabla)\mathbf F
-(\mathbf n\cdot a)(\nabla\cdot\mathbf F)\right]dS\\
&=a\cdot\iint_\Sigma(\mathbf n\times\nabla)\times\mathbf F\,dS.
\end{aligned}
$$

For precision, the operator in the last line has components

$$
\bigl[(\mathbf n\times\nabla)\times\mathbf F\bigr]_i
=\sum_{j=1}^3n_j\partial_iF_j-n_i\sum_{j=1}^3\partial_jF_j.
$$

The [partial derivatives](../../../../../../partial-derivative.md) act on $\mathbf F$, with $\mathbf n$ multiplying their values; they do not differentiate $\mathbf n$. Since the [dot products](../../../../../../dot-product.md) agree for every constant $a$, the [cross-product form of Stokes theorem](../../../../../../cross-product-form-of-stokes-theorem.md) follows:

$$
\boxed{\oint_{\partial\Sigma}d\mathbf r\times\mathbf F
=\iint_\Sigma(\mathbf n\times\nabla)\times\mathbf F\,dS.}
$$

Here $\wedge$ in the paper denotes the [cross product](../../../../../../cross-product.md), and the printed surface integral has its [area element](../../../../../../area-element-of-a-surface.md) $dS$ understood.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [Mathematics V](../../../mathematics-v-split.md)
4. [Prelims](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
