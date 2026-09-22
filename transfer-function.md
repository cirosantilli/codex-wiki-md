# Transfer function

↑ **Parent:** [Control theory](control-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Transfer_function)

A [transfer function](transfer-function.md) packages the response of a [linear time-invariant system](linear-time-invariant-system.md) into a rule for turning a [plant input](input-control-theory.md) into a [plant output](output-control-theory.md). Instead of solving a [differential equation](differential-equation-split.md) separately for every [signal](signal.md), take a [Laplace transform](laplace-transform.md), multiply by $G(s)$, then transform back. This also makes it possible to compare slow and fast oscillations through the [continuous-time frequency response](continuous-time-frequency-response.md).

Here consider a continuous-time, causal, finite-dimensional [linear time-invariant system](linear-time-invariant-system.md) with one [plant input](input-control-theory.md) $u(t)$ and one [plant output](output-control-theory.md) $y(t)$. With every initial state set to zero, its [transfer function](transfer-function.md) is defined by

$$
U(s)=\mathcal L\{u\}(s),\qquad Y(s)=\mathcal L\{y\}(s),\qquad Y(s)=G(s)U(s).
$$

The ratio $G(s)=Y(s)/U(s)$ is used where $U(s)\ne0$ in a common [Laplace convergence region](region-of-absolute-convergence-of-a-laplace-transform.md); $G$ describes the system, independently of that particular [plant input](input-control-theory.md). Zero initial state matters: stored motion or another nonzero [initial condition](initial-condition.md) can contribute to the [plant output](output-control-theory.md) even when the [plant input](input-control-theory.md) vanishes. [MIT 18.03SC, The Transfer Function: rest initial conditions and transformed input/output](https://ocw.mit.edu/courses/18-03sc-differential-equations-fall-2011/941349ccabc51e8c116a86db62ba6566_MIT18_03SCF11_s30_1text.pdf)

The [first-order low-pass filter](first-order-low-pass-filter.md) below shows the same [transfer function](transfer-function.md) predicting both a step and a sustained [sinusoid](sinusoid.md). Its [pole](pole.md) gives a decay rate, its value at zero gives the eventual gain, and its values along the imaginary axis give the [continuous-time frequency response](continuous-time-frequency-response.md). These descriptions make a useful bridge between a physical relaxation model and [control theory](control-theory-split.md) calculations.

**Table of contents**

- [Formal sinusoidal response of an unstable linear system](formal-sinusoidal-response-of-an-unstable-linear-system.md)
- [First-order low-pass filter](first-order-low-pass-filter.md)
- [Continuous-time frequency response](continuous-time-frequency-response.md)
  - [Bode plot](bode-plot.md)
- [Proper rational transfer function](proper-rational-transfer-function.md)
- [Bounded-input bounded-output stability](bounded-input-bounded-output-stability.md)
- [Nyquist stability criterion](nyquist-stability-criterion.md)
- [Step response](step-response.md)
  - [Settling time](settling-time.md)

## ↑ Ancestors (4)

1. [Control theory](control-theory-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (30)

- [Analysis of the Sallen-Key Architecture by James Karki](analysis-of-the-sallen-key-architecture-by-james-karki.md)
- [Base-excited oscillator](base-excited-oscillator.md)
- [Bounded-input bounded-output stability](bounded-input-bounded-output-stability.md)
- [Calibrated Einstein-de Haas torsion response](calibrated-einstein-de-haas-torsion-response.md)
- [Continuous-time frequency response](continuous-time-frequency-response.md)
- [First-order low-pass filter](first-order-low-pass-filter.md)
- [Formal sinusoidal response of an unstable linear system](formal-sinusoidal-response-of-an-unstable-linear-system.md)
- [High-pass filter](high-pass-filter.md)
- [Inverting two-pole band-pass filter](inverting-two-pole-band-pass-filter.md)
- [Operational amplifier](operational-amplifier.md)
- [Passive cavity input-output transfer function](passive-cavity-input-output-transfer-function.md)
- [Solution](past-exam-of-the-formation-of-structure-in-the-universe-course-of-the-university-of-cambridge/2012/paper-1/1/d/solution.md)
- [Solution](past-exam-of-the-formation-of-structure-in-the-universe-course-of-the-university-of-cambridge/2016/paper-1/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-60/5/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-3/6a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-2/5/b/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2012/paper-1/section-d/d12/b/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2012/paper-1/section-d/d13/c/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2012/paper-1/section-d/d13/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-1/section-a/a5/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-1/section-d/d12/b/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-1/section-d/d12/c/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-1/section-d/d12/e/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2019/paper-2/section-c/c13/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1/section-a/a3/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1/section-c/c11/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/section-a/6/solution.md)
- [Solution](past-exam-of-the-relativistic-astrophysics-and-cosmology-course-of-the-university-of-cambridge/2014/paper-1/3/b/solution.md)
- [Proper rational transfer function](proper-rational-transfer-function.md)
- [Transfer function](transfer-function.md)
