# Horn copositive matrix

↑ **Parent:** [Copositive matrix](copositive-matrix.md)

The five-dimensional Horn copositive matrix has diagonal entries $1$, entries $-1$ on the edges of the five-cycle, and entries $1$ on the remaining pairs:

$$
H=\begin{pmatrix}
1&-1&1&1&-1\\
-1&1&-1&1&1\\
1&-1&1&-1&1\\
1&1&-1&1&-1\\
-1&1&1&-1&1
\end{pmatrix}.
$$

For $x\geq0$, a cyclic relabelling puts a smallest coordinate at $x_5$. The identity

$$
x^THx=(x_1-x_2+x_3-x_4+x_5)^2+4x_2x_5+4x_1(x_4-x_5)
$$

then proves that $H$ is a [copositive matrix](copositive-matrix.md).

However, $H$ is outside the [positive-semidefinite-plus-nonnegative cone](positive-semidefinite-plus-nonnegative-cone.md). Set $w=(1,2,1,0,0)^T$. Its [quadratic form](quadratic-form.md) is zero. If $H=P+N$ with $P$ a [positive semidefinite matrix](positive-semidefinite-matrix.md) and $N$ a symmetric [nonnegative matrix](nonnegative-matrix.md), both $w^TPw$ and $w^TNw$ must vanish. Positivity of the first three coordinates of $w$ forces every entry of the leading $3\times3$ block of $N$ to vanish. Applying the argument to all cyclic shifts of $w$ forces every entry of $N$ to vanish, since each pair of indices lies in a cyclic interval of length three. This would make $H$ a [positive semidefinite matrix](positive-semidefinite-matrix.md), but [zero quadratic form of a positive semidefinite matrix](zero-quadratic-form-of-a-positive-semidefinite-matrix.md) would then give $Hw=0$, whereas $Hw=(0,0,0,2,2)^T$.

## ↑ Ancestors (7)

1. [Copositive matrix](copositive-matrix.md)
2. [Symmetric matrix](symmetric-matrix.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Copositive matrix](copositive-matrix.md)
- [Nonnegative polynomial](nonnegative-polynomial.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-339/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-339/3/d/solution.md)
- [Positive-semidefinite-plus-nonnegative cone](positive-semidefinite-plus-nonnegative-cone.md)
