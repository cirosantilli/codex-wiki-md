# Galerkin coarse-grid operator

↑ **Parent:** [Coarse-grid correction](coarse-grid-correction.md)

A Galerkin coarse-grid operator is obtained by composing interpolation, the fine operator and residual restriction. With $R=cP^T$, $c>0$, and positive-definite $A_h$, the exact [coarse-grid correction](coarse-grid-correction.md) $I-P(RA_hP)^{-1}RA_h$ is the energy-orthogonal projection onto the complement of the coarse space. Indeed it annihilates every vector $Pz$, and its corrected error $e'$ satisfies $P^TA_he'=0$. These identities explain why compatible transfers remove representable smooth error rather than merely averaging an approximate solution.

## ↑ Ancestors (7)

1. [Coarse-grid correction](coarse-grid-correction.md)
2. [Multigrid method](multigrid-method.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-67/7/solution.md)
