<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $D_1=X_1-Y_1$, $D_2=X_2-Y_2$ and

$$
B=\begin{pmatrix}1&0&-1&0\\0&1&0&-1\end{pmatrix}.
$$

The difference vector is $D=BZ$. Its mean is zero because the two sons have the same mean vector. Its [covariance matrix](../../../../../../covariance-matrix.md) is

$$
BVB^T=2\begin{pmatrix}a-c&b-c\\b-c&a-c\end{pmatrix}.
$$

For example, $\operatorname{Cov}(D_1,D_2)=b-c-c+b=2(b-c)$. Thus

$$
\boxed{\begin{pmatrix}D_1\\D_2\end{pmatrix}\sim N_2\!\left(\begin{pmatrix}0\\0\end{pmatrix},\ 2\begin{pmatrix}a-c&b-c\\b-c&a-c\end{pmatrix}\right).}
$$

The [positive definiteness](../../../../../../positive-definiteness.md) assumption supplies $a-b>0$ and $a+b-2c>0$: these are [eigenvalues](../../../../../../eigenvalue.md) of the original [matrix](../../../../../../matrix.md) on within-son contrast and between-son difference directions. In particular the resulting difference [covariance](../../../../../../covariance.md) is positive definite.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
