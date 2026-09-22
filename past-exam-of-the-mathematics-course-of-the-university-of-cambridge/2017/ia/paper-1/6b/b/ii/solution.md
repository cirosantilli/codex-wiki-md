<h1 id="6b/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Multiplication gives

$$
B^TB=(I+nm^T)(I+mn^T)=I+mn^T+nm^T+nn^T.
$$

The vector $p=m\times n$ is an eigenvector with eigenvalue one. On the plane spanned by the orthonormal pair $m,n$, the matrix is

$$
\begin{pmatrix}1&1\\1&2\end{pmatrix}.
$$

Its eigenvalues are the roots of $\mu^2-3\mu+1$, namely

$$
\mu_\pm=\frac{3\pm\sqrt5}{2}.
$$

For either root, an eigenvector is $m+(\mu_\pm-1)n$. Therefore

$$
\boxed{
\begin{array}{c|c}
\text{eigenvector}&\text{eigenvalue}\\ \hline
m\times n&1\\
m+\frac{1+\sqrt5}{2}n&\frac{3+\sqrt5}{2}\\
m+\frac{1-\sqrt5}{2}n&\frac{3-\sqrt5}{2}
\end{array}}
$$

These positive eigenvalues are the squared [singular values](../../../../../../../singular-value.md) of $B$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [6B](../../../6b.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ia](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
