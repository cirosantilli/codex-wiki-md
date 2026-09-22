# Bounded-input bounded-output stability

↑ **Parent:** [Transfer function](transfer-function.md)

[Bounded-input bounded-output stability](bounded-input-bounded-output-stability.md) means that every bounded [plant input](input-control-theory.md) produces a bounded [plant output](output-control-theory.md) from zero initial state. For a causal continuous-time [linear time-invariant system](linear-time-invariant-system.md) with a [proper rational transfer function](proper-rational-transfer-function.md), [BIBO stability](bounded-input-bounded-output-stability.md) is equivalent to every [pole](pole.md) of the reduced [transfer function](transfer-function.md) having strictly negative [real part](real-part.md). Cancel common factors first: an apparent denominator root may be absent from the reduced [transfer function](transfer-function.md). For $K/(\tau s+1)$ with $\tau>0$, the only [pole](pole.md) is $-1/\tau$, so the [first-order low-pass filter](first-order-low-pass-filter.md) is [BIBO stable](bounded-input-bounded-output-stability.md). [Dahleh, Dahleh and Verghese, section 15.3.1 and example 15.5: input/output versus internal stability](https://ocw.mit.edu/courses/6-241j-dynamic-systems-and-control-spring-2011/996025f6db0d90b00f11c44fc49b85f9_MIT6_241JS11_textbook.pdf)

Internal [asymptotic stability](asymptotic-stability.md) also requires every unforced internal state to decay. A canceled factor can hide a growing internal state. For example, consider the [linear system of ordinary differential equations](linear-system-of-differential-equations.md)

$$
\dot x_1=-x_1+u,\qquad \dot x_2=x_2+u,\qquad y=x_1.
$$

Its zero-state [transfer function](transfer-function.md) can be written $(s-1)/((s+1)(s-1))=1/(s+1)$ and has [BIBO stability](bounded-input-bounded-output-stability.md). Yet from zero [initial conditions](initial-condition.md) and a unit-step [plant input](input-control-theory.md), $x_2(t)=e^t-1$ grows without bound while the [plant output](output-control-theory.md) remains bounded. The reduced [transfer function](transfer-function.md) conceals that second state. Even a [transfer function](transfer-function.md) with no visible cancellations can be implemented with additional hidden states; its [poles](pole.md) alone do not establish internal [asymptotic stability](asymptotic-stability.md) of an arbitrary implementation.

## ↑ Ancestors (5)

1. [Transfer function](transfer-function.md)
2. [Control theory](control-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Bounded-input bounded-output stability](bounded-input-bounded-output-stability.md)
