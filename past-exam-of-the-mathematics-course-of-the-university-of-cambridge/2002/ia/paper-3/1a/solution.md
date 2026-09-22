<h1 id="1a/solution">Solution</h1>

↑ **Parent:** [1A](../1a.md)

Since $AB=0$, the [image of a linear map](../../../../../image-of-a-linear-map.md) represented by $B$ lies in the [kernel](../../../../../kernel-of-a-linear-map.md) of $A$. The [matrix](../../../../../matrix.md) $B$ is nonzero, so this [image of a linear map](../../../../../image-of-a-linear-map.md) contains a nonzero [vector](../../../../../vector.md); consequently $\dim\ker A\geq1$. On the other hand, $A\neq0$ gives $\operatorname{rank}A\geq1$. The [rank-nullity theorem](../../../../../rank-nullity-theorem.md) in dimension two therefore gives

$$
\dim\ker A=1,\qquad\operatorname{rank}A=1.
$$

Thus **the image of $A$ is a line through the origin**, and $A$ maps onto that line.

Reversing the order of the [matrix multiplication](../../../../../matrix-multiplication.md) need not give zero. For example,

$$
A=\begin{pmatrix}1&0\\0&0\end{pmatrix},\qquad B=\begin{pmatrix}0&0\\1&0\end{pmatrix}
$$

gives $AB=0$ but $BA=B\neq0$. This also shows why information about one composition of [linear maps](../../../../../linear-map.md) does not establish the corresponding property of the reversed composition.

Write $A=\begin{pmatrix}a&b\\c&d\end{pmatrix}$. Its [rank](../../../../../rank-one-quadratic-form.md) is one, so its [determinant](../../../../../determinant.md) is zero. Choose its [adjugate matrix](../../../../../adjugate-matrix.md):

$$
\boxed{C=\begin{pmatrix}d&-b\\-c&a\end{pmatrix}.}
$$

Direct [matrix multiplication](../../../../../matrix-multiplication.md) gives $AC=CA=(ad-bc)I=0$. Since the entries of $C$ are the entries of the nonzero [matrix](../../../../../matrix.md) $A$, rearranged with possible sign changes, $C\neq0$. This establishes both required annihilation properties.

## ↑ Ancestors (10)

1. [1A](../1a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
