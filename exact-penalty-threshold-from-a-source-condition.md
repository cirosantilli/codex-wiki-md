# Exact-penalty threshold from a source condition

↑ **Parent:** [Exact penalty method](exact-penalty-method.md)

Suppose $Au^\dagger=f$ and $p^\dagger=A^*\mu^\dagger\in\partial J(u^\dagger)$. For $F_\alpha(u)=\|Au-f\|+\alpha J(u)$, the [subgradient inequality](subgradient-inequality.md) and [dual pairing](dual-pairing.md) bound give

$$
F_\alpha(u)-F_\alpha(u^\dagger)
\geq(1-\alpha\|\mu^\dagger\|)\|Au-f\|.
$$

Thus $0<\alpha\|\mu^\dagger\|<1$ forces every minimizer to solve $Au=f$ exactly. Comparison of penalties then shows it is a [J-minimizing solution](j-minimizing-solution.md), and $D_J^{p^\dagger}(u,u^\dagger)=0$. The conclusion also holds for all $\alpha>0$ when $\mu^\dagger=0$. One-homogeneity is not needed for this argument.

## ↑ Ancestors (8)

1. [Exact penalty method](exact-penalty-method.md)
2. [Variational regularization](variational-regularization.md)
3. [Regularization of an inverse problem](regularization-of-an-inverse-problem.md)
4. [Inverse problem](inverse-problem-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-326/4/c/solution.md)
