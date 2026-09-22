# Discounted boundary-hitting representation

↑ **Parent:** [Feynman-Kac formula](feynman-kac-formula.md)

For a continuous [Itô diffusion](ito-diffusion.md) with [diffusion generator](diffusion-generator.md) $\mathcal L$, let $u$ solve $\mathcal Lu=\lambda u$ with $\lambda>0$, be bounded on an open domain and its boundary, and equal $g$ on the boundary. Stop at the first boundary hit $\tau$. The [Itô formula](ito-s-lemma.md) makes $e^{-\lambda(t\wedge\tau)}u(X_{t\wedge\tau})$ a bounded martingale. Its limit is zero on $\{\tau=\infty\}$ and equals $e^{-\lambda\tau}g(X_\tau)$ on $\{\tau<\infty\}$. Thus

$$
u(x)=\mathbb E_x[e^{-\lambda\tau}g(X_\tau)\mathbf1_{\{\tau<\infty\}}].
$$

Boundedness justifies passage to the terminal expectation even if hitting is not almost surely finite.

## ↑ Ancestors (10)

1. [Feynman-Kac formula](feynman-kac-formula.md)
2. [Kolmogorov backward equation](kolmogorov-backward-equation.md)
3. [Stochastic differential equation](stochastic-differential-equation.md)
4. [Stochastic calculus](stochastic-calculus-split.md)
5. [Stochastic process](stochastic-process-split.md)
6. [Probability theory](probability-theory-split.md)
7. [Probability and statistics](probability-and-statistics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (2)

- [First-passage Laplace transform for Brownian motion with drift](first-passage-laplace-transform-for-brownian-motion-with-drift.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-25/6/d/solution.md)
