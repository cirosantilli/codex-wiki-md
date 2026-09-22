# Reduced row echelon form

↑ **Parent:** [Row echelon form](row-echelon-form.md)

A [row echelon form](row-echelon-form.md) is in [reduced row echelon form](reduced-row-echelon-form.md) when every [pivot element](pivot-element.md) is one and is the only nonzero entry in its column.[Interactive Linear Algebra by Dan Margalit and others; §1.2.2, reduced echelon conditions 4 and 5](interactive-linear-algebra-by-dan-margalit-and-others/row-reduction.md) This extra reduction displays each pivot unknown directly in terms of the [free variables in a linear system](free-variable-in-a-linear-system.md). The zero [matrix](matrix.md) also satisfies the definition: it has no [pivot elements](pivot-element.md).

Every [matrix](matrix.md) has exactly one [reduced row echelon form](reduced-row-echelon-form.md) under [elementary row operations](elementary-row-operation.md), with its size and column order held fixed.[Interactive Linear Algebra by Dan Margalit and others; §1.2.3, theorem preceding the Row Reduction Algorithm](interactive-linear-algebra-by-dan-margalit-and-others/row-reduction.md) Ordinary [row echelon form](row-echelon-form.md) is not unique: multiplying a nonzero row by two over the [rational numbers](rational-number.md) keeps the staircase but changes the [matrix](matrix.md). The reduced conditions remove that freedom.

For a fixed number of columns, each [row space](row-space.md) has a unique reduced [matrix](matrix.md) after zero rows are removed; at a fixed full size, the number of appended zero rows is also determined. Thus [reduced row echelon form](reduced-row-echelon-form.md) represents a [vector subspace](vector-subspace.md) independently of the starting [basis](basis.md). This is the uniqueness used by [Gaussian binomial coefficients](gaussian-binomial-coefficient.md) to count [vector subspaces](vector-subspace.md) over a [finite field](finite-field.md).

The fixed column order matters. [Elementary column operations](elementary-column-operation.md) can change the [row space](row-space.md), the [kernel](kernel-of-a-linear-map-split.md) and the resulting [reduced row echelon form](reduced-row-echelon-form.md). For instance, swapping the columns of $(1\ \ 2)$ over the [rational numbers](rational-number.md) gives $(2\ \ 1)$, whose [reduced row echelon form](reduced-row-echelon-form.md) is $(1\ \ 1/2)$ instead of $(1\ \ 2)$. When solving a [linear system](system-of-linear-equations.md), a column interchange also requires tracking the corresponding interchange of unknowns.

**Table of contents**

- [Reading solutions from reduced row echelon form](reading-solutions-from-reduced-row-echelon-form.md)
- [Uniqueness of reduced row echelon form](uniqueness-of-reduced-row-echelon-form.md)

## ↑ Ancestors (8)

1. [Row echelon form](row-echelon-form.md)
2. [Gaussian elimination](gaussian-elimination.md)
3. [Numerical linear algebra](numerical-linear-algebra-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Gaussian binomial coefficient counts finite-field subspaces](gaussian-binomial-coefficient-counts-finite-field-subspaces.md)
- [Matrix rank](matrix-rank.md)
- [Reduced row echelon form](reduced-row-echelon-form.md)
- [Row echelon form](row-echelon-form.md)
- [Row rank](row-rank.md)
- [Row reduction with a parameterized right-hand side](row-reduction-with-a-parameterized-right-hand-side.md)
- [Uniqueness of reduced row echelon form](uniqueness-of-reduced-row-echelon-form.md)
