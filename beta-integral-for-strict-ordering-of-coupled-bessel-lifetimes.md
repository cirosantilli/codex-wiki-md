# Beta integral for strict ordering of coupled Bessel lifetimes

↑ **Parent:** [Bessel process](bessel-process.md)

Couple $dX=dB+aX^{-1}dt$ and $dY=dB+aY^{-1}dt$ from $0<x<y$, with $1/4<a<1/2$. Suppose their finite lifetimes end at zero and $\int_0^{\sigma_y}Y_t^{-2}dt=\infty$. Their difference is positive and has derivative $-a(Y-X)/(XY)$, so $\sigma_x\leq\sigma_y$. For $\Theta=(Y-X)/Y$, the [Itô formula](ito-s-lemma.md) gives

$$
d\Theta=-\Theta Y^{-1}dB+\Theta Y^{-2}\left(1-a-\frac a{1-\Theta}\right)dt.
$$

The normalized [scale function of a one-dimensional diffusion](scale-function-stochastic-processes.md) $I_\Theta(4a-1,1-2a)$ is a bounded [local martingale](local-martingale.md). Its finite [quadratic variation](quadratic-variation.md) and the divergent $Y^{-2}$ clock force $\Theta\to0$ on simultaneous extinction; on strict extinction $\Theta\to1$. Its terminal value is therefore the strict-extinction indicator, proving the formula by [optional sampling theorem](optional-sampling-theorem-for-a-supermartingale.md). For [SLE](schramm-loewner-evolution.md) boundary images, $a=2/\kappa$; this compares strict and simultaneous [boundary swallowing times](boundary-point-swallowing-time-for-a-loewner-chain.md) for $4<\kappa<8$.

## ↑ Ancestors (8)

1. [Bessel process](bessel-process.md)
2. [Brownian motion](brownian-motion-split.md)
3. [Stochastic process](stochastic-process-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Cardy boundary crossing formula](cardy-boundary-crossing-formula.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-27/3/solution.md)
