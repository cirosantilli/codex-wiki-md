# Low-pass filter

↑ **Parent:** [Linear filter](linear-filter.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Low-pass_filter)

A low-pass filter preferentially transmits low [frequencies](frequency.md) and attenuates higher [frequencies](frequency.md). It can smooth rapid [noise](noise-signal-processing.md) in a slowly varying [signal](signal.md), but it also suppresses wanted variations outside the useful [signal bandwidth](signal-bandwidth.md). An [RC low-pass filter](rc-low-pass-filter.md) gives a concrete continuous-time example; a [moving average](moving-average.md) implements related smoothing on a [discrete-time signal](discrete-time-signal.md).

The useful question is how much change the measurement can tolerate. Preserving the low [frequencies](frequency.md) of a temperature record while reducing a fast unwanted oscillation can improve readability. Preserving the sharp onset of a pulse requires higher [frequencies](frequency.md), so excessive smoothing changes its timing and shape. The [RC low-pass frequency response](rc-low-pass-frequency-response.md) and [RC low-pass step response](rc-low-pass-step-response.md) make this [signal bandwidth](signal-bandwidth.md) versus [settling time](settling-time.md) tradeoff quantitative.

**Table of contents**

- [Butterworth filter](butterworth-filter.md)
- [Sallen-Key low-pass filter](sallen-key-low-pass-filter.md)
  - [Sallen-Key equal-component stability bound](sallen-key-equal-component-stability-bound.md)
- [RL low-pass filter](rl-low-pass-filter.md)
- [RC low-pass filter](rc-low-pass-filter.md)
  - [RC low-pass frequency response](rc-low-pass-frequency-response.md)
  - [RC low-pass step response](rc-low-pass-step-response.md)
  - [RC low-pass output loading](rc-low-pass-output-loading.md)
  - [RC low-pass laboratory](rc-low-pass-laboratory.md)

## ↑ Ancestors (4)

1. [Linear filter](linear-filter.md)
2. [Signal processing](signal-processing.md)
3. [Electrical engineering](electrical-engineering-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (14)

- [Amplitude modulation laboratory](amplitude-modulation-laboratory.md)
- [Coherent demodulation](coherent-demodulation.md)
- [Discrete-jump model of Barkhausen noise](discrete-jump-model-of-barkhausen-noise.md)
- [Filtered shot noise](filtered-shot-noise.md)
- [Finite-window lock-in response](finite-window-lock-in-response.md)
- [Inductive Barkhausen experiment](inductive-barkhausen-experiment.md)
- [Inverting low-pass amplifier](inverting-low-pass-amplifier.md)
- [Lock-in amplifier](lock-in-amplifier.md)
- [Martinis-Devoret-Clarke circuit experiments](martinis-devoret-clarke-circuit-experiments.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2014/paper-1/section-d/d13/b/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2017/paper-1/section-d/d13/a/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1/section-b/b2/solution.md)
- [RL low-pass filter](rl-low-pass-filter.md)
- [Shot noise worked example](shot-noise-worked-example.md)
