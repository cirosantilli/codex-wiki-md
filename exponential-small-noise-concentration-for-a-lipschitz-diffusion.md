# Exponential small-noise concentration for a Lipschitz diffusion

↑ **Parent:** [Itô diffusion](ito-diffusion.md)

Couple $dX_t^\varepsilon=b(X_t^\varepsilon)dt+\varepsilon dW_t$ with $\dot x_t=b(x_t)$ and the same initial value. If $b$ has Lipschitz constant $L$, the [Gronwall inequality](gronwall-inequality.md) gives $\sup_{s\le t}|X_s^\varepsilon-x_s|\le\varepsilon e^{Lt}\sup_{s\le t}|W_s|$. Applying the [Gaussian maximal bound for Brownian motion](gaussian-maximal-bound-for-brownian-motion.md) coordinatewise in dimension $d$ bounds the deviation [probability](probability.md) by $2d\exp[-\delta^2e^{-2Lt}/(2dt\varepsilon^2)]$ for $t>0$. Matching initial values is essential.

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

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-31/4/solution.md)
