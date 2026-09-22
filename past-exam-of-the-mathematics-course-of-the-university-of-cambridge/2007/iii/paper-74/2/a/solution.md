<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\mu=\langle X\rangle$. The [Markov jump-process generator](../../../../../../markov-jump-process-generator.md) applied to $X$ gives the exact [moment equation](../../../../../../moment-equation.md) $\dot\mu=3\lambda-\beta\langle\sqrt X\rangle$. With the prescribed [moment closure](../../../../../../moment-closure.md), $\langle\sqrt X\rangle\approx\sqrt\mu$, stationarity gives

$$
\boxed{\mu\approx\left(\frac{3\lambda}{\beta}\right)^2.}
$$

The production flux counts molecules, not reaction events: it is $v^+=3\lambda$, while the removal flux is $v^-=\beta\sqrt\mu=3\lambda$. The [reaction-rate elasticity](../../../../../../reaction-rate-elasticity.md) of removal relative to constant production is

$$
H=\frac{\partial\log v^-}{\partial\log\mu}-\frac{\partial\log v^+}{\partial\log\mu}=\frac12.
$$

The [mean molecular lifetime](../../../../../../mean-molecular-lifetime.md) is population divided by its stationary molecular removal flux. Therefore

$$
\boxed{H=\frac12,\qquad \tau=\frac{\mu}{\beta\sqrt\mu}=\frac{\mu}{3\lambda}\approx\frac{3\lambda}{\beta^2}.}
$$

The noise-relevant average chemical event size is the [molecular-flux-weighted reaction event size](../../../../../../molecular-flux-weighted-reaction-event-size.md). For the [stoichiometric vectors](../../../../../../stoichiometric-vector.md) $+3$ and $-1$ it is

$$
\langle s\rangle=\frac{3^2\lambda+(-1)^2\beta\sqrt\mu}{3\lambda+\beta\sqrt\mu}
=\frac{9\lambda+3\lambda}{3\lambda+3\lambda}
=\boxed{2.}
$$

This weights each absolute jump by the molecular turnover it contributes. Equivalently, the balanced production and removal fluxes give equal weight to their sizes $3$ and $1$, yielding $(3+1)/2$. An event-count-weighted average would be $3/2$, since three quarters of firing events are deaths at stationarity; that different average does not determine the diffusion term in the [linear noise approximation](../../../../../../linear-noise-approximation.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
