# Uniqueness of reduced row echelon form

↑ **Parent:** [Reduced row echelon form](reduced-row-echelon-form.md)

Here is a short proof that uses only the [row space](row-space.md). For a [vector subspace](vector-subspace.md) $W\subseteq\mathbb F^n$, let $d_j$ be the [dimension](dimension-vector-space.md) of its [projection map](projection-map.md) onto the first $j$ coordinates, with $d_0=0$. In any [reduced row echelon form](reduced-row-echelon-form.md) with [row space](row-space.md) $W$, $d_j$ counts the [pivot columns](pivot-column.md) among those first $j$ columns: later-pivot rows project to zero, while earlier-pivot rows remain [linearly independent](linear-independence.md). Thus the positions where $d_j-d_{j-1}=1$ determine all pivot positions from $W$ alone.

If those positions are $p_1,\ldots,p_r$, the map sending $w\in W$ to $(w_{p_1},\ldots,w_{p_r})$ is an [isomorphism](isomorphism.md) $W\to\mathbb F^r$: the reduced nonzero rows map to the [standard basis](standard-basis.md). Its $i$th row is therefore the unique [vector](vector.md) of $W$ with pivot-coordinate values equal to the $i$th [standard basis](standard-basis.md) vector. Any other [reduced row echelon form](reduced-row-echelon-form.md) with that [row space](row-space.md) has identical nonzero rows in identical order. At a fixed [matrix](matrix.md) size, the remaining rows must be zero. Together with existence by [Gaussian elimination](gaussian-elimination.md), this proves uniqueness.

## ↑ Ancestors (9)

1. [Reduced row echelon form](reduced-row-echelon-form.md)
2. [Row echelon form](row-echelon-form.md)
3. [Gaussian elimination](gaussian-elimination.md)
4. [Numerical linear algebra](numerical-linear-algebra-split.md)
5. [Numerical analysis](numerical-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)
