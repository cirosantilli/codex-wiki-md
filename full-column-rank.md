# Full column rank

↑ **Parent:** [Matrix rank](matrix-rank.md)

An $m\times n$ [matrix](matrix.md) has [full column rank](full-column-rank.md) when its [matrix rank](matrix-rank.md) is $n$, equivalently when its columns are [linearly independent vectors](linear-independence.md). This requires $n\leq m$. Its [kernel](kernel-of-a-linear-map-split.md) is $\{0\}$, so the represented [linear map](linear-map.md) is [injective](injective-function.md) and every solvable [linear system](system-of-linear-equations.md) $Ax=b$ has a unique solution. It need not reach every output.[Interactive Linear Algebra, §3.2.1, One-to-one matrix transformations theorem and Wide matrices do not have one-to-one transformations](interactive-linear-algebra-by-dan-margalit-and-others/one-to-one-and-onto-transformations.md)

For example,

$$
B=\begin{pmatrix}1&0\\0&1\\1&1\end{pmatrix}
$$

has [full column rank](full-column-rank.md) two, but its [column space](column-space.md) is the [plane](plane.md) $b_3=b_1+b_2$ in $\mathbb R^3$. An attainable output fixes the input uniquely as $(b_1,b_2)^T$; an output outside this [plane](plane.md) has no preimage.

## ↑ Ancestors (9)

1. [Matrix rank](matrix-rank.md)
2. [Matrix](matrix.md)
3. [Linear map](linear-map.md)
4. [Vector space](vector-space-split.md)
5. [Linear algebra](linear-algebra-split.md)
6. [Algebra](algebra-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (22)

- [Full column rank](full-column-rank.md)
- [Full row rank](full-row-rank.md)
- [Invertible matrix](invertible-matrix.md)
- [Linear regression](linear-regression-split.md)
- [Normal equations for linear least squares](normal-equations-for-linear-least-squares.md)
- [Ordinary least squares estimators](ordinary-least-squares-estimators.md)
- [Orthogonal projection matrix](orthogonal-projection-matrix.md)
- [Overdetermined least-squares example](overdetermined-least-squares-example.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-4/13i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-30/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-205/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-206/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-206/2/f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ib/paper-2/18h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-326/1/b/iv/solution.md)
- [QR decomposition](qr-decomposition.md)
- [QR decomposition by Givens rotations](qr-decomposition-by-givens-rotations.md)
- [Rank of a centered sample covariance matrix](rank-of-a-centered-sample-covariance-matrix.md)
- [Reverse-order law for the Moore--Penrose inverse](reverse-order-law-for-the-moore-penrose-inverse.md)
- [Ridge regression](ridge-regression.md)
- [Singular matrix](singular-matrix.md)
- [Trivial kernel](trivial-kernel.md)
