# Uniform-quantization error bound

↑ **Parent:** [Quantization (signal processing)](quantization-signal-processing.md)

Rounding a voltage to the nearest level in a uniform grid of spacing $q$ gives a [quantization](quantization-signal-processing.md) error of magnitude at most $q/2$, provided the input is within the converter's range. This follows because each grid point represents the interval bounded by the midpoints to its two neighbors. Clipping invalidates the bound.

The bound concerns recorded samples, whereas the [Nyquist–Shannon sampling theorem](nyquist-shannon-sampling-theorem.md) concerns reconstruction from exact samples of a [bandlimited function](bandlimited-function.md). If a reconstruction is $\widetilde v(t)=\sum_n Q_q(v_n)w_n(t)$, its error is $\sum_n\epsilon_nw_n(t)$, so a general bound involves $(q/2)\sum_n|w_n(t)|$, not simply $q/2$. Thus sampling bandwidth and per-sample rounding precision are distinct specifications. Under an additional uniform independent-error model, the quantization-noise [standard deviation](standard-deviation.md) is $q/\sqrt{12}$, an rms statement rather than a worst-case reconstruction guarantee.

## ↑ Ancestors (4)

1. [Quantization (signal processing)](quantization-signal-processing.md)
2. [Image processing](image-processing.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Analog-to-digital converter](analog-to-digital-converter.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-1/section-d/d13/c/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2021/paper-1/section-a/5/solution.md)
