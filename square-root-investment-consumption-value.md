# Square-root investment-consumption value

↑ **Parent:** [Constant relative risk aversion utility](constant-relative-risk-aversion-utility.md)

For zero cash interest, constant excess drift $\mu$, volatility $\sigma$, and both terminal and consumption utility $2\sqrt{x}$, set $A=\sigma\sigma^T$ and assume $\mu$ belongs to the [image of a linear map](image-of-a-linear-map.md) $A$. Let $A^+$ be the [Moore-Penrose inverse](moore-penrose-inverse.md) and $q=\mu^T A^+\mu$. Then $h'+qh+1=0$, $h(T)=1$, so $h(t)=e^{q(T-t)}+(e^{q(T-t)}-1)/q$ for $q>0$, and $h(t)=1+T-t$ for $q=0$. The [Hamilton-Jacobi-Bellman equation](hamilton-jacobi-bellman-equation.md) has the displayed solution. Maximizing dollar investment and consumption are $\theta_t=2X_t A^+\mu$ and $C_t=X_t/h(t)$. The resulting positive [portfolio wealth](portfolio-wealth.md) is a [geometric Brownian motion](geometric-brownian-motion.md) with a deterministic time-dependent drift, and finite-horizon moment bounds justify equality in verification.

## ↑ Ancestors (7)

1. [Constant relative risk aversion utility](constant-relative-risk-aversion-utility.md)
2. [Utility function](utility-function-split.md)
3. [Mathematical finance](mathematical-finance-split.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-42/2/solution.md)
