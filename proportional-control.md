# Proportional control

↑ **Parent:** [Closed-loop control](closed-loop-control.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Proportional_control)

[Proportional control](proportional-control.md) chooses a [control input](control-input.md) proportional to the current [tracking error](tracking-error.md). For the ideal [controlled plant](plant-control-theory.md) and constant [reference signal](reference-signal.md) $r$, its [ordinary differential equation](ordinary-differential-equation.md) is $\dot x=k(r-x)+w$. With $w=0$ and [initial condition](initial-condition.md) $x(0)=x_0$, the exact response is

$$
x(t)=r+(x_0-r)e^{-kt}.
$$

For $r=1$, $x_0=0$ and $k=2$, this gives $x(1)=1-e^{-2}\simeq0.864665$ and $x(2)=1-e^{-4}\simeq0.981684$. To verify the formula, substitute it into the [ordinary differential equation](ordinary-differential-equation.md) and check the [initial condition](initial-condition.md); its decaying [exponential function](exponential-function.md) explains the approach to the goal.

With a constant [control disturbance](control-disturbance.md), setting $\dot x=0$ gives the [equilibrium point](equilibrium-point-of-a-dynamical-system.md) $x_*=r+w/k$ and [steady-state tracking error](steady-state-tracking-error.md) $e_*=-w/k$. For $w=0.2$, doubling the [feedback gain](feedback-gain.md) from $k=2$ to $k=4$ reduces the offset from $0.1$ to $0.05$. This improvement is a statement about the ideal model: it neglects [feedback delay](feedback-delay.md) and [measurement noise](measurement-noise.md), so it does not establish that arbitrarily large [feedback gains](feedback-gain.md) are safe. [Åström and Murray, Chapter 1: feedback benefits and drawbacks](https://www.fbswiki.org/wiki/index.php/Introduction)

In the first diagram's switched [control disturbance](control-disturbance.md) experiment, $k=2$ and $w=0.2$ from $t=2$ give, for $t\ge2$,

$$
x(t)=1.1+(1-e^{-4}-1.1)e^{-2(t-2)}.
$$

Thus $x(4)\simeq1.097833$ and $x(8)\simeq1.099999$. At the [equilibrium point](equilibrium-point-of-a-dynamical-system.md), the [controller](controller-control-theory.md) supplies $u=-0.2$ to cancel the [control disturbance](control-disturbance.md). [Proportional control](proportional-control.md) needs a nonzero [tracking error](tracking-error.md) to produce that persistent correction.

## ↑ Ancestors (5)

1. [Closed-loop control](closed-loop-control.md)
2. [Control theory](control-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (11)

- [Closed-loop control](closed-loop-control.md)
- [Control theory](control-theory-split.md)
- [Delay stability of proportional integrator control](delay-stability-of-proportional-integrator-control.md)
- [Feedback delay](feedback-delay.md)
- [Feedback gain](feedback-gain.md)
- [Homeostatic temperature model](homeostatic-temperature-model.md)
- [PID controller](pid-controller.md)
- [Proportional control](proportional-control.md)
- [Proportional-integral control](proportional-integral-control.md)
- [Steady-state tracking error](steady-state-tracking-error.md)
- [Tracking error](tracking-error.md)
