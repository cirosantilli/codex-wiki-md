# Damping measurement from free decay

↑ **Parent:** [Damping](damping.md)

An experimentally useful question is whether the disappearing [oscillation](oscillation.md) follows [viscous damping](viscous-damping.md), and whether increasing the brake changes $b$ rather than $m$ or $k$. A published teaching protocol uses a cart on an [air track](air-track.md), attached between two [springs](spring.md), with ceramic magnets providing [eddy-current damping](eddy-current-damping.md) and an [ultrasonic motion sensor](ultrasonic-motion-sensor.md) recording [position](position.md) against [time](time-in-physics.md). Replace the magnets with equal [masses](mass.md) in the baseline trial so the moving [mass](mass.md) stays fixed. Obtain each [spring constant](spring-constant.md) from the slope of applied [force](force.md) versus extension, then use $k=k_1+k_2$. Time many baseline cycles to check $\omega_0\simeq\sqrt{k/m}$. Compare one-magnet and two-magnet free decays; the protocol calls for a fit of the full trace including its offset. [Driven Harmonic Oscillator](driven-harmonic-oscillator.md)

The following additional controls make the inference testable. Level the [air track](air-track.md) and hold its air supply fixed. Check the [ultrasonic motion sensor](ultrasonic-motion-sensor.md) at several stationary flag positions against a ruler, including the full planned travel range; record the offset and scale correction. Check elapsed acquisition [time](time-in-physics.md) against an independent clock, and choose a [sampling rate](sampling-rate.md) that resolves many samples within the shortest expected [oscillation period](period-of-an-oscillation.md). Record the resting [equilibrium](equilibrium-point-of-a-dynamical-system.md) before and after each run. Release the cart from a small measured [displacement](displacement.md) with minimal initial [velocity](velocity.md), with the driving apparatus inactive. Repeat at several release sizes and magnet settings while keeping the [springs](spring.md) and total [mass](mass.md) unchanged. These are proposed calibration and repeatability checks, not reported measurements from the source.

For [underdamping](underdamping.md), fit the recorded [position](position.md) to $y(t)=y_{\mathrm{eq}}+Ae^{-\alpha t}\cos(\omega_{\mathrm d}t+\phi)$ by [nonlinear regression](nonlinear-regression.md). The readout to inspect is a sequence of alternating extrema about $y_{\mathrm{eq}}$ with shrinking [amplitudes](wave-amplitude.md), and the deviations of the fitted curve from the recorded points. The model predicts

$$
\alpha=\frac{b}{2m}=\zeta\omega_0,\qquad
\alpha^2+\omega_{\mathrm d}^2=\frac{k}{m}.
$$

Compare the right-hand side, determined independently from [mass](mass.md) and [spring constants](spring-constant.md), with the fitted left-hand side. A good fit supports a constant-coefficient single [normal mode](normal-mode.md) over the observed range; it does not establish a universal microscopic [force](force.md) law. The published protocol denotes the decay rate by $b$ and the [velocity](velocity.md)-proportional coefficient by $c$; here they are $\alpha$ and $b$, respectively.

At [critical damping](critical-damping.md) or [overdamping](overdamping.md), fit the corresponding nonoscillatory response including its offset and both [initial conditions](initial-condition.md), rather than forcing a damped cosine onto the data. Adjusting the brake can explore the transition, but the cited protocol does not establish that its one-magnet or two-magnet settings attain [critical damping](critical-damping.md). A near-critical trace over a short interval can be hard to distinguish from neighbouring [damping ratios](damping-ratio.md).

Important limitations are finite sensor range, missed or reflected [acoustic wave](acoustic-wave.md) pulses, [measurement noise](measurement-noise.md) near [equilibrium](equilibrium-point-of-a-dynamical-system.md), nonzero release [velocity](velocity.md), and position-dependent magnetic braking. Changing the release size tests for [quadratic drag](quadratic-drag.md) or nonlinear [spring](spring.md) response; inspecting deviations near turning points can expose [kinetic friction](kinetic-friction.md). Slow drift of the offset can imitate a long [overdamped](overdamping.md) tail. Report uncertainties in fitted rates and independently measured $m,k$; absence of a visible crossing only bounds the behaviour within the instrument's sensitivity and recording interval. No numerical experimental results are asserted here.

**Table of contents**

- [Air track](air-track.md)
- [Ultrasonic motion sensor](ultrasonic-motion-sensor.md)
- [Logarithmic decrement](logarithmic-decrement.md)

## ↑ Ancestors (7)

1. [Damping](damping.md)
2. [Wave equation](wave-equation-split.md)
3. [Partial differential equation](partial-differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
