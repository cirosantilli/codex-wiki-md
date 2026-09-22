# Row-equivalent matrices

↑ **Parent:** [Row echelon form](row-echelon-form.md)

Two [matrices](matrix.md) of the same size over the same [field](field.md) are [row-equivalent matrices](row-equivalent-matrices.md) if a sequence of [elementary row operations](elementary-row-operation.md) transforms one into the other.[Interactive Linear Algebra by Dan Margalit and others; §1.2.1, definition of row equivalence](interactive-linear-algebra-by-dan-margalit-and-others/row-reduction.md) Every operation is reversible, so they have the same [row space](row-space.md) and the same column [linear relations](linear-relation.md). Writing the entire sequence as multiplication by an [invertible matrix](invertible-matrix.md) gives $R=EA$ and

$$
Az=0\ \Longleftrightarrow\ Rz=0,\qquad
Ax=b\ \Longleftrightarrow\ Rx=Eb.
$$

Thus the [kernel](kernel-of-a-linear-map-split.md) is preserved. For a nonzero right-hand side, perform every operation on the whole [augmented matrix](augmented-matrix.md) $[A\mid b]$: changing the coefficients while keeping $b$ fixed generally changes the solutions. The [column space](column-space.md) instead transforms to $E\operatorname{col}A$, which need not equal $\operatorname{col}A$.

## ↑ Ancestors (8)

1. [Row echelon form](row-echelon-form.md)
2. [Gaussian elimination](gaussian-elimination.md)
3. [Numerical linear algebra](numerical-linear-algebra-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Row-equivalent matrices](row-equivalent-matrices.md)
