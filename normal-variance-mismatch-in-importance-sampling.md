# Normal variance mismatch in importance sampling

↑ **Parent:** [Importance sampling](importance-sampling.md)

For target $p=N(0,\sigma^2)$ and proposal $q=N(0,1)$, this is the [importance weight](importance-weight.md). Assuming only $E_pf^2<\infty$, the weighted estimator has guaranteed finite variance for $0<\sigma\leq1$, since $E_q(w_\sigma^2f^2)=E_p(w_\sigma f^2)\leq\sigma^{-1}E_pf^2$. For every $\sigma>1$, choosing $f^2=e^{ax^2}$ with $\max(0,\sigma^{-2}-1/2)<a<(2\sigma^2)^{-1}$ gives finite target second moment but infinite weighted second moment. With the additional assumption that $f$ is bounded, the sufficient range is instead $\sigma<\sqrt2$. The integrand hypothesis therefore matters.

## ↑ Ancestors (6)

1. [Importance sampling](importance-sampling.md)
2. [Monte Carlo method](monte-carlo-method-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
