<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Maurer-Cartan form](../../../../../../maurer-cartan-form.md) is $g^{-1}dg=\lambda^jX_j$. Direct matrix multiplication gives

$$
g^{-1}dg=\begin{pmatrix}d\rho/\rho&dx^1/\rho&dx^2/\rho\\0&0&0\\0&0&0\end{pmatrix},\qquad
\boxed{\lambda^0=\frac{d\rho}{\rho},\quad\lambda^1=\frac{dx^1}{\rho},\quad\lambda^2=\frac{dx^2}{\rho}.}
$$

These are [left-invariant differential forms](../../../../../../left-invariant-differential-form.md): for a constant group element $a$, $(ag)^{-1}d(ag)=g^{-1}dg$. Equivalently, left translation sends $(\rho,x)$ to $(a\rho,b+ax)$, so all three coordinate differentials and the denominator acquire the same factor $a>0$.

The [left-invariant coframe of the translation-dilation group](../../../../../../left-invariant-coframe-of-the-translation-dilation-group.md) is pointwise linearly independent because $\rho>0$. Consequently

$$
h=\sum_{j=0}^2\lambda^j\otimes\lambda^j
$$

is positive definite and unchanged under every left translation. **It therefore defines the required [left-invariant metric](../../../../../../left-invariant-metric.md)**, with precisely the coordinate expression obtained from this sum. The notation $d\rho^2$ in that metric means $d\rho\otimes d\rho$, not the differential of $\rho^2$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 55](../../../paper-55-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
