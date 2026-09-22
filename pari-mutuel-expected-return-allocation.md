# Pari-mutuel expected-return allocation

↑ **Parent:** [Convex optimization](convex-optimization-split.md)

For positive existing stakes $s_i$ and budget $b$, maximizing $\sum_i p_ix_i/(s_i+x_i)$ is equivalent to minimizing $\sum_i p_is_i/(s_i+x_i)$. A positive multiplier $\tau$ chosen so that $\sum_i x_i=b$ gives the displayed allocation. Each coordinate minimizes $p_is_i/(s_i+x)+\tau x$ on $x\ge0$, which proves global optimality by [Lagrangian sufficiency theorem](lagrange-sufficiency-theorem.md). Its active set is ordered by $p_i/s_i$. Zero existing stakes require a separate payoff convention and can cause nonattainment; the positive-stake formula should not be extended through undefined ratios.

## ↑ Ancestors (5)

1. [Convex optimization](convex-optimization-split.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-4/14h/solution.md)
