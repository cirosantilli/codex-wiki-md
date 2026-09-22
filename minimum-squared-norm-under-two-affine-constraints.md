# Minimum squared norm under two affine constraints

↑ **Parent:** [Lagrange sufficiency theorem](lagrange-sufficiency-theorem.md)

For real $a_i$ not all equal, let $S_1=\sum_i a_i$, $S_2=\sum_i a_i^2$ and $\Delta=nS_2-S_1^2>0$. The unique minimizer of $\sum_i x_i^2$ under $\sum_i x_i=1$, $\sum_i a_ix_i=0$ is $x_i^*=(S_2-S_1a_i)/\Delta$, with minimum $S_2/\Delta$. To prove sufficiency, the [optimization Lagrangian](optimization-lagrangian.md) with multipliers $\lambda=S_2/\Delta$, $\mu=-S_1/\Delta$ is a sum of squares in $x_i-\lambda-\mu a_i$ plus a constant. Equivalently every feasible $x$ satisfies $\sum_i x_i^2-\sum_i(x_i^*)^2=\sum_i(x_i-x_i^*)^2$.

## ↑ Ancestors (5)

1. [Lagrange sufficiency theorem](lagrange-sufficiency-theorem.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-3/5d/solution.md)
