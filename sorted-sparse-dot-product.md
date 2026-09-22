# Sorted sparse dot product

↑ **Parent:** [Sparse linked vector representation](sparse-linked-vector-representation.md)

For two [sparse vectors](sparse-vector.md) with the same dimension and sorted nonzero entries, merge their coordinate lists. Equal indices contribute their product and advance both cursors. If one index is smaller, advance only that cursor: the other [vector](vector.md) has zero at that coordinate, because all its smaller indices have already been processed and all remaining indices are larger. This proves a [loop invariant](loop-invariant.md) consisting of the accumulated [inner product](inner-product-split.md) over settled indices. Every iteration consumes at least one stored entry, giving [time complexity](time-complexity.md) $O(k_x+k_y+1)$ and constant [auxiliary space](auxiliary-space.md) for $k_x,k_y$ nonzero entries. The method avoids work proportional to the ambient dimension. Its [floating-point arithmetic](floating-point-arithmetic-split.md) error remains distinct from its exact [algorithm correctness](algorithm-correctness.md).

## ↑ Ancestors (9)

1. [Sparse linked vector representation](sparse-linked-vector-representation.md)
2. [Sparse vector](sparse-vector.md)
3. [Compressed sensing](compressed-sensing.md)
4. [Sparse optimization](sparse-optimization.md)
5. [Numerical analysis](numerical-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/imperative-programming/3/g/solution.md)
