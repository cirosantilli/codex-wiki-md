<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Over the [complex numbers](../../../../../../complex-number.md), the [characteristic polynomial](../../../../../../characteristic-polynomial.md) splits into three distinct [roots of a polynomial](../../../../../../root-of-a-polynomial.md), $1,i,-i$. Direct multiplication gives the [eigenvectors](../../../../../../eigenvector.md)

$$
v_1=\begin{pmatrix}0\\0\\1\end{pmatrix},\qquad
v_i=\begin{pmatrix}1\\-i\\0\end{pmatrix},\qquad
v_{-i}=\begin{pmatrix}1\\i\\0\end{pmatrix},
\qquad Av_1=v_1,\quad Av_i=iv_i,\quad Av_{-i}=-iv_{-i}.
$$

They are [linearly independent](../../../../../../linear-independence.md): the last two have two-dimensional [determinant](../../../../../../determinant.md) $2i\ne0$ in the first two coordinates, and the first has nonzero third coordinate. Thus

$$
\boxed{\mathcal B=(v_1,v_i,v_{-i}),\qquad[T']_{\mathcal B}=\operatorname{diag}(1,i,-i).}
$$

This is a [basis](../../../../../../basis.md) of [eigenvectors](../../../../../../eigenvector.md) of $\mathbb C^3$, proving that $T'$ has a [diagonalizable matrix](../../../../../../diagonalizable-matrix.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [Mathematics I](../../../mathematics-i-split.md)
4. [Prelims](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
