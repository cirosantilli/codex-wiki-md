<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Here $\Delta x=1/M$ and periodic indexing is taken modulo $2M$. The [second-order central difference](../../../../../../second-order-central-difference.md) matrix is the real symmetric circulant matrix

$$
A=M^2
\begin{pmatrix}
-2&1&0&\cdots&0&1\\
1&-2&1&\ddots&&0\\
0&1&-2&\ddots&\ddots&\vdots\\
\vdots&\ddots&\ddots&\ddots&1&0\\
0&&\ddots&1&-2&1\\
1&0&\cdots&0&1&-2
\end{pmatrix}.
$$

Since $V$ is real diagonal, $H=A-V$ is [Hermitian](../../../../../../hermitian-operator.md). Therefore $iH$ is [skew-Hermitian](../../../../../../skew-hermitian-matrix.md), and

$$
\boxed{\frac d{dt}\|\mathbf u\|_2^2
=\mathbf u^*(iH)\mathbf u+
\mathbf u^*(-iH)\mathbf u=0.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
