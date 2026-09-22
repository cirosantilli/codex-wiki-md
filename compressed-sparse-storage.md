# Compressed sparse storage

↑ **Parent:** [Sparse matrix](sparse-matrix.md)

[Compressed sparse storage](compressed-sparse-storage.md) keeps a [sparse matrix](sparse-matrix.md) as numerical nonzero values, their row or column indices, and pointers to the start of each compressed column or row. It avoids allocating all $N^2$ entries. A sparse direct solver must additionally allocate possible [fill-in](fill-in.md) predicted by [symbolic factorization](symbolic-factorization.md), because elimination can create entries absent from the input.

## ↑ Ancestors (9)

1. [Sparse matrix](sparse-matrix.md)
2. [Matrix](matrix.md)
3. [Linear map](linear-map.md)
4. [Vector space](vector-space-split.md)
5. [Linear algebra](linear-algebra-split.md)
6. [Algebra](algebra-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Compressed sparse storage](compressed-sparse-storage.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-60/6/solution.md)
