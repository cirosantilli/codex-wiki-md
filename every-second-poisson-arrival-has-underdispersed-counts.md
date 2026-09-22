# Every second Poisson arrival has underdispersed counts

↑ **Parent:** [Poisson process](poisson-process.md)

For a rate-$\lambda$ [Poisson process](poisson-process.md), keeping every second arrival gives a renewal process with independent interarrival times equal to sums of two exponential waiting times. Put $x=\lambda t$. Its count mean and variance are $(2x+e^{-2x}-1)/4$ and $(4x-8xe^{-2x}-e^{-4x}+1)/16$. The variance is strictly smaller than the mean for $x>0$: sixteen times their difference has derivative $4[-1+4xe^{-2x}+e^{-4x}]<0$ and is zero at zero, because $\sinh(2x)>2x$. Therefore this process is not a [Cox process](cox-process.md).

## ↑ Ancestors (6)

1. [Poisson process](poisson-process.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
