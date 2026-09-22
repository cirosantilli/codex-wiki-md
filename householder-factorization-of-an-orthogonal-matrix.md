# Householder factorization of an orthogonal matrix

↑ **Parent:** [Householder transformation](householder-transformation.md)

Every real [orthogonal matrix](orthogonal-matrix.md) of dimension $n$ is a product of at most $n$ [Householder matrices](householder-transformation.md). For a first-column unit vector $q\ne e_1$, the reflection with normal $q-e_1$ sends $q$ to $e_1$. Orthogonality then makes the transformed matrix $\operatorname{diag}(1,Q')$, reducing the problem by one dimension. If $q=e_1$, omit that reflection. The dimension-one cases are $1$, the empty product, and $-1$, a single reflection. Induction and reversal of the transformations prove the factorization.

## ↑ Ancestors (6)

1. [Householder transformation](householder-transformation.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford/2007/a/1/a/solution.md)
