# Dyadic quadratic variation of a bounded continuous martingale

↑ **Parent:** [Quadratic variation](quadratic-variation.md)

Let $X$ be a continuous martingale on $[0,1]$ with $X_0=0$ and $|X_t|\le C$. For the dyadic squared-increment sums, including the unfinished increment at time $t$, set $A_t^{(n)}=\sum_k(X_{k2^{-n}\wedge t}-X_{(k-1)2^{-n}\wedge t})^2$. The associated martingale transform $M_t^{(n)}=(X_t^2-A_t^{(n)})/2$ satisfies $\mathbb E(M_1^{(n)})^2\le C^4$ and $\mathbb E(A_1^{(n)})^2\le10C^4$. Discrete martingale orthogonality, the path modulus of continuity and the [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) show that the terminal transforms are Cauchy in $L^2$. The [Doob L2 maximal inequality](doob-l2-maximal-inequality.md) then gives $\mathbb E\sup_{t\le1}|A_t^{(n)}-A_t^{(m)}|^2\to0$. The sums need not be increasing in time before taking the limit. This provides an elementary construction of [quadratic variation](quadratic-variation.md) under boundedness.

## ↑ Ancestors (8)

1. [Quadratic variation](quadratic-variation.md)
2. [Stochastic calculus](stochastic-calculus-split.md)
3. [Stochastic process](stochastic-process-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-25/3/d/solution.md)
