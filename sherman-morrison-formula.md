<h1 id="sherman-morrison-formula">Sherman–Morrison formula</h1>

↑ **Parent:** [Matrix inverse](matrix-inverse.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sherman–Morrison_formula)

The [Sherman–Morrison formula](sherman-morrison-formula.md) computes the [matrix inverse](matrix-inverse.md) after a [rank-one matrix update](rank-one-matrix-update.md). If $A$ is an [invertible matrix](invertible-matrix.md) and $\delta=1+v^TA^{-1}u\ne0$, then

$$
(A+uv^T)^{-1}
=A^{-1}-\frac{A^{-1}uv^TA^{-1}}{1+v^TA^{-1}u}.
$$

The inverse correction is itself an [outer product](outer-product.md), divided by the [scalar](scalar.md) $\delta$. The [matrix determinant lemma](matrix-determinant-lemma.md) shows that the nonzero-denominator condition is exactly the condition that the updated [matrix](matrix.md) remains an [invertible matrix](invertible-matrix.md).

For $A=I$, $u=(1,2)^T$, and $v=(3,-1)^T$, we have $\delta=2$. Thus the computed inverse is

$$
\boxed{
\begin{pmatrix}4&-1\\6&-1\end{pmatrix}^{-1}
=I-\frac12\begin{pmatrix}3&-1\\6&-2\end{pmatrix}
=\begin{pmatrix}-1/2&1/2\\-3&2\end{pmatrix}
}.
$$

Multiplication in either order gives the [identity matrix](identity-matrix.md). The result reuses the original inverse $I$ and the same correction [vectors](vector.md), rather than solving independently for all four inverse entries.

Often only the solution of an updated [linear system](system-of-linear-equations.md) is needed. If $Ax_0=b$ and $Az=u$, then

$$
(A+uv^T)x=b
\quad\Longrightarrow\quad
x=x_0-z\,\frac{v^Tx_0}{1+v^Tz},
$$

provided $1+v^Tz\ne0$. The two solves use the same [LU decomposition](lu-decomposition.md) of $A$. This expresses the computational benefit without requiring an explicitly stored [matrix inverse](matrix-inverse.md). Strang's [Lecture 14, transcript pp. 9–10](https://ocw.mit.edu/courses/18-065-matrix-methods-in-data-analysis-signal-processing-and-machine-learning-spring-2018/988b4c05680f40a5a4b3be7004a32500_XhSk_Lw2X_U.pdf) explains this reuse of the original factorization.

To see why the inverse correction works, first consider $A=I$ and put $s=v^Tu$. The [rank-one matrix](rank-one-matrix.md) $R=uv^T$ satisfies $R^2=sR$. Expanding

$$
(I+R)\left(I-\frac{R}{1+s}\right)
=I+R-\frac{R}{1+s}-\frac{sR}{1+s}=I
$$

also works in the reverse order. The general case follows by factoring out $A$ and replacing $u$ by $A^{-1}u$. A matrix identity has reduced to cancellation of scalar coefficients.

Historically, Jack Sherman and Winifred J. Morrison studied updating an inverse when a single matrix entry changes in their [1950 paper, Adjustment of an Inverse Matrix Corresponding to a Change in One Element of a Given Matrix](https://doi.org/10.1214/aoms/1177729893). Such an entry change is the special [rank-one matrix update](rank-one-matrix-update.md) $\alpha e_ie_j^T$, with [standard basis](standard-basis.md) [vectors](vector.md) $e_i,e_j$. The reference and the earlier 1949 abstract on row or column changes are recorded in [Henderson and Searle, On Deriving the Inverse of a Sum of Matrices (1981), references 40–41](https://epubs.siam.org/doi/10.1137/1023004). This distinguishes the specific original setting from the more general $uv^T$ formula used here.

**Table of contents**

- [Rank-one update singularity criterion](rank-one-update-singularity-criterion.md)

## ↑ Ancestors (6)

1. [Matrix inverse](matrix-inverse.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Matrix determinant lemma](matrix-determinant-lemma.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-205/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-205/5/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-205/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-218/5/e/solution.md)
- [Rank-one matrix update](rank-one-matrix-update.md)
- [Sherman–Morrison formula](sherman-morrison-formula.md)
