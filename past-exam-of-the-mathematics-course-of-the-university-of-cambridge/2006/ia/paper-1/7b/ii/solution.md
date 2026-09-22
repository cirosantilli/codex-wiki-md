<h1 id="7b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A trace-zero [Hermitian matrix](../../../../../../hermitian-operator.md) has the unique form

$$
\begin{pmatrix}h&w\\\overline w&-h\end{pmatrix},
\qquad h\in\mathbb R,\quad w\in\mathbb C.
$$

Set $x_3=h$, $x_1=\operatorname{Re}w$ and $x_2=-\operatorname{Im}w$. Then it is exactly $R(x)$; these assignments also prove uniqueness. This is the real [Pauli matrix](../../../../../../pauli-matrices.md) representation $R(x)=x_1\sigma_1+x_2\sigma_2+x_3\sigma_3$.

For a [unitary matrix](../../../../../../unitary-matrix.md), $U^{-1}=U^\dagger$. Thus

$$
(U^{-1}AU)^\dagger=U^\dagger A^\dagger(U^{-1})^\dagger=U^{-1}AU,
$$

and invariance of the [matrix trace](../../../../../../matrix-trace.md) under [similarity transformations](../../../../../../similarity-transformation.md) gives $\operatorname{tr}(U^{-1}AU)=0$. Therefore conjugation maps the space to itself.

Finally,

$$
\det R(x)=-x_3^2-(x_1-ix_2)(x_1+ix_2)=-|x|^2.
$$

The [determinant](../../../../../../determinant.md) is invariant under [similarity transformations](../../../../../../similarity-transformation.md), so $\det R(y)=\det R(x)$ implies

$$
\boxed{|y|=|x|.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [7B](../../7b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
