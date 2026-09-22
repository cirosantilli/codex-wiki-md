# Optimal cost-constrained stratified sampling allocation

↑ **Parent:** [Stratified sampling](stratified-sampling.md)

Suppose the [variance](variance-split.md) is $\sum_i v_i/x_i$ and the sampling cost is $\sum_i a_ix_i\leq b$, with positive costs, variance coefficients and budget. The [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) gives $A^2\leq(\sum_i v_i/x_i)(\sum_i a_ix_i)\leq b\sum_i v_i/x_i$. Equality forces $x_i$ proportional to $\sqrt{v_i/a_i}$ and a tight budget, proving the displayed unique optimum. The minimal variance is $A^2/b$. For the [optimization Lagrangian](optimization-lagrangian.md) $f-\lambda(\sum_i a_ix_i-b)$, the multiplier and budget derivative both equal $-A^2/b^2$. Therefore a small resource change $\delta b$ changes the optimum by $\lambda\delta b+O((\delta b)^2)$. This is a continuous allocation; integer sample-size restrictions define a separate optimization problem.

## ↑ Ancestors (7)

1. [Stratified sampling](stratified-sampling.md)
2. [Probability sampling](probability-sampling.md)
3. [Statistical inference](statistical-inference-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-35/1/solution.md)
