# Linear filter

↑ **Parent:** [Signal processing](signal-processing.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linear_filter)

A linear filter obeys the [superposition principle](superposition-principle.md): filtering $\alpha x+\beta z$ gives $\alpha T[x]+\beta T[z]$. Many familiar examples are also [linear time-invariant systems](linear-time-invariant-system.md), represented by an [impulse response](impulse-response.md) and [convolution](convolution.md). Linearity alone does not imply time invariance: multiplying $x[n]$ by the index $n$ is linear but changes its behavior when the same input is shifted.

The [moving average](moving-average.md) is a [finite impulse response](finite-impulse-response.md) example implemented by arithmetic; a [band-pass filter](band-pass-filter.md) can instead be built from a [series RLC circuit](series-rlc-circuit.md). Their [frequency responses](frequency-response.md) explain which oscillations pass through. Choosing a filter means choosing how much amplitude, timing and detail may change, not simply removing every visible fluctuation.

**Table of contents**

- [Relative attenuation by a linear filter](relative-attenuation-by-a-linear-filter.md)
- [Low-pass filter](low-pass-filter.md)
  - [Butterworth filter](butterworth-filter.md)
  - [Sallen-Key low-pass filter](sallen-key-low-pass-filter.md)
    - [Sallen-Key equal-component stability bound](sallen-key-equal-component-stability-bound.md)
  - [RL low-pass filter](rl-low-pass-filter.md)
  - [RC low-pass filter](rc-low-pass-filter.md)
    - [RC low-pass frequency response](rc-low-pass-frequency-response.md)
    - [RC low-pass step response](rc-low-pass-step-response.md)
    - [RC low-pass output loading](rc-low-pass-output-loading.md)
    - [RC low-pass laboratory](rc-low-pass-laboratory.md)
- [Causal filter](causal-filter.md)
- [Finite impulse response](finite-impulse-response.md)
  - [Moving average](moving-average.md)
- [Band-pass filter](band-pass-filter.md)
- [Cutoff frequency](cutoff-frequency.md)

## ↑ Ancestors (3)

1. [Signal processing](signal-processing.md)
2. [Electrical engineering](electrical-engineering-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Discrete-jump model of Barkhausen noise](discrete-jump-model-of-barkhausen-noise.md)
- [Effective noise bandwidth](effective-noise-bandwidth.md)
- [Filtered shot noise](filtered-shot-noise.md)
- [Noise (signal processing)](noise-signal-processing.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2015/paper-1/section-d/d13/c/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2017/paper-1/section-d/d12/solution.md)
- [Shot noise counting model](shot-noise-counting-model.md)
- [Signal processing](signal-processing.md)
