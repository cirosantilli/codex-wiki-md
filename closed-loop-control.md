# Closed-loop control

↑ **Parent:** [Control theory](control-theory-split.md)

[Feedback control](closed-loop-control.md) selects a [control input](control-input.md) using observations of the actual [controlled plant](plant-control-theory.md). In a tracking loop, compare the [reference signal](reference-signal.md) $r$ with the [measured output](measured-output.md) $y_m$ to form the [tracking error](tracking-error.md) $e=r-y_m$, then let the [controller](controller-control-theory.md) change $u$. The [control input](control-input.md) changes the [plant output](output-control-theory.md), which is measured again: that return path closes the loop. A [controller](controller-control-theory.md) can use earlier observations as well as the latest one. [Åström and Murray, Feedback Systems, Chapter 2: Feedback Principles](https://www.fbswiki.org/wiki/index.php/Feedback_Principles)

For the ideal [controlled plant](plant-control-theory.md), [proportional control](proportional-control.md) $u=2(1-x)$ initially commands $u(0)=2$. As $x$ approaches $1$, the command shrinks. When a positive [control disturbance](control-disturbance.md) pushes $x$ above $1$, the [tracking error](tracking-error.md) becomes negative and the [control input](control-input.md) pushes back. The result is a bounded offset rather than the continuing drift of [open-loop control](open-loop-control.md). [Integral action](integral-action.md) can remove that offset by remembering past [tracking errors](tracking-error.md).

A control selected from the observed current state, rather than specified only as a function of the initial state and time. For $x_{t+1}=x_t+u_t$ and stage cost $x_t^2+2x_tu_t+7u_t^2$, the infinite-horizon feedback $u_t=-x_t/3$ gives $x_t=(2/3)^tx_0$ and total cost $2x_0^2$. The finite-horizon Bellman coefficients satisfy $\Pi_0=0$, $\Pi_s=6(1+\Pi_{s-1})/(7+\Pi_{s-1})$ and increase to two, proving optimality.

**Table of contents**

- [Reference signal](reference-signal.md)
  - [Ramp reference signal](ramp-reference-signal.md)
- [Tracking error](tracking-error.md)
  - [Steady-state tracking error](steady-state-tracking-error.md)
- [Proportional control](proportional-control.md)
- [Integral action](integral-action.md)
  - [Proportional-integral control](proportional-integral-control.md)
- [Feedback delay](feedback-delay.md)
  - [Initial history of delayed feedback](initial-history-of-delayed-feedback.md)
  - [Delay stability of proportional integrator control](delay-stability-of-proportional-integrator-control.md)
  - [Delayed cursor feedback experiment](delayed-cursor-feedback-experiment.md)
- [Measurement-based quantum feedback](measurement-based-quantum-feedback.md)
  - [Qubit stabilization by measurement feedback](qubit-stabilization-by-measurement-feedback.md)

## ↑ Ancestors (4)

1. [Control theory](control-theory-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Adaptive experimental quantum control](adaptive-experimental-quantum-control.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-52/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-3/28k/solution.md)
