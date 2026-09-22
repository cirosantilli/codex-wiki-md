<h1 id="6a/solution">Solution</h1>

↑ **Parent:** [6A](../6a.md)

For two [upper triangular matrices](../../../../../upper-triangular-matrix.md) and $i>j$,

$$
(AB)_{ij}=\sum_{k=1}^3A_{ik}B_{kj}=0.
$$

Indeed a potentially nonzero factor $A_{ik}$ requires $k\geq i$, while a potentially nonzero $B_{kj}$ requires $k\leq j$. These requirements cannot both hold when $i>j$. Thus their [matrix product](../../../../../matrix-product.md) is upper triangular.

Direct [matrix multiplication](../../../../../matrix-multiplication.md) for the given $A$ gives

$$
A^2=\begin{pmatrix}1&0&2\\0&1&-2\\0&0&1\end{pmatrix},\qquad
A^3=\begin{pmatrix}1&2&-2\\0&-1&3\\0&0&-1\end{pmatrix}.
$$

Adding $A^3+A^2-A$ yields $I$, so $A(A^2+A-I)=(A^2+A-I)A=I$. Hence

$$
\boxed{A^{-1}=A^2+A-I=\begin{pmatrix}1&2&2\\0&-1&-1\\0&0&-1\end{pmatrix}.}
$$

Every nonnegative [matrix power](../../../../../matrix-power.md) is in $\operatorname{span}\{I,A,A^2\}$: reduce powers of degree at least three using $A^3=-A^2+A+I$. More formally, repeated reduction shows that products of any two polynomials of degree at most two in $A$ again lie in this span. Since $A^{-1}$ also lies in it, positive powers of $A^{-1}$ prove the same assertion for all negative integers. This is an instance of the [integer powers for an annihilating polynomial with roots one and minus one](../../../../../integer-powers-for-an-annihilating-polynomial-with-roots-one-and-minus-one.md), because $A^3+A^2-A-I=(A-I)(A+I)^2=0$.

To find the required entries for every integer, use the block upper-triangular structure. The top-left entry of $A^n$ is $1$ for positive and negative powers. Its lower-right block is

$$
J=-I_2+N=-(I_2-N),\qquad
N=\begin{pmatrix}0&1\\0&0\end{pmatrix},\qquad N^2=0.
$$

The identity $(I_2-N)^n=I_2-nN$ holds for all integers: multiplication adds the coefficients of $N$, and $(I_2-N)^{-1}=I_2+N$ proves the negative cases. Therefore

$$
\boxed{(A^n)_{11}=1,\quad(A^n)_{22}=(-1)^n,\quad(A^n)_{23}=n(-1)^{n-1}.}
$$

Write $s=(-1)^n$ and $A^n=\alpha_nA^2+\beta_nA+\gamma_nI$. Comparing those three entries gives

$$
\alpha_n+\beta_n+\gamma_n=1,\qquad
\alpha_n-\beta_n+\gamma_n=s,\qquad
-2\alpha_n+\beta_n=-ns.
$$

Subtracting the first two equations finds $\beta_n$; the third then finds $\alpha_n$, and the first finds $\gamma_n$. The unique solution is

$$
\boxed{\alpha_n=\frac{1-s}{4}+\frac{ns}{2},\quad
\beta_n=\frac{1-s}{2},\quad
\gamma_n=\frac{1+3s}{4}-\frac{ns}{2},\qquad s=(-1)^n.}
$$

For clarity, substituting also gives the full [matrix power](../../../../../matrix-power.md)

$$
\boxed{A^n=\begin{pmatrix}
1&1-s&(1-s)/2+ns\\0&s&-ns\\0&0&s
\end{pmatrix}\quad(n\in\mathbb Z).}
$$

## ↑ Ancestors (10)

1. [6A](../6a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
