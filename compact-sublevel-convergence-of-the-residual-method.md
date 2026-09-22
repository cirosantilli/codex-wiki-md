# Compact-sublevel convergence of the residual method

↑ **Parent:** [Residual method for variational regularization](residual-method-for-variational-regularization.md)

Suppose $J$ is nonnegative and [sequentially lower semicontinuous](sequential-lower-semicontinuity.md), and its sublevel sets are strongly sequentially compact. For a solvable exact equation $Au=f$, every sequence of residual-method minimizers with $\delta\to0$ has a strongly convergent subsequence, and every limit is a [J-minimizing solution](j-minimizing-solution.md). Indeed, comparison with an exact penalty minimizer bounds all reconstructions in one compact sublevel set; the residual bound gives $\|Au_\delta-f\|\leq2\delta$. Continuity of $A$ and lower semicontinuity of $J$ identify each subsequential limit as an exact minimizer. Thus the [distance to a set](distance-to-a-set.md) of exact penalty minimizers tends to zero. Uniqueness of the exact minimizer upgrades this to full [strong convergence](norm-convergence.md).

Uniqueness cannot be omitted: for $A=0$, $f_\delta=f=0$, and $J(u)=\max\{|u|-1,0\}$ on $\mathbb R$, the sublevel sets are compact intervals but the minimizers $u_{1/k}=(-1)^k$ do not converge.

## ↑ Ancestors (8)

1. [Residual method for variational regularization](residual-method-for-variational-regularization.md)
2. [Variational regularization](variational-regularization.md)
3. [Regularization of an inverse problem](regularization-of-an-inverse-problem.md)
4. [Inverse problem](inverse-problem-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-326/2/c/solution.md)
