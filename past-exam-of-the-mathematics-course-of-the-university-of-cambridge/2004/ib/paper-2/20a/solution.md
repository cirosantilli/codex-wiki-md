<h1 id="20a/solution">Solution</h1>

↑ **Parent:** [20A](../20a.md)

Let $r=Ax-b$ and consider an arbitrary variation $x+th$. The objective for the [linear least-squares problem](../../../../../linear-least-squares-problem.md) is

$$
\|A(x+th)-b\|^2=\|r\|^2+2t\,h^TA^Tr+t^2\|Ah\|^2.
$$

At a minimizer the [derivative](../../../../../derivative.md) at $t=0$ must vanish for every $h$, so $A^Tr=0$. Conversely, when this holds, the same expansion at $t=1$ gives $\|A(x+h)-b\|^2=\|r\|^2+\|Ah\|^2\geq\|r\|^2$ for every $h$. Thus **$x$ minimizes the residual norm if and only if $A^T(Ax-b)=0$**. These [least-squares normal equations](../../../../../normal-equations-for-linear-least-squares.md) do not require $A$ to have full rank; without full rank the minimizing vector need not be unique.

The original PDF has $A_{22}=1$, not the 2 in the converted TeX. Using the PDF's [matrix](../../../../../matrix.md) gives

$$
A^TA=\begin{pmatrix}27&6\\6&15\end{pmatrix},\qquad A^Tb=\begin{pmatrix}10\\5\end{pmatrix},\qquad\det(A^TA)=369.
$$

The [least-squares normal equations](../../../../../normal-equations-for-linear-least-squares.md) consequently have the unique solution

$$
\boxed{x=\frac1{123}\begin{pmatrix}40\\25\end{pmatrix}.}
$$

As a direct check, $Ax-b=(-279,-95,238,-61)^T/123$, whose [inner product](../../../../../inner-product.md) with either column of $A$ is zero. The positive [determinant](../../../../../determinant.md) verifies full column rank for this particular problem.

## ↑ Ancestors (10)

1. [20A](../20a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
