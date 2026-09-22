# Row rank

↑ **Parent:** [Matrix rank](matrix-rank.md)

The [row rank](row-rank.md) of a [matrix](matrix.md) is the [dimension](dimension-vector-space.md) of the [vector space](vector-space-split.md) spanned by its rows. [Elementary row operations](elementary-row-operation.md) preserve this [row space](row-space.md); multiplication on the right by an [invertible matrix](invertible-matrix.md) preserves all [linear relations](linear-relation.md) among the rows.

To see why [row rank](row-rank.md) equals [column rank](column-rank.md), write a [reduced row echelon form](reduced-row-echelon-form.md) as $R=EA$, where $E$ is a product of [elementary matrices](elementary-matrix.md) and is an [invertible matrix](invertible-matrix.md). Reversibility of the [row operations](elementary-row-operation.md) gives equal [row spaces](row-space.md) for $R$ and $A$. Also $Rz=0$ if and only if $Az=0$, so the columns have exactly the same [linear relations](linear-relation.md). If $R$ has $r$ nonzero rows, its [pivot columns](pivot-column.md) are the first $r$ [standard basis](standard-basis.md) [vectors](vector.md) of $\mathbb F^m$ and span its [column space](column-space.md). Its nonzero rows are [linearly independent](linear-independence.md), since their [matrix entries](matrix-entry.md) in the pivot positions form an [identity matrix](identity-matrix.md). Both [dimensions](dimension-vector-space.md) therefore equal $r$, and both counts transfer back to $A$.

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

## ← Incoming links (5)

- [Column rank](column-rank.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-3/10g/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-1/9e/solution.md)
- [Row echelon form](row-echelon-form.md)
- [Row rank](row-rank.md)
