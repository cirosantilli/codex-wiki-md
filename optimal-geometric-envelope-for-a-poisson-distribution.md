# Optimal geometric envelope for a Poisson distribution

↑ **Parent:** [Rejection sampling](rejection-sampling.md)

For a [Poisson distribution](poisson-distribution.md) target of mean $\lambda>0$ and a [geometric distribution](geometric-distribution.md) proposal with [probability mass function](probability-mass-function.md) $q_k=(1-t)t^k$ on the nonnegative integers, the tight [rejection sampling](rejection-sampling.md) envelope is

$$
M(t)=\frac{e^{-\lambda}}{1-t}\frac{(\lambda/t)^m}{m!},\qquad m=\lfloor\lambda/t\rfloor.
$$

Successive target-to-proposal ratios have ratio $\lambda/[t(k+1)]$, proving this maximizing index. The function $\log M(t)$ is the maximum of the [convex functions](convex-function.md) $-\lambda-\log(1-t)+k\log(\lambda/t)-\log(k!)$. Within a branch its [derivative](derivative.md) is $(1-t)^{-1}-m/t$.

Writing $K=\lceil\lambda\rceil$, the optimum is $t_*=\min\{\lambda/K,K/(K+1)\}$, and the success parameter is $\rho_*=1-t_*$. For $K-1<\lambda\leq K^2/(K+1)$, $t_* =\lambda/K$ is a branch boundary; the left and right [derivatives](derivative.md) are nonpositive and nonnegative respectively. For $K^2/(K+1)<\lambda\leq K$, the active branch has a zero [derivative](derivative.md) at $t_*=K/(K+1)$, including a tie at the upper endpoint. Convexity proves global optimality. The minimum expected proposal count is $M(t_*)$; no claim about machine-specific instruction costs is implied.

## ↑ Ancestors (6)

1. [Rejection sampling](rejection-sampling.md)
2. [Monte Carlo method](monte-carlo-method-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-simulation-and-statistical-programming-course-of-the-university-of-oxford/2021/2/a/iii/solution.md)
