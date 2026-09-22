# Causal Green function of a damped oscillator

↑ **Parent:** [Damped harmonic oscillator](damped-harmonic-oscillator.md)

For $L=D_t^2+2kD_t+k^2+\omega^2$, with $k>0$ and $\omega>0$, the causal [Green function](green-s-function-split.md) is $G(t)=H(t)e^{-kt}\sin(\omega t)/\omega$, where $H$ is the [Heaviside step function](heaviside-step-function.md). It satisfies $LG=\delta(t)$: it is continuous at zero, with a unit jump in its first [derivative](derivative.md). Its smooth positive-time kernel $g$ obeys $g(0)=0,g'(0)=1$. The zero-frequency limit is $H(t)te^{-kt}$. Shifting $G$ gives the zero-initial-data response to a delayed [Dirac delta function](dirac-delta-function.md).

With the [Fourier transform](fourier-transform-split.md) convention $\widehat f(\xi)=\int f(t)e^{-i\xi t}\,dt$, the transformed equation gives $\widehat G(\xi)=[k^2+\omega^2-\xi^2+2ik\xi]^{-1}$. Its [poles](pole.md) $\xi=ik\pm\omega$ lie in the upper half of the [complex plane](complex-plane.md). Inverting by [contour integration](contour-integration.md) therefore gives zero for negative time and an exponentially damped oscillation for positive time.

**Table of contents**

- [Exponential forcing of an underdamped oscillator](exponential-forcing-of-an-underdamped-oscillator.md)
- [Decay of a damped oscillator under exponentially decaying forcing](decay-of-a-damped-oscillator-under-exponentially-decaying-forcing.md)
- [Step response of a damped oscillator](step-response-of-a-damped-oscillator.md)
  - [Added-load step response of a supported table](added-load-step-response-of-a-supported-table.md)
  - [Shift derivative of a step response](shift-derivative-of-a-step-response.md)

## ↑ Ancestors (5)

1. [Damped harmonic oscillator](damped-harmonic-oscillator.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (12)

- [Critical damping](critical-damping.md)
- [Decay of a damped oscillator under exponentially decaying forcing](decay-of-a-damped-oscillator-under-exponentially-decaying-forcing.md)
- [Exponential forcing of an underdamped oscillator](exponential-forcing-of-an-underdamped-oscillator.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-2/8a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-2/8a/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2005/paper-1/8/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-1/3/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-2/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-2/5/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2018/paper-2/5/d/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1/3/ii/solution.md)
- [Solution](past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2016/paper-1/3/d/solution.md)
