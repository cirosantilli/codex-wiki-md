<h1 id="5b/solution">Solution</h1>

↑ **Parent:** [5B](../5b.md)

Apply symmetric [Gaussian elimination](../../../../../gaussian-elimination.md) without row exchanges. At step $k$, let $d_k$ be the leading diagonal entry of the remaining symmetric [Schur complement](../../../../../schur-complement.md). If $d_k\leq0$, stop and report that $A$ is not [positive definite](../../../../../positive-definite-matrix.md). If $d_k>0$, use it to eliminate the rest of its row and column. If all steps succeed, this constructs an [LDL decomposition](../../../../../ldl-decomposition.md)

$$
A=LDL^T,
$$

where $L$ is unit lower triangular and $D=\operatorname{diag}(d_1,\ldots,d_n)$ has positive diagonal.

The test is correct from first principles. If all $d_k>0$, then for every nonzero $x$,

$$
x^TAx=(L^Tx)^TD(L^Tx)>0
$$

because $L$ is invertible. Conversely, if $A$ is positive definite, its first pivot is $a_{11}>0$, and completing the square gives

$$
\begin{pmatrix}s\\y\end{pmatrix}^{T}
\begin{pmatrix}a&b^T\\b&C\end{pmatrix}
\begin{pmatrix}s\\y\end{pmatrix}
=a\left(s+\frac{b^Ty}{a}\right)^2
+y^T\left(C-\frac{bb^T}{a}\right)y.
$$

Choosing $s=-b^Ty/a$ shows that the Schur complement is positive definite. Induction forces every pivot to be positive. This is also [Sylvester's criterion](../../../../../sylvester-s-criterion.md).

At step $k$, updating the remaining matrix costs $O((n-k)^2)$ arithmetic operations. Hence the total is

$$
\sum_{k=1}^nO((n-k)^2)=O(n^3),
$$

which proves the existence of the required algorithm.

## ↑ Ancestors (10)

1. [5B](../5b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
