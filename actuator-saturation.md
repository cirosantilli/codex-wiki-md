# Actuator saturation

↑ **Parent:** [Controller (control theory)](controller-control-theory.md)

[Actuator saturation](actuator-saturation.md) means the applied [control input](control-input.md) reaches a device limit even if the [controller](controller-control-theory.md) requests a larger or smaller command. In the heater interpretation, the applied command is bounded between $0$ and $100\%$. If [integral action](integral-action.md) continues accumulating a persistent [tracking error](tracking-error.md) beyond that limit, its stored [integral](integral.md) can grow without producing the requested physical correction, delaying recovery when the goal changes. The unconstrained [steady-state tracking error](steady-state-tracking-error.md) formulas require that the necessary command can actually be applied. [Åström and Murray, PID Control: saturation and integral windup](https://www.fbswiki.org/wiki/index.php/PID_Control)

## ↑ Ancestors (5)

1. [Controller (control theory)](controller-control-theory.md)
2. [Control theory](control-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Actuator saturation](actuator-saturation.md)
- [Steady-state tracking error](steady-state-tracking-error.md)
- [Tracking error](tracking-error.md)
