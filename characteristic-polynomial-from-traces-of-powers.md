# Characteristic polynomial from traces of powers

↑ **Parent:** [Newton's identities](newton-s-identities.md)

For a complex $n\times n$ [matrix](matrix.md) $A$, $\operatorname{tr}(A^k)$ is the sum of the $k$th powers of its [eigenvalues](eigenvalue.md), counted with [algebraic multiplicity](algebraic-multiplicity.md). This does not require [diagonalizability](diagonalizable-matrix.md): a similar [upper triangular matrix](upper-triangular-matrix.md) has the [eigenvalues](eigenvalue.md) on its diagonal, and taking powers raises those diagonal entries to their corresponding powers. [Newton's identities](newton-s-identities.md) therefore recover its [characteristic polynomial](characteristic-polynomial.md) from the first $n$ such [traces](matrix-trace.md).

For the [Jordan block](jordan-block.md) $A=\begin{pmatrix}2&1\\0&2\end{pmatrix}$, $\operatorname{tr}A=4$ and $\operatorname{tr}(A^2)=8$. Hence $e_1=4$ and $e_2=(4^2-8)/2=4$, giving **$\det(zI-A)=z^2-4z+4=(z-2)^2$**. The repeated [eigenvalue](eigenvalue.md) is recovered even though this [matrix](matrix.md) is not [diagonalizable](diagonalizable-matrix.md).[§5, pp. 4–5](rational-univariate-representation-lecture-12-by-jan-verschelde.md)

## ↑ Ancestors (7)

1. [Newton's identities](newton-s-identities.md)
2. [Elementary symmetric polynomial](elementary-symmetric-polynomial.md)
3. [Polynomial](polynomial-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-2/6/b/solution.md)
