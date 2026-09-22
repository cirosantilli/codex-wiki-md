<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $\overline{\mathbf y}=(\mathbf y_n+\mathbf y_{n+1})/2$. The [implicit midpoint rule](../../../../../../implicit-midpoint-rule.md) reads

$$
\mathbf y_{n+1}-\mathbf y_n
=hA(\overline{\mathbf y})\overline{\mathbf y}.
$$

Taking the [inner product](../../../../../../inner-product.md) with $\mathbf y_{n+1}+\mathbf y_n=2\overline{\mathbf y}$ gives

$$
\begin{aligned}
\|\mathbf y_{n+1}\|_2^2-\|\mathbf y_n\|_2^2
&=(\mathbf y_{n+1}+\mathbf y_n)^T(\mathbf y_{n+1}-\mathbf y_n)\\
&=2h\overline{\mathbf y}^{T}A(\overline{\mathbf y})\overline{\mathbf y}=0.
\end{aligned}
$$

The last equality again follows from [skew-symmetry](../../../../../../skew-symmetric-matrix.md). [Mathematical induction](../../../../../../mathematical-induction.md) therefore yields

$$
\boxed{\|\mathbf y_n\|_2=\|\mathbf y_0\|_2\quad(n\in\mathbb Z_+).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
