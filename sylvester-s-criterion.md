<h1 id="sylvester-s-criterion">Sylvester's criterion</h1>

↑ **Parent:** [Positive-definite matrix](positive-definite-matrix.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sylvester's_criterion)

A [Hermitian matrix](hermitian-operator.md) $A$ is a [positive-definite matrix](positive-definite-matrix.md) exactly when its [leading principal minors](leading-principal-minor.md)

$$
\Delta_k=\det A_{1:k,1:k},\qquad k=1,\ldots,n,
$$

are all positive. The [leading principal minor](leading-principal-minor.md) uses the first $k$ rows and the first $k$ columns in the same ordering. For the two-by-two [Cholesky decomposition](cholesky-decomposition.md) example, $\Delta_1=4$ and $\Delta_2=4\cdot5-2^2=16$, so the criterion proves [positive definiteness](positive-definiteness.md) without calculating [eigenvalues](eigenvalue.md).

The successive [pivot elements](pivot-element.md) before taking [square roots](square-root.md) are $\Delta_k/\Delta_{k-1}$, with $\Delta_0=1$. Here they are $4$ and $16/4=4$. In general, a leading [triangular matrix](triangular-matrix.md) factor has [determinant](determinant.md) equal to the product of its diagonal entries, so

$$
\Delta_k=\prod_{j=1}^k\ell_{jj}^{\,2}.
$$

Conversely, positive [leading principal minors](leading-principal-minor.md) make each successive [Schur complement](schur-complement.md) [pivot element](pivot-element.md) positive, allowing the [Cholesky decomposition](cholesky-decomposition.md) to be constructed. The identity $u^TAu=\|L^Tu\|_2^2$ then proves [positive definiteness](positive-definiteness.md); for complex [matrices](matrix.md), replace the [transposes](transpose.md) by [conjugate transposes](conjugate-transpose.md). This gives a short inductive proof of the criterion.

For $B=\begin{pmatrix}1&2\\2&1\end{pmatrix}$, the first minor is positive but $\det B=-3$. The second Cholesky radicand would be $1-2^2=-3$, and $v=(1,-1)^T$ directly gives $v^TBv=-2<0$. Thus positive diagonal entries are insufficient. Replacing “positive” by “nonnegative” in just the leading-minor test is also insufficient for [positive semidefiniteness](positive-semidefinite-matrix.md): $\operatorname{diag}(0,-1)$ has leading minors $0,0$, but its [quadratic form](quadratic-form-split.md) is negative on $(0,1)^T$.

## ↑ Ancestors (8)

1. [Positive-definite matrix](positive-definite-matrix.md)
2. [Definite matrix](definite-matrix.md)
3. [Quadratic form](quadratic-form-split.md)
4. [Linear algebra](linear-algebra-split.md)
5. [Algebra](algebra-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (10)

- [Cholesky decomposition](cholesky-decomposition.md)
- [Leading principal minor](leading-principal-minor.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-35/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-4/10g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-20/1/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-1/5b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-4/1f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-111/2/a/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2008/paper-2/16/b/ii/solution.md)
- [Two-by-two positive-definiteness test](two-by-two-positive-definiteness-test.md)
