# Exact sampling of an Ornstein-Uhlenbeck process

↑ **Parent:** [Ornstein-Uhlenbeck process](ornstein-uhlenbeck-process.md)

For any step $\Delta>0$, set $a=e^{-\theta\Delta}$. The [Ornstein-Uhlenbeck transition distribution](ornstein-uhlenbeck-transition-distribution.md) gives the exact update

$$
X_{t+\Delta}=\mu+a(X_t-\mu)+\sqrt{\frac{\sigma^2}{2\theta}(1-a^2)}\,Z,\qquad Z\sim\mathcal N(0,1),
$$

using a fresh independent [standard normal random variable](standard-normal-random-variable.md) for each interval. The update reproduces the [joint probability distribution](joint-probability-distribution.md) on the selected time grid. It can start from a fixed value or use [Ornstein-Uhlenbeck stationary initialization](ornstein-uhlenbeck-stationary-initialization.md). On an equally spaced grid it is an [autoregressive process of order one](autoregressive-process-of-order-one.md) after subtracting $\mu$. Its stationary [variance](variance-split.md) follows directly from $v=a^2v+v_\infty(1-a^2)$.

For the stipulated example with $\Delta=0.1$, $a=e^{-0.1}\approx0.90484$ and the innovation [variance](variance-split.md) is $1-e^{-0.2}\approx0.18127$. Given $X_t=6$, the next [conditional expected value](conditional-expectation.md) is about $5.61935$ and the conditional [standard deviation](standard-deviation.md) is about $0.42576$.

The [Euler-Maruyama method](euler-maruyama-method.md) instead approximates the same [stochastic differential equation](stochastic-differential-equation.md) by

$$
X_{t+\Delta}^{\mathrm E}=\mu+(1-\theta\Delta)(X_t^{\mathrm E}-\mu)+\sigma\sqrt\Delta\,Z.
$$

For $0<\theta\Delta<2$ its stationary [variance](variance-split.md) solves $v=(1-\theta\Delta)^2v+\sigma^2\Delta$, giving

$$
v_{\mathrm E}=\frac{\sigma^2}{2\theta-\theta^2\Delta}=\frac{v_\infty}{1-\theta\Delta/2}.
$$

At $\Delta=0.1$ in the example, this is $1/0.95\approx1.05263$, about $5.26\%$ above the continuous model's stationary [variance](variance-split.md). If $\theta\Delta\ge2$, this Euler recurrence has no finite stationary [variance](variance-split.md) despite the stable continuous model. Exact transitions avoid this discretization error at sampled times; neither update alone determines the unresolved motion between samples.

## ↑ Ancestors (8)

1. [Ornstein-Uhlenbeck process](ornstein-uhlenbeck-process.md)
2. [Gaussian process](gaussian-process-split.md)
3. [Stochastic process](stochastic-process-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
