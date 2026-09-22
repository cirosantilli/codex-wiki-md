# Practical stability of a finite difference scheme

↑ **Parent:** [Stability of a numerical method](stability-of-a-numerical-method.md)

In the contraction convention for numerical evolution, practical stability means non-growth of the chosen [norm](norm.md) for every datum and every permitted time level. This is stronger than finite-time mesh-uniform [stability](stability-of-a-numerical-method.md) allowing a bound $C_T\|U^0\|$. For a scalar translation-invariant one-step scheme on the infinite grid, a [Fourier amplification symbol](fourier-amplification-symbol.md) $G$ with $|G|\leq1$ gives this contraction by the [Parseval identity](parseval-identity.md). If $|G|\geq1+c>1$ on a frequency set of positive measure, choose a nonzero square-integrable transform supported there to obtain $\|U^m\|\geq(1+c)^m\|U^0\|$. The constant $c$ may depend on the mesh. Centered pure advection with forward time has $c=\sqrt{1+(\Delta t/\Delta x)^2/2}-1$ on the set $\sin^2\theta\geq1/2$. The distinction from finite-time [stability](stability-of-a-numerical-method.md) is quantified by [centered-advection refinement-dependent stability](centered-advection-refinement-dependent-stability.md).

## ↑ Ancestors (6)

1. [Stability of a numerical method](stability-of-a-numerical-method.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [2023](past-exam-of-the-numerical-solutions-of-partial-differential-equations-course-of-the-university-of-oxford/2023-split.md)
- [Solution](past-exam-of-the-numerical-solutions-of-partial-differential-equations-course-of-the-university-of-oxford/2023/3/b/solution.md)
- [Solution](past-exam-of-the-numerical-solutions-of-partial-differential-equations-course-of-the-university-of-oxford/2023/3/e/solution.md)
