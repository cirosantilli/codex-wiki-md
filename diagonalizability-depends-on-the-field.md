# Diagonalizability depends on the field

↑ **Parent:** [Diagonalizable matrix](diagonalizable-matrix.md)

For a [matrix](matrix.md) over a [field](field.md) $F$, [diagonalizability](diagonalizable-matrix.md) requires an [eigenbasis](eigenbasis.md) with entries in $F$ and [eigenvalues](eigenvalue.md) in $F$. Passing to a larger [field](field.md) can supply missing [roots](root-of-a-root-system.md) of the [characteristic polynomial](characteristic-polynomial.md). For example,

$$
A=\begin{pmatrix}0&1&0\\1&1&0\\0&1&1\end{pmatrix},\qquad
\chi_A(t)=(t-1)(t^2-t-1)
$$

is not a [diagonalizable matrix](diagonalizable-matrix.md) over the [rational numbers](rational-number.md), since the quadratic factor has no rational [root](root-of-a-root-system.md). It is a [diagonalizable matrix](diagonalizable-matrix.md) over the [real numbers](real-number.md) and [complex numbers](complex-number.md), since its three [eigenvalues](eigenvalue.md) are distinct. More generally, [diagonalizability](diagonalizable-matrix.md) is equivalent to the [minimal polynomial](minimal-polynomial.md) splitting into distinct linear factors over the specified [field](field.md).

For an integer [matrix](matrix.md), reduction modulo a [prime number](prime-number-split.md) is a different operation from extension of its coefficient [field](field.md), and can merge [eigenvalues](eigenvalue.md). In the same example modulo $5$, $\chi_A(t)=(t-1)(t-3)^2$, while $\ker(A-3I)$ is spanned by $(1,3,4)^T$. Thus the [geometric multiplicity](geometric-multiplicity.md) of $3$ is one and its [algebraic multiplicity](algebraic-multiplicity.md) is two, preventing [diagonalizability](diagonalizable-matrix.md) even though all [eigenvalues](eigenvalue.md) belong to the [finite field](finite-field.md).

## ↑ Ancestors (8)

1. [Diagonalizable matrix](diagonalizable-matrix.md)
2. [Eigenvalue](eigenvalue.md)
3. [Operator theory](linear-operator-theory-split.md)
4. [Linear algebra](linear-algebra-split.md)
5. [Algebra](algebra-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford/2012/2/b/iii/solution.md)
