# Regularized spectral deconvolution

↑ **Parent:** [Deconvolution](deconvolution.md)

[Tikhonov regularization](tikhonov-regularization.md) of [deconvolution](deconvolution.md) can minimize $|HF-G|^2+\lambda|F|^2$ separately at each [frequency](frequency.md). Completing the square gives $F_\lambda=H^*G/(|H|^2+\lambda)$ for $\lambda>0$. The [regularization parameter](regularization-parameter.md) trades reduced [noise](noise-signal-processing.md) amplification against bias: the reconstruction multiplies the true noiseless component by $|H|^2/(|H|^2+\lambda)$ and the [noise](noise-signal-processing.md) by $H^*/(|H|^2+\lambda)$.

## ↑ Ancestors (7)

1. [Deconvolution](deconvolution.md)
2. [Convolution](convolution.md)
3. [Fourier analysis](fourier-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2010/paper-2a/section-d/d17/c/solution.md)
