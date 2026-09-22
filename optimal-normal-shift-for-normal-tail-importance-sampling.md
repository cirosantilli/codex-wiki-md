# Optimal normal shift for normal-tail importance sampling

↑ **Parent:** [Importance sampling](importance-sampling.md)

To estimate $\mathbb P(Z>z)$ for a standard normal variable using proposal $N(\mu,1)$, the weighted indicator has second moment $e^{\mu^2}\bar\Phi(z+\mu)$. Differentiating it at a minimum gives the displayed equation. Since $\varphi(a)/\bar\Phi(a)=E[Z\mid Z>a]$, the minimizing shift is half the target conditional mean above the shifted threshold. The resulting estimator remains unbiased with the exact likelihood-ratio weight.

## ↑ Ancestors (6)

1. [Importance sampling](importance-sampling.md)
2. [Monte Carlo method](monte-carlo-method-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
