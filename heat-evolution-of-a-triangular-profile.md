# Heat evolution of a triangular profile

↑ **Parent:** [Heat equation](heat-equation.md)

On the real line, let $T(x)=\max(1-|x|/2,0)$. The [Fourier transform of a triangular function](fourier-transform-of-a-triangular-function.md) gives $\widehat T(\omega)=2\sin^2\omega/\omega^2$, with value two at zero. The [Gaussian heat kernel](gaussian-heat-kernel.md) has transform $e^{-t\omega^2}$. Hence $u=q_t*T$ solves the [heat equation](heat-equation.md) with initial profile $T$, and the [inverse Fourier transform](inverse-fourier-transform.md) gives the displayed integral. Differentiating for positive time is justified by Gaussian decay. The [uniform continuity](uniform-continuity.md) of $T$ and the vanishing Gaussian mass outside any fixed neighborhood of zero prove uniform recovery of $T$ as $t\downarrow0$. Convolution preserves total integral two, keeps the solution nonnegative, and smooths the corners for every positive time. Unlike the finite-interval problem in [heat flow from a triangular initial temperature](heat-flow-from-a-triangular-initial-temperature.md), this evolution has no endpoints through which heat can escape.

## ↑ Ancestors (7)

1. [Heat equation](heat-equation.md)
2. [Diffusion equation](diffusion-equation-split.md)
3. [Partial differential equation](partial-differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-algebra-1-and-differential-equations-1-course-of-the-university-of-oxford/2014/6/e/ii/solution.md)
