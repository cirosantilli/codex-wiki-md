# Hessenberg reduction

↑ **Parent:** [Hessenberg matrix](hessenberg-matrix.md)

The reduction of a real square [matrix](matrix.md) to upper Hessenberg form uses [orthogonal similarity transformations](orthogonal-similarity.md). A [Householder reflector](householder-transformation.md) at column $k$ acts on rows $k+1,\ldots,n$ to annihilate entries below row $k+1$, and its matching right action preserves similarity. Previous zeros are preserved. Rank-one application of each reflector gives total $O(n^3)$ work. Subsequent shifted systems with $H-\lambda I$ can be factored in $O(n^2)$ work each because only one entry per column lies below the diagonal.

## ↑ Ancestors (9)

1. [Hessenberg matrix](hessenberg-matrix.md)
2. [Matrix](matrix.md)
3. [Linear map](linear-map.md)
4. [Vector space](vector-space-split.md)
5. [Linear algebra](linear-algebra-split.md)
6. [Algebra](algebra-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Orthogonal similarity](orthogonal-similarity.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford/2010/a/2/b/solution.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford/2010/a/2/c/solution.md)
