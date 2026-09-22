# Finite impulse response

↑ **Parent:** [Linear filter](linear-filter.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Finite_impulse_response)

A [linear time-invariant system](linear-time-invariant-system.md) has finite impulse response when its [impulse response](impulse-response.md) is nonzero at only finitely many indices. For a [causal filter](causal-filter.md) supported at indices $0,\ldots,M-1$,

$$
y[n]=\sum_{j=0}^{M-1}h[j]x[n-j].
$$

This is a finite [discrete convolution](discrete-convolution.md). The coefficients $h[j]$ specify the complete operation; they need not be positive or equal. Such a filter has a simple bounded-input estimate, $|y[n]|\leq\|x\|_\infty\sum_j|h[j]|$, so bounded inputs remain bounded. The [moving average](moving-average.md) chooses $h[j]=1/M$.

**Table of contents**

- [Moving average](moving-average.md)

## ↑ Ancestors (4)

1. [Linear filter](linear-filter.md)
2. [Signal processing](signal-processing.md)
3. [Electrical engineering](electrical-engineering-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Impulse response](impulse-response.md)
- [Linear filter](linear-filter.md)
- [Moving average](moving-average.md)
