# Strong convergence of relaxed Landweber iteration

↑ **Parent:** [Landweber iteration](landweber-iteration.md)

For nonzero [compact operator](compact-operator-split.md) $A$, step $0<\tau<2/\|A\|^2$, and data admitting a [minimum-norm least-squares solution](minimum-norm-least-squares-solution.md) $x^\dagger$, zero-initialized [Landweber iteration](landweber-iteration.md) satisfies

$$
 \|x_n-x^\dagger\|^2=\sum_i|1-\tau\sigma_i^2|^{2n}\frac{|\langle y,u_i\rangle|^2}{\sigma_i^2}\longrightarrow0.
$$

The [Picard criterion](picard-criterion.md) makes the majorant summable, so the [dominated convergence theorem](dominated-convergence-theorem.md) proves this limit. No mesh-independent or singular-value-independent strict contraction factor is required. At $\tau=2/\|A\|^2$, the top singular mode has multiplier $-1$ and may not converge. Without solvable projected data, the iterates need not have a limit in the solution [Hilbert space](hilbert-space-split.md), even when their residuals approach the least-squares infimum.

## ↑ Ancestors (7)

1. [Landweber iteration](landweber-iteration.md)
2. [Normal equation for a linear inverse problem](normal-equation-for-a-linear-inverse-problem.md)
3. [Inverse problem](inverse-problem-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-76/3/d/solution.md)
