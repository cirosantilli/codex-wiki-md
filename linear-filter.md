# Linear filter

↑ **Parent:** [Signal processing](signal-processing.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linear_filter)

A linear filter obeys the [superposition principle](superposition-principle.md): filtering $\alpha x+\beta z$ gives $\alpha T[x]+\beta T[z]$. Many familiar examples are also [linear time-invariant systems](linear-time-invariant-system.md), represented by an [impulse response](impulse-response.md) and [convolution](convolution.md). Linearity alone does not imply time invariance: multiplying $x[n]$ by the index $n$ is linear but changes its behavior when the same input is shifted.

The [moving average](moving-average.md) is a [finite impulse response](finite-impulse-response.md) example implemented by arithmetic; a [band-pass filter](band-pass-filter.md) can instead be built from a [series RLC circuit](series-rlc-circuit.md). Their [frequency responses](frequency-response.md) explain which oscillations pass through. Choosing a filter means choosing how much amplitude, timing and detail may change, not simply removing every visible fluctuation.

**Table of contents**

- [Causal filter](causal-filter.md)
- [Finite impulse response](finite-impulse-response.md)
  - [Moving average](moving-average.md)
- [Band-pass filter](band-pass-filter.md)

## ↑ Ancestors (3)

1. [Signal processing](signal-processing.md)
2. [Electrical engineering](electrical-engineering-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Noise (signal processing)](noise-signal-processing.md)
- [Signal processing](signal-processing.md)
