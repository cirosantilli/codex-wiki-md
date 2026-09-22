# Row echelon form

↑ **Parent:** [Gaussian elimination](gaussian-elimination.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Row_echelon_form)

A [matrix](matrix.md) over a [field](field.md) $\mathbb F$ is in [row echelon form](row-echelon-form.md) when all zero rows follow the nonzero rows, each nonzero row's first nonzero entry lies strictly to the right of the preceding row's first nonzero entry, and all entries below each such leading entry vanish. These leading entries are its [pivot elements](pivot-element.md). They need not be one, and entries above them need not vanish.[Interactive Linear Algebra by Dan Margalit and others; §1.2.2, Echelon Forms: three echelon conditions and definition of a pivot](interactive-linear-algebra-by-dan-margalit-and-others/row-reduction.md)

The staircase turns a [linear system](system-of-linear-equations.md) into a sequence of simpler equations. For example,

$$
U=\begin{pmatrix}1&2&-1\\0&1&3\\0&0&0\\0&0&0\end{pmatrix}
$$

is in [row echelon form](row-echelon-form.md), with [pivot columns](pivot-column.md) 1 and 2. Its second equation determines $x_2$ once $x_3$ is chosen; its first then determines $x_1$ by [back substitution](back-substitution.md). It is not in [reduced row echelon form](reduced-row-echelon-form.md), because the second [pivot column](pivot-column.md) contains a nonzero entry above its [pivot element](pivot-element.md). Neither being square nor having a nonzero entry in every row is required.

[Elementary row operations](elementary-row-operation.md) bring every [matrix](matrix.md) to [row echelon form](row-echelon-form.md): choose a nonzero entry in the leftmost available nonzero column, interchange rows, clear entries below it, and repeat on the remaining rows and later columns. Skip columns with no remaining nonzero entry. Clearing above each [pivot element](pivot-element.md) and scaling it to one completes [reduced row echelon form](reduced-row-echelon-form.md).[Interactive Linear Algebra by Dan Margalit and others; §1.2.3, The Row Reduction Algorithm, forward steps and Last Step](interactive-linear-algebra-by-dan-margalit-and-others/row-reduction.md)

The nonzero rows of an [row echelon form](row-echelon-form.md) are [linearly independent](linear-independence.md): in a vanishing [linear combination](linear-combination.md), inspecting the first [pivot column](pivot-column.md) forces the first coefficient to be zero, then the next forces the second, and so on. They give a [basis](basis.md) of the original [row space](row-space.md). The number of [pivot elements](pivot-element.md) is both the [row rank](row-rank.md) and the [column rank](column-rank.md). To recover a [basis](basis.md) of the original [column space](column-space.md), select the corresponding original [pivot columns](pivot-column.md); the reduced column [vectors](vector.md) generally belong to a different [column space](column-space.md).

Here the arithmetic is exact in the specified [field](field.md). For [floating-point arithmetic](floating-point-arithmetic-split.md), deciding whether a computed entry counts as zero requires a numerical criterion; see [Tiny-pivot roundoff in Gaussian elimination](tiny-pivot-roundoff-in-gaussian-elimination.md) and [condition number](condition-number.md). An exact [row echelon form](row-echelon-form.md) classification alone does not settle [numerical stability](stability-of-a-numerical-method.md).

**Table of contents**

- [Row-equivalent matrices](row-equivalent-matrices.md)
- [Row reduction with a parameterized right-hand side](row-reduction-with-a-parameterized-right-hand-side.md)
- [Reduced row echelon form](reduced-row-echelon-form.md)
  - [Reading solutions from reduced row echelon form](reading-solutions-from-reduced-row-echelon-form.md)
  - [Uniqueness of reduced row echelon form](uniqueness-of-reduced-row-echelon-form.md)

## ↑ Ancestors (7)

1. [Gaussian elimination](gaussian-elimination.md)
2. [Numerical linear algebra](numerical-linear-algebra-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Column rank](column-rank.md)
- [Free variable in a linear system](free-variable-in-a-linear-system.md)
- [Gaussian elimination](gaussian-elimination.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-1/9e/solution.md)
- [Pivot column](pivot-column.md)
- [Reduced row echelon form](reduced-row-echelon-form.md)
- [Row echelon form](row-echelon-form.md)
- [Row reduction with a parameterized right-hand side](row-reduction-with-a-parameterized-right-hand-side.md)
