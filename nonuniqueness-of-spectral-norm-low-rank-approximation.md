# Nonuniqueness of spectral-norm low-rank approximation

↑ **Parent:** [Low-rank approximation](low-rank-approximation.md)

Even distinct [singular values](singular-value.md) do not make a best [low-rank approximation](low-rank-approximation.md) unique in the [spectral norm](matrix-2-norm.md). If $A=\sum_{j=1}^n\sigma_ju_jv_j^T$ has $\sigma_1>\cdots>\sigma_n>0$ and $1\leq r<n$, its [truncated singular value decomposition](truncated-singular-value-decomposition.md) $A_r$ can be changed to $A_r+t u_1v_1^T$ for any $|t|\leq\sigma_{r+1}$. Its [matrix rank](matrix-rank.md) stays $r$ since $\sigma_1+t>0$, while the [spectral norm](matrix-2-norm.md) error is $\max(|t|,\sigma_{r+1})=\sigma_{r+1}$, the optimum from the [Eckart-Young-Mirsky theorem](eckart-young-mirsky-theorem.md).

## ↑ Ancestors (6)

1. [Low-rank approximation](low-rank-approximation.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-numerical-analysis-course-of-the-university-of-oxford/2021/2/b/iii/solution.md)
