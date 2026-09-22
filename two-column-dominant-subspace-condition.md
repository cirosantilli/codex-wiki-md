# Two-column dominant-subspace condition

↑ **Parent:** [Simultaneous iteration interpretation of the QR algorithm](simultaneous-iteration-interpretation-of-the-qr-algorithm.md)

Let a real [symmetric matrix](symmetric-matrix.md) have an [orthonormal eigenbasis](orthonormal-eigenbasis.md) $w_1,\ldots,w_n$, with

$$
|\lambda_1|\leq\cdots\leq|\lambda_{n-2}|<
|\lambda_{n-1}|=|\lambda_n|.
$$

Write two starting vectors as

$$
u=\sum_i b_iw_i,
\qquad
v=\sum_i c_iw_i.
$$

For two-column [subspace iteration](subspace-iteration.md) to recover  
$\operatorname{span}(w_{n-1},w_n)$, the two projections onto that dominant subspace must be independent. The exact condition is

$$
\det\begin{pmatrix}
b_{n-1}&c_{n-1}\\
b_n&c_n
\end{pmatrix}
=b_{n-1}c_n-b_nc_{n-1}\ne0.
$$

Requiring each of the four coefficients to be nonzero does not imply this determinant condition.

## ↑ Ancestors (8)

1. [Simultaneous iteration interpretation of the QR algorithm](simultaneous-iteration-interpretation-of-the-qr-algorithm.md)
2. [Unshifted QR algorithm](unshifted-qr-algorithm.md)
3. [Numerical linear algebra](numerical-linear-algebra.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1/41e/b/solution.md)
