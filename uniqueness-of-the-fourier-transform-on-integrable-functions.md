# Uniqueness of the Fourier transform on integrable functions

↑ **Parent:** [Fourier transform](fourier-transform-split.md)

For [integrable functions](lebesgue-integrable-function.md) on the real line, equality of their [Fourier transforms](fourier-transform-split.md) implies equality almost everywhere. To prove it, subtract and assume $\widehat h=0$. Convolve $h$ with a [Gaussian heat kernel](gaussian-heat-kernel.md) $q_t$. The [convolution theorem](convolution-theorem.md) gives $\widehat{h*q_t}=0$, which is integrable, so the [Fourier inversion theorem](fourier-inversion-theorem.md) gives $h*q_t=0$ almost everywhere. Finally $q_t$ is an [approximate identity](approximate-identity.md): $\|h*q_t-h\|_1\leq\int q_t(y)\|h(\cdot-y)-h\|_1dy\to0$. This follows from [translation continuity in Lp](translation-continuity-in-lp.md) with exponent one and the vanishing Gaussian tails. Hence $h=0$ in $L^1$. If the two original functions are continuous, equality almost everywhere strengthens to equality everywhere, since a nonzero continuous difference has magnitude bounded below by a positive constant on some interval.

## ↑ Ancestors (5)

1. [Fourier transform](fourier-transform-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-algebra-1-and-differential-equations-1-course-of-the-university-of-oxford/2014/6/d/solution.md)
