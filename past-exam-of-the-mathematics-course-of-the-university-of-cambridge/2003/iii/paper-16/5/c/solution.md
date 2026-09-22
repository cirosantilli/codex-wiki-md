<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Consider the [orientation-preserving affine group of the real line](../../../../../../orientation-preserving-affine-group-of-the-real-line.md), realized as

$$
G=\left\{\begin{pmatrix}a&b\\0&1\end{pmatrix}:a>0,\ b\in\mathbb R\right\}.
$$

The coordinates $(\log a,b)$ identify it smoothly with $\mathbb R^2$, so this [Lie group](../../../../../../lie-group.md) is connected. Choose the [Lie algebra](../../../../../../lie-algebra-split.md) element $E$ and the group element $D$:

$$
E=\begin{pmatrix}0&1\\0&0\end{pmatrix},\qquad D=\begin{pmatrix}2&0\\0&1\end{pmatrix}\in G.
$$

Direct [matrix multiplication](../../../../../../matrix-multiplication.md) gives $\operatorname{Ad}_D E=DED^{-1}=2E$.

If a [bi-invariant Riemannian metric](../../../../../../bi-invariant-riemannian-metric.md) existed, every conjugation map $x\mapsto D xD^{-1}$ would be an [isometry](../../../../../../isometry.md) fixing the identity. Its [differential](../../../../../../differential-of-a-smooth-map.md) there, the [Adjoint representation of a Lie group](../../../../../../adjoint-representation-of-a-lie-group.md), would preserve the [positive-definite](../../../../../../positive-definite-bilinear-form.md) [inner product](../../../../../../inner-product.md) at the identity. Thus

$$
\|E\|^2=\|\operatorname{Ad}_D E\|^2=\|2E\|^2=4\|E\|^2,
$$

a contradiction since $E\ne0$. Therefore **this connected Lie group admits no bi-invariant Riemannian metric**. This is the [adjoint dilation obstruction to a bi-invariant Riemannian metric](../../../../../../adjoint-dilation-obstruction-to-a-bi-invariant-riemannian-metric.md), an elementary alternative permitted by the question. The positive definite [Riemannian metric](../../../../../../riemannian-metric.md) interpretation matters; no claim about indefinite metrics is needed.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
