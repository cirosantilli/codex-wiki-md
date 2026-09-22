# Integral action

↑ **Parent:** [Closed-loop control](closed-loop-control.md)

[Integral action](integral-action.md) adds memory of the [tracking error](tracking-error.md) to a [controller](controller-control-theory.md): $z(t)=z(0)+\int_0^t e(s)\,ds$. A persistent [tracking error](tracking-error.md) keeps changing $z$, so an [equilibrium point](equilibrium-point-of-a-dynamical-system.md) with constant $z$ must have $e=0$. The accumulated value can remain nonzero after the [tracking error](tracking-error.md) has vanished, maintaining the [control input](control-input.md) needed to cancel a constant [control disturbance](control-disturbance.md). Convergence still requires a stable [feedback control](closed-loop-control.md) design. [Åström and Murray, Chapter 1: integral action](https://www.fbswiki.org/wiki/index.php/Introduction)

**Table of contents**

- [Proportional-integral control](proportional-integral-control.md)

## ↑ Ancestors (5)

1. [Closed-loop control](closed-loop-control.md)
2. [Control theory](control-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (14)

- [Actuator saturation](actuator-saturation.md)
- [Closed-loop control](closed-loop-control.md)
- [Controller (control theory)](controller-control-theory.md)
- [Effector saturation](effector-saturation.md)
- [Integral action](integral-action.md)
- [Solution](past-exam-of-the-systems-biology-course-of-the-university-of-cambridge/2024/paper-1/section-ii/2-1/solution.md)
- [Physiological integrator](physiological-integrator.md)
- [PID controller](pid-controller.md)
- [Proportional-integral control](proportional-integral-control.md)
- [Robust perfect adaptation](robust-perfect-adaptation.md)
- [Signaling adaptation](signaling-adaptation.md)
- [Signaling feedback](signaling-feedback.md)
- [Steady-state tracking error](steady-state-tracking-error.md)
- [Tracking error](tracking-error.md)
