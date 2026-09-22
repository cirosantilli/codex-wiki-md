# Periodic extension of a finite sequence

↑ **Parent:** [Discrete Fourier transform](discrete-fourier-transform-split.md)

A block $x_0,\ldots,x_{N-1}$ determines a repeating [sequence](sequence.md) by setting $x_n=x_{n\bmod N}$ for every [integer](integer-split.md) $n$. The [inverse discrete Fourier transform](inverse-discrete-fourier-transform.md) gives this extension because each [discrete Fourier mode](discrete-fourier-mode.md) satisfies $e^{2\pi ik(n+N)/N}=e^{2\pi ikn/N}$. The extension explains why [circular convolution](circular-convolution.md) wraps indices around the block. It specifies values at discrete indices; a continuous curve between samples requires an additional choice of [interpolation](interpolation-split.md).

## ↑ Ancestors (6)

1. [Discrete Fourier transform](discrete-fourier-transform-split.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Discrete Fourier transform](discrete-fourier-transform-split.md)
