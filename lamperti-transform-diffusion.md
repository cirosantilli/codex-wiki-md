# Lamperti transform (diffusion)

↑ **Parent:** [Itô diffusion](ito-diffusion.md)

On an interval where $\sigma>0$ is continuously differentiable, define $F(x)=\int^x\sigma(y)^{-1}dy$. The [Itô formula](ito-s-lemma.md) transforms $dX=b(X)dt+\sigma(X)dB$ into

$$
dF(X_t)=dB_t+\left(\frac{b(X_t)}{\sigma(X_t)}-\frac12\sigma'(X_t)\right)dt.
$$

The transformed [Itô diffusion](ito-diffusion.md) has constant noise coefficient. For a [power diffusion](power-diffusion.md) $\sigma(x)=x^\alpha$, $F(x)=x^{1-\alpha}/(1-\alpha)$ when $\alpha\ne1$, and $F(x)=\log x$ when $\alpha=1$. This simplifies comparison with [Brownian motion](brownian-motion-split.md) and exposes the boundary drift.

## ↑ Ancestors (9)

1. [Itô diffusion](ito-diffusion.md)
2. [Stochastic differential equation](stochastic-differential-equation.md)
3. [Stochastic calculus](stochastic-calculus-split.md)
4. [Stochastic process](stochastic-process-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)
