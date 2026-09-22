<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

With $N$ [vanishing moments](../../../../../../vanishing-moment.md), a [wavelet](../../../../../../wavelet.md) annihilates every [polynomial](../../../../../../polynomial-split.md) of degree below $N$. A [Taylor polynomial](../../../../../../taylor-polynomial.md) then explains small [wavelet](../../../../../../wavelet.md) coefficients on smooth parts of a signal, and efficient [best N-term approximation](../../../../../../best-n-term-approximation.md). [Compact support](../../../../../../compact-support.md) localizes coefficients near a feature, limits the number of boundary interactions, and permits a finite filter implementation. Increasing the number of [vanishing moments](../../../../../../vanishing-moment.md) while keeping an [orthonormal basis](../../../../../../orthonormal-basis.md) generally requires a larger [support of a function](../../../../../../support.md): a finite orthonormal filter with $N$ [vanishing moments](../../../../../../vanishing-moment.md) needs at least $2N$ taps, and the minimal-support [Daubechies wavelet](../../../../../../daubechies-wavelet.md) has support length $2N-1$ in the standard normalization.

The [Haar wavelet](../../../../../../haar-wavelet.md), $\psi=\chi_{[0,1/2)}-\chi_{[1/2,1)}$, has one [vanishing moment](../../../../../../vanishing-moment.md), unit support length and discontinuities. It is inexpensive and particularly suitable for piecewise constant data with sharp jumps. A [Daubechies wavelet](../../../../../../daubechies-wavelet.md) of a larger order has more [vanishing moments](../../../../../../vanishing-moment.md) and a longer finite filter; sufficiently large orders also provide greater regularity. It is useful when smooth trends should yield small coefficients, although the wider [support of a function](../../../../../../support.md) can spread a jump across more coefficients. **Choose Haar for compact jump localization; choose a higher-order Daubechies wavelet for smooth polynomial structure.** More [vanishing moments](../../../../../../vanishing-moment.md) alone does not make every low-order wavelet highly differentiable.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 340](../../../paper-340-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
