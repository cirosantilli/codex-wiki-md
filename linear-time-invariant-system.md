# Linear time-invariant system

↑ **Parent:** [Signal processing](signal-processing.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linear_time-invariant_system)

A linear time-invariant system combines two properties. [Linearity](linearity.md) means that the [output](output-computing.md) from a [linear combination](linear-combination.md) of inputs is the same [linear combination](linear-combination.md) of their outputs. Time invariance means that shifting an [input](input-computer-science.md) by an integer delay shifts its [output](output-computing.md) by exactly that delay. The operation has no preference for a particular time origin.

For discrete time, write the unit impulse as $\delta[n]=1$ at $n=0$ and zero otherwise, a [Kronecker delta](kronecker-delta.md). Its response $h[n]=T[\delta][n]$ is the [impulse response](impulse-response.md). A finite [input](input-computer-science.md) can be decomposed into shifted impulses, giving

$$
x[n]=\sum_kx[k]\delta[n-k]
\quad\Longrightarrow\quad
y[n]=\sum_kx[k]h[n-k]=(x*h)[n].
$$

The [superposition principle](superposition-principle.md) supplies the sum and time invariance supplies the shifted copies of $h$. Infinite sums need convergence assumptions; for a bounded input and an impulse response $h$ with [absolute summability](absolute-convergence.md), the [discrete convolution](discrete-convolution.md) converges absolutely. For a physical system with stored initial [energy](energy-split.md), this construction describes the response with zero initial state; a separate free response accounts for nonzero initial conditions.

The gain is reuse. Measure or calculate one [impulse response](impulse-response.md), and the [convolution](convolution.md) predicts the response to every allowed [signal](signal.md) without solving a new dynamical problem each time. Alternatively, the [frequency response](frequency-response.md) predicts how each oscillatory component changes. [Oppenheim, lecture 4: convolution from shifted impulses](https://ocw.mit.edu/courses/res-6-007-signals-and-systems-spring-2011/0400ba59406d52d94c079d99928156ee_MITRES_6_007S11_lec04.pdf).

**Table of contents**

- [Frequency response](frequency-response.md)
  - [Antiresonance](antiresonance.md)

## ↑ Ancestors (3)

1. [Signal processing](signal-processing.md)
2. [Electrical engineering](electrical-engineering-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (25)

- [Bounded-input bounded-output stability](bounded-input-bounded-output-stability.md)
- [Continuous-time frequency response](continuous-time-frequency-response.md)
- [Controllability](controllability.md)
- [Controllability matrix](controllability-matrix.md)
- [Convolution](convolution.md)
- [Convolution kernel](convolution-kernel.md)
- [Delay stability of proportional integrator control](delay-stability-of-proportional-integrator-control.md)
- [Double integrator](double-integrator.md)
- [Electrical impedance](electrical-impedance.md)
- [Filtered shot noise](filtered-shot-noise.md)
- [Finite impulse response](finite-impulse-response.md)
- [Fourier series](fourier-series-split.md)
- [Frequency response](frequency-response.md)
- [Impulse response](impulse-response.md)
- [Kalman rank criterion](kalman-rank-criterion.md)
- [Laplace transform](laplace-transform.md)
- [Linear filter](linear-filter.md)
- [Moving average](moving-average.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2010/paper-2a/section-d/d17/c/solution.md)
- [Proper rational transfer function](proper-rational-transfer-function.md)
- [Reachability in control theory](reachability-in-control-theory.md)
- [Relative attenuation by a linear filter](relative-attenuation-by-a-linear-filter.md)
- [Signal processing](signal-processing.md)
- [Thermal noise spectral convention](thermal-noise-spectral-convention.md)
- [Transfer function](transfer-function.md)
