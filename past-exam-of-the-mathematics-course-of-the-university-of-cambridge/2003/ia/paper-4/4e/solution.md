<h1 id="4e/solution">Solution</h1>

↑ **Parent:** [4E](../4e.md)

About a fixed origin, the total [momentum](../../../../../momentum.md) and [angular momentum](../../../../../angular-momentum.md) are

$$
\mathbf P=\sum_i m_i\mathbf v_i,\qquad \mathbf L=\sum_i\mathbf x_i\times m_i\mathbf v_i.
$$

A time-independent translation $\mathbf x'_i=\mathbf x_i-\mathbf b$ leaves every [velocity](../../../../../velocity.md) unchanged. Therefore

$$
\boxed{\mathbf P'=\mathbf P,\qquad \mathbf L'=\mathbf L-\mathbf b\times\mathbf P}.
$$

The [cross product](../../../../../cross-product.md) $\mathbf b\times\mathbf P$ is perpendicular to $\mathbf P$, giving the invariant

$$
\boxed{\mathbf L'\cdot\mathbf P'=\mathbf L\cdot\mathbf P}.
$$

The other requested transformation follows from the vector triple-product identity:

$$
\boxed{\mathbf L'\times\mathbf P'=\mathbf L\times\mathbf P+|\mathbf P|^2\mathbf b-(\mathbf b\cdot\mathbf P)\mathbf P}.
$$

The actual PDF asks about $\mathbf L\times\mathbf P$; the TeX's occurrence of $\mathbf F$ is a transcription error.

If $\mathbf P=0$, the translation term vanishes and [angular momentum](../../../../../angular-momentum.md) is independent of origin. If $\mathbf P\ne0$, choose

$$
\boxed{\mathbf b=\frac{\mathbf P\times\mathbf L}{|\mathbf P|^2}+\lambda\mathbf P,\qquad \lambda\in\mathbb R}.
$$

Then $\mathbf b\times\mathbf P=\mathbf L-(\mathbf L\cdot\mathbf P)\mathbf P/|\mathbf P|^2$, and so

$$
\mathbf L'=\frac{\mathbf L\cdot\mathbf P}{|\mathbf P|^2}\mathbf P.
$$

Thus the new [angular momentum](../../../../../angular-momentum.md) is parallel to the total [momentum](../../../../../momentum.md). The freedom along $\mathbf P$ gives the [central axis of a momentum system](../../../../../central-axis-of-a-momentum-system.md). If the invariant [dot product](../../../../../dot-product.md) is zero, the new [angular momentum](../../../../../angular-momentum.md) is the zero vector. All expressions assume a translated fixed origin, not a moving reference frame.

## ↑ Ancestors (10)

1. [4E](../4e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
