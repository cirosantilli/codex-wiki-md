# First-order low-pass filter

↑ **Parent:** [Transfer function](transfer-function.md)

A [first-order low-pass filter](first-order-low-pass-filter.md) with positive constant gain $K$ and [time constant](time-constant.md) $\tau>0$ obeys the [ordinary differential equation](ordinary-differential-equation.md)

$$
\tau y'(t)+y(t)=Ku(t).
$$

The [derivative](derivative.md) term limits how quickly the [plant output](output-control-theory.md) follows a changing [plant input](input-control-theory.md). A larger [time constant](time-constant.md) means slower adjustment. This standard form, with $K=1$, is developed in [Derek Rowell, MIT 2.004, lecture 20, section 1.1: first-order systems](https://www.ocw.mit.edu/courses/2-004-dynamics-and-control-ii-spring-2008/2cd1d6082fe3ba8a6a37fae62b10051f_lecture_20.pdf); the following calculation keeps the gain $K$ explicit.

Write $y_0=y(0)$. The [Laplace transform](laplace-transform.md) of the [derivative](derivative.md) is $sY(s)-y_0$, so

$$
\tau\bigl(sY(s)-y_0\bigr)+Y(s)=KU(s),\qquad
Y(s)=\frac{K}{\tau s+1}U(s)+\frac{\tau y_0}{\tau s+1}.
$$

Setting the [initial condition](initial-condition.md) $y_0=0$ gives the [transfer function](transfer-function.md) $G(s)=K/(\tau s+1)$. Its single [simple pole](simple-pole.md) is $s=-1/\tau$, which has negative [real part](real-part.md). The unforced response decays, and the input/output map has [BIBO stability](bounded-input-bounded-output-stability.md). The eventual gain for a constant [plant input](input-control-theory.md) is $G(0)=K$.

For a unit step, represented by the [Heaviside step function](heaviside-step-function.md) $u(t)=H(t)$, the [Laplace transform](laplace-transform.md) is $U(s)=1/s$. From zero [initial condition](initial-condition.md),

$$
Y(s)=\frac{K}{s(\tau s+1)}
=\frac Ks-\frac K{s+1/\tau},\qquad
y(t)=K\bigl(1-e^{-t/\tau}\bigr)\quad(t\ge0).
$$

Take $K=2$ and $\tau=3\,\mathrm{s}$, with dimensionless [plant input](input-control-theory.md) and [plant output](output-control-theory.md). Then $y(t)=2(1-e^{-t/(3\,\mathrm{s})})$ rises toward $2$. After one [time constant](time-constant.md), at $t=3\,\mathrm{s}$, it reaches $2(1-e^{-1})\approx1.2642$, or $63.2\%$ of its final value. At $t=9\,\mathrm{s}=3\tau$, it reaches $2(1-e^{-3})\approx1.9004$, or $95.0\%$. These percentages describe the rise from zero, rather than an instantaneous jump to the target.

With a nonzero [initial condition](initial-condition.md), the same step instead gives

$$
y(t)=K\bigl(1-e^{-t/\tau}\bigr)+y_0e^{-t/\tau}.
$$

For $K=2$ and $\tau=3\,\mathrm{s}$, compare $y_0=0$ with $y_0=1$. Their [plant outputs](output-control-theory.md) differ by $e^{-t/(3\,\mathrm{s})}$ despite having the same [transfer function](transfer-function.md) and the same [plant input](input-control-theory.md). The extra [exponential decay](exponential-decay.md) term must be supplied from the [initial condition](initial-condition.md); $G$ and $u$ alone cannot determine it.

<a id="image-one-transfer-function-one-unit-step-two-initial-conditions"></a>
![](first-order-transfer-step-response.png)

**[Figure 11](#image-one-transfer-function-one-unit-step-two-initial-conditions). One transfer function, one unit step, two initial conditions**. The [first-order low-pass filter](first-order-low-pass-filter.md) has $K=2$ and [time constant](time-constant.md) $\tau=3\,\mathrm{s}$. The blue curve starts at $y_0=0$ and the orange curve at $y_0=1$. The marked $63.2\%$ and $95.0\%$ levels refer to the blue curve's final value $2$; the two curves' difference is the decaying initial-state contribution.

## ↑ Ancestors (5)

1. [Transfer function](transfer-function.md)
2. [Control theory](control-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Bode plot](bode-plot.md)
- [Bounded-input bounded-output stability](bounded-input-bounded-output-stability.md)
- [Continuous-time frequency response](continuous-time-frequency-response.md)
- [First-order low-pass filter](first-order-low-pass-filter.md)
- [Reference signal](reference-signal.md)
- [Steady-state tracking error](steady-state-tracking-error.md)
- [Transfer function](transfer-function.md)
