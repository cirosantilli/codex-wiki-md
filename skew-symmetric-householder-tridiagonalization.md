# Skew-symmetric Householder tridiagonalization

↑ **Parent:** [Householder tridiagonalization](householder-tridiagonalization.md)

An [orthogonal](orthogonal-vectors.md) similarity preserves skew symmetry, so upper-Hessenberg reduction of a real [skew-symmetric matrix](skew-symmetric-matrix.md) is automatically tridiagonal with zero diagonal. For a [Householder reflection](householder-transformation.md), the scalar $v^TAv$ vanishes, eliminating the fourth term of the general similarity update. Storing only one triangle and using the displayed skew rank-two update costs $2n^3/3+O(n^2)$ scalar products, the same leading product count as optimized symmetric tridiagonalization; the simplification saves lower-order work.

## ↑ Ancestors (7)

1. [Householder tridiagonalization](householder-tridiagonalization.md)
2. [Numerical linear algebra](numerical-linear-algebra.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-4/39a/a/solution.md)
