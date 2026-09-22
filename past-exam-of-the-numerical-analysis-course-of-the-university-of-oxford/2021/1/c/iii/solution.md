<h1 id="1/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Set $W=\operatorname{diag}(w_0,\ldots,w_n)$. For column indices $j,k\in\{1,\ldots,n+1\}$, the product $P_{j-1}P_{k-1}$ has [polynomial degree](../../../../../degree-of-a-polynomial.md) at most $2n$, so exactness of [Gauss-Legendre quadrature](../../../../../gauss-legendre-quadrature.md) and [orthonormality](../../../../../orthonormal-set.md) give

$$
(A^TWA)_{jk}=\sum_{i=0}^nw_iP_{j-1}(x_i)P_{k-1}(x_i)
=\int_{-1}^1P_{j-1}(x)P_{k-1}(x)\,dx=\delta_{jk}.
$$

Thus $Q=W^{1/2}A$ is a square [matrix](../../../../../matrix.md) with $Q^TQ=I$, and therefore is an [orthogonal matrix](../../../../../orthogonal-matrix.md): $QQ^T=I$ as well. It follows that

$$
\boxed{AA^T=W^{-1},\qquad
(AA^T)_{ij}=\begin{cases}
w_{i-1}^{-1},&i=j,\\
0,&i\ne j.
\end{cases}}
$$

Equivalently, the rows of the [generalized Vandermonde matrix](../../../../../generalized-vandermonde-matrix.md) are [orthogonal](../../../../../orthogonal-vectors.md) and

$$
\sum_{k=0}^nP_k(x_i)^2=\frac1{w_i}.
$$

The normalization matters: here $P_{n+1}=\sqrt{(2n+3)/2}\,L_{n+1}$, where $L_{n+1}$ is the conventional [Legendre polynomial](../../../../../legendre-polynomial.md) used above. Thus a formula containing only the nodes and the question's [orthonormal](../../../../../orthonormal-set.md) [polynomials](../../../../../polynomial-split.md) is

$$
\boxed{(AA^T)_{ij}=\delta_{ij}
\frac{(1-x_{i-1}^2)[P_{n+1}'(x_{i-1})]^2}{2n+3}.}
$$

This identity is the [discrete orthogonality of Gaussian quadrature](../../../../../discrete-orthogonality-of-gaussian-quadrature.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the numerical analysis course of the University of Oxford](../../../../split.md)
6. [Numerical analysis course of the University of Oxford](../../../../../numerical-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
