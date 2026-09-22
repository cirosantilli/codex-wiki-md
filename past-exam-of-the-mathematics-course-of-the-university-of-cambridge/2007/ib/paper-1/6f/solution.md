<h1 id="6f/solution">Solution</h1>

↑ **Parent:** [6F](../6f.md)

The first [matrix](../../../../../matrix.md) column is already the unit vector $e_1$, so the first QR elimination needs no reflection. In the remaining three coordinates, the second column is $v=(2,2,1)^T$, with norm three. To map it to $(-3,0,0)^T$, use the [Householder transformation](../../../../../householder-transformation.md)

$$
w=v+3e_1=(5,2,1)^T,\qquad H=I-\frac{2ww^T}{w^Tw}=I-\frac{ww^T}{15}.
$$

It is symmetric and orthogonal and satisfies $Hv=(-3,0,0)^T$. Extend it to $Q^T=\operatorname{diag}(1,H)$. The [QR decomposition](../../../../../qr-decomposition.md) and transformed right side are

$$
Q^TA=\begin{pmatrix}1&3\\0&-3\\0&0\\0&0\end{pmatrix},\qquad
Q^Tb=\begin{pmatrix}4\\-3\\12/5\\-9/5\end{pmatrix}.
$$

For the lower right-side block, $w^T(1,4,-1)^T=12$, so its transformed value is $(1,4,-1)^T-(12/15)w=(-3,12/5,-9/5)^T$.

Orthogonality preserves the least-squares residual norm. Thus the first two squared residual terms can and must be set to zero, while the last two are independent of the unknowns:

$$
x_1+3x_2=4,\quad -3x_2=-3,
\qquad\boxed{x_1=x_2=1.}
$$

The minimum squared residual is $(12/5)^2+(-9/5)^2=9$. The solution is unique since the triangular factor has nonzero diagonal entries. No normal equations are used.

## ↑ Ancestors (10)

1. [6F](../6f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
