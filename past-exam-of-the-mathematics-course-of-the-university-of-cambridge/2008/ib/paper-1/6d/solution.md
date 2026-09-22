<h1 id="6d/solution">Solution</h1>

↑ **Parent:** [6D](../6d.md)

A unit lower triangular $L$ is invertible. For $x\ne0$, $y=L^Tx\ne0$, so an [LDL decomposition](../../../../../ldl-decomposition.md) with positive diagonal $D$ gives

$$
x^TAx=(L^Tx)^TD(L^Tx)=\sum_i d_i y_i^2>0.
$$

Also $A=LDL^T$ is symmetric. Hence $A$ is a [positive-definite matrix](../../../../../positive-definite-matrix.md).

For the specified [matrix](../../../../../matrix.md), comparing entries successively gives $d_1=1$, $l_{21}=-1$, $l_{31}=2$, $d_2=3-l_{21}^2d_1=2$, and

$$
l_{32}=\frac{1-l_{31}l_{21}d_1}{d_2}=\frac32,\qquad d_3=3-l_{31}^2d_1-l_{32}^2d_2=-\frac{11}{2}.
$$

Thus

$$
\boxed{L=\begin{pmatrix}1&0&0\\-1&1&0\\2&3/2&1\end{pmatrix},\qquad D=\operatorname{diag}(1,2,-11/2).}
$$

The last pivot is negative, so this particular factorization is outside the positive-diagonal case proved above. Indeed $x=(-2,0,1)^T$ has $x^TAx=-1$, and $\det A=-11$. **There is no positive-diagonal LDL factorization for the printed [matrix](../../../../../matrix.md).** The unrestricted LDL decomposition above is nevertheless valid.

## ↑ Ancestors (10)

1. [6D](../6d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
