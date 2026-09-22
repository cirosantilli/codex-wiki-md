# Forecast horizon

↑ **Parent:** [Butterfly effect](butterfly-effect.md)

A forecast horizon is the duration over which a prediction meets a specified error tolerance. If an initial uncertainty $\varepsilon_0$ grows approximately as $\varepsilon_0e^{\lambda n}$ with positive [Lyapunov exponent](lyapunov-exponent.md) $\lambda$, then solving for when it reaches a tolerance $\Delta$ gives the displayed estimate. Here $\log$ is the [natural logarithm](natural-logarithm.md) and $\lambda$ is measured per step of the [discrete dynamical system](discrete-dynamical-system.md); for a [flow map](flow-map.md), use the exponent per unit [time](time-in-physics.md) instead. The estimate assumes the growth approximation remains valid up to the chosen tolerance and excludes additional model errors.

Reducing $\varepsilon_0$ by a factor ten buys approximately $(\log10)/\lambda$ more steps, rather than multiplying the forecast duration by ten. For typical [logistic map](logistic-map.md) [orbits](orbit-dynamical-system.md) at $r=4$, $\lambda=\log2$, so one extra decimal digit buys roughly $3.32$ steps in this approximation. Better measurements help, but their benefit is logarithmic. A forecast of a [probability distribution](probability-distribution.md) or a stable long-term average asks a different question from predicting each individual state.

## ↑ Ancestors (6)

1. [Butterfly effect](butterfly-effect.md)
2. [Devaney chaos](devaney-chaos.md)
3. [Dynamical systems](dynamical-systems-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Weather forecasting](weather-forecasting.md)
