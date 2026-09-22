# Diffusion with hyperbolic tangent drift

↑ **Parent:** [Itô diffusion](ito-diffusion.md)

The scalar [stochastic differential equation](stochastic-differential-equation.md) $dX_t=\tanh X_t\,dt+dW_t$ has a pathwise unique global strong solution, since its coefficients are globally Lipschitz. The positive martingale $e^{t/2}/\cosh X_t$ gives a [Girsanov theorem](girsanov-theorem.md) change of measure under which $X_t-X_0$ is [Brownian motion](brownian-motion-split.md). For $X_0=x$, its transition density is

$$
p_t(x,z)=e^{-t/2}\frac{\cosh z}{\cosh x}(2\pi t)^{-1/2}e^{-(z-x)^2/(2t)}.
$$

This is a [Doob h-transform](doob-h-transform.md) with $h=\cosh$, and a mixture of $N(x+t,t)$ and $N(x-t,t)$ with weights $e^x/(2\cosh x)$ and $e^{-x}/(2\cosh x)$.

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

## ← Incoming links (2)

- [Binary Brownian drift filter](binary-brownian-drift-filter.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-25/4/d/solution.md)
