<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take the [orientation-preserving affine group of the real line](../../../../../../orientation-preserving-affine-group-of-the-real-line.md), written as

$$
G=\left\{\begin{pmatrix}a&b\\0&1\end{pmatrix}:a>0,\ b\in\mathbb R\right\},\qquad
(a,b)(a',b')=(aa',b+ab').
$$

It is a [connected](../../../../../../connected-space.md) [Lie group](../../../../../../lie-group.md), since its underlying manifold is $(0,\infty)\times\mathbb R$. We use the permitted alternative to part (a), a direct obstruction from the [Adjoint representation of a Lie group](../../../../../../adjoint-representation-of-a-lie-group.md).

If a [bi-invariant Riemannian metric](../../../../../../bi-invariant-riemannian-metric.md) existed, conjugation $h\mapsto ghg^{-1}$ would be an [isometry](../../../../../../isometry.md), being a composition of a left and a right translation. Its differential at the identity would preserve the positive [inner product](../../../../../../inner-product.md) on the [Lie algebra](../../../../../../lie-algebra-split.md). Let $T$ be the nonzero infinitesimal translation,

$$
T=\begin{pmatrix}0&1\\0&0\end{pmatrix},\qquad g=\begin{pmatrix}2&0\\0&1\end{pmatrix}.
$$

Direct multiplication gives $\operatorname{Ad}_gT=gTg^{-1}=2T$. Metric invariance would then imply $\|T\|^2=\|2T\|^2=4\|T\|^2$, impossible for a nonzero vector in a positive [inner product](../../../../../../inner-product.md). Therefore **this [connected](../../../../../../connected-space.md) affine Lie [group](../../../../../../group-split.md) has no bi-invariant [Riemannian metric](../../../../../../riemannian-metric.md)**. This is the [adjoint dilation obstruction to a bi-invariant Riemannian metric](../../../../../../adjoint-dilation-obstruction-to-a-bi-invariant-riemannian-metric.md); allowing an indefinite metric would be a different question.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 19](../../../paper-19-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
