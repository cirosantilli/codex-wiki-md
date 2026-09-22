# Backward stability

↑ **Parent:** [Numerical analysis](numerical-analysis-split.md)

A [numerical algorithm](numerical-algorithm.md) is backward stable when its computed output is the exact output for input data perturbed by an amount comparable to the arithmetic's [round-off error](round-off-error.md). The allowed input perturbations and their [norm](norm.md) must be specified. A bound on [backward error](backward-error.md) gives a [forward error](forward-error.md) bound only after accounting for the problem's [condition number](condition-number.md). For example, a [singular value decomposition](singular-value-decomposition.md) with [orthonormal](orthonormal-set.md) computed outer factors is backward stable in the [spectral norm](matrix-2-norm.md) if $\|A-\widehat U\widehat\Sigma\widehat V^T\|_2\leq c u\|A\|_2$, with machine precision $u$ and a modest dimension-dependent constant $c$.

## ↑ Ancestors (5)

1. [Numerical analysis](numerical-analysis-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-numerical-linear-algebra-course-of-the-university-of-oxford/2025/1/b/ii/solution.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-course-of-the-university-of-oxford/2025/1/b/iii/solution.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-course-of-the-university-of-oxford/2025/1/b/iv/solution.md)
