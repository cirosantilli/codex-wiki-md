# Full row rank

↑ **Parent:** [Matrix rank](matrix-rank.md)

An $m\times n$ [matrix](matrix.md) has [full row rank](full-row-rank.md) when its [matrix rank](matrix-rank.md) is $m$, equivalently when its rows are [linearly independent vectors](linear-independence.md). This requires $m\leq n$. Its [column space](column-space.md) is all of $\mathbb F^m$, so the represented [linear map](linear-map.md) is [surjective](surjective-function.md) and every [linear system](system-of-linear-equations.md) $Ax=b$ is solvable. If $n>m$, its [nullity](nullity-of-a-linear-map.md) is $n-m>0$, so solutions are not unique.[Interactive Linear Algebra, §3.2.2, Onto matrix transformations theorem and Tall matrices do not have onto transformations](interactive-linear-algebra-by-dan-margalit-and-others/one-to-one-and-onto-transformations.md)

For example, the [matrix transpose](transpose.md) of the [matrix](matrix.md) in [full column rank](full-column-rank.md) is

$$
B^T=\begin{pmatrix}1&0&1\\0&1&1\end{pmatrix}.
$$

It has [full row rank](full-row-rank.md) two. Every output $(p,q)^T$ has solutions $(p-t,q-t,t)^T$, with $t\in\mathbb R$. A [square matrix](square-matrix.md) of size $n$ has [full row rank](full-row-rank.md) and [full column rank](full-column-rank.md) together exactly when its [matrix rank](matrix-rank.md) is $n$; then it is an [invertible matrix](invertible-matrix.md). A nonsquare [matrix](matrix.md) cannot have both properties, and has no two-sided inverse: such an inverse would make its [linear map](linear-map.md) a [linear isomorphism](linear-isomorphism.md) between [vector spaces](vector-space-split.md) of different [dimensions](dimension-vector-space.md).

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

## ← Incoming links (9)

- [Full row rank](full-row-rank.md)
- [Invertible matrix](invertible-matrix.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-31/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-326/1/b/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-339/2/c/ii/solution.md)
- [Reverse-order law for the Moore--Penrose inverse](reverse-order-law-for-the-moore-penrose-inverse.md)
- [Singular matrix](singular-matrix.md)
- [Trivial kernel](trivial-kernel.md)
- [Underdetermined minimum-norm example](underdetermined-minimum-norm-example.md)
