# Initial history of delayed feedback

↑ **Parent:** [Feedback delay](feedback-delay.md)

For positive [feedback delay](feedback-delay.md) $\tau$, an [initial condition](initial-condition.md) at a single instant is insufficient. Prescribe a [continuous function](continuous-function.md) $\phi$ throughout $[-\tau,0]$: for $0\le t\le\tau$, the [derivative](derivative.md) depends on $x(t-\tau)=\phi(t-\tau)$. A right [derivative](derivative.md) at $t=0$ is understood; the earlier history need not itself obey the subsequent control law. Once this first interval is computed, it supplies the delayed values for the next interval. This successive integration is the method of steps for a [delay differential equation](delay-differential-equation.md). [John W. Cain and Angela M. Reynolds, Ordinary and Partial Differential Equations, sections 6.1 and 6.2: history and the method of steps](https://math1um.github.io/Teaching/cain-reynolds-odes.pdf#page=174)

For the constant [initial history of delayed feedback](initial-history-of-delayed-feedback.md) $\phi(t)=1$, direct [integration](integral.md) gives

$$
x(t)=1-kt\quad(0\le t\le\tau),\qquad
x(t)=1-kt+\frac{k^2}{2}(t-\tau)^2\quad(\tau\le t\le2\tau).
$$

For $k=1$, $\tau=1.2$, the [plant output](output-control-theory.md) crosses zero at $t=1$, while its [measured output](measured-output.md) remains positive until $t=2.2$. At $t=1.4$, the delayed command therefore increases the magnitude of the actual deviation. This short exact calculation explains the first diagram without relying on a numerical approximation.

## ↑ Ancestors (6)

1. [Feedback delay](feedback-delay.md)
2. [Closed-loop control](closed-loop-control.md)
3. [Control theory](control-theory-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Delay stability of proportional integrator control](delay-stability-of-proportional-integrator-control.md)
- [Feedback delay](feedback-delay.md)
- [Initial history of delayed feedback](initial-history-of-delayed-feedback.md)
