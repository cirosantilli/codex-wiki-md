# Reference signal

↑ **Parent:** [Closed-loop control](closed-loop-control.md)

A [reference signal](reference-signal.md) $r(t)$ specifies the desired physical [plant output](output-control-theory.md) as a function of [time](time-in-physics.md). A fixed [reference signal](reference-signal.md) is often called a setpoint; a changing [reference signal](reference-signal.md) describes a trajectory to follow. A [reference signal](reference-signal.md) is a goal, whereas the [control input](control-input.md) $u(t)$ is the command chosen to achieve that goal. [Jeffrey Kantor, Practical Proportional and Proportional-Integral Control, nomenclature and sign conventions](https://jckantor.github.io/cbe30338-book/notebooks/03.06-Proportional-Integral-Control.html)

Asking for a [temperature](temperature.md) of $40\,{}^\circ\mathrm C$ does not specify a heater command of $40\%$: [dimensional analysis](dimensional-analysis.md) distinguishes the units of these quantities. The [reference signal](reference-signal.md) and the [measured output](measured-output.md) must describe the same quantity in the same coordinates before their difference can define a [tracking error](tracking-error.md). An unconverted sensor readout cannot be subtracted directly from a desired [temperature](temperature.md).

For example, let $y=T-T_0$ be [temperature](temperature.md) rise above a fixed ambient baseline $T_0$, and write the desired [temperature](temperature.md) as $T_d=T_0+r$. A [Heaviside step function](heaviside-step-function.md) gives $r(t)=R$ for $t\ge0$, with $r(t)=0$ before the change: the target rise becomes $R$ at once, although a physical [controlled plant](plant-control-theory.md) generally cannot jump at once. A [ramp reference signal](ramp-reference-signal.md) $r(t)=vt$ instead asks the [temperature](temperature.md) rise to increase at a fixed rate $v$. If $R=1\,{}^\circ\mathrm C$ and $v=0.2\,{}^\circ\mathrm C\,\mathrm s^{-1}$, the first [reference signal](reference-signal.md) asks for a lasting one-degree rise; the second asks for a one-degree rise at $t=5\,\mathrm s$ and a two-degree rise at $t=10\,\mathrm s$. Here [degree Celsius](degree-celsius.md) differences are also [kelvin](kelvin.md) differences. A target that grows forever is useful for analytical tests but eventually exceeds a real heater's range.

To make the distinction between a goal and a command concrete, the examples in [steady-state tracking error](steady-state-tracking-error.md) use the [first-order low-pass filter](first-order-low-pass-filter.md) as a new [controlled plant](plant-control-theory.md), rather than the accumulating [controlled plant](plant-control-theory.md) $\dot x=u+w$ used in the earlier feedback demonstration:

$$
\tau\dot y+y=Ku+d,\qquad \tau>0,\quad K>0.
$$

The [time constant](time-constant.md) $\tau$ has units of [time](time-in-physics.md), $K$ has units of [plant output](output-control-theory.md) per [control input](control-input.md), and the additive [control disturbance](control-disturbance.md) $d$ has the units of $y$. This $d$ is an equivalent output offset, not the rate-like $w$ in $\dot x=u+w$. A heater interpretation uses $y$ in [degree Celsius](degree-celsius.md) differences and $u$ in percentage points of heater command, with $K$ in degrees per percentage point; the [control input](control-input.md) is a command, not a direct measurement of delivered power. With exact measurement, holding $y=R$ requires $u=(R-d)/K$. Thus even a constant [reference signal](reference-signal.md) can require a persistent nonzero [control input](control-input.md). The numerical model below is deliberately synthetic and has no fitted laboratory parameters.

**Table of contents**

- [Ramp reference signal](ramp-reference-signal.md)

## ↑ Ancestors (5)

1. [Closed-loop control](closed-loop-control.md)
2. [Control theory](control-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (11)

- [Closed-loop control](closed-loop-control.md)
- [Control theory](control-theory-split.md)
- [Feedback delay](feedback-delay.md)
- [Open-loop control](open-loop-control.md)
- [Physiological set point](physiological-set-point.md)
- [Proportional control](proportional-control.md)
- [Proportional-integral control](proportional-integral-control.md)
- [Ramp reference signal](ramp-reference-signal.md)
- [Reference signal](reference-signal.md)
- [Steady-state tracking error](steady-state-tracking-error.md)
- [Tracking error](tracking-error.md)
