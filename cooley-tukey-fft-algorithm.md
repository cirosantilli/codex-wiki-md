# Cooley-Tukey FFT algorithm

↑ **Parent:** [Fast Fourier transform](fast-fourier-transform.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cooley–Tukey_FFT_algorithm)

The radix-two Cooley--Tukey algorithm recursively splits a discrete Fourier transform into transforms of the even-indexed and odd-indexed samples. For a power-of-two length this evaluates the transform in $O(m\log m)$ arithmetic operations.

The saving comes from reusing the two shorter [discrete Fourier transforms](discrete-fourier-transform-split.md) for both halves of the output, through an [FFT butterfly](fft-butterfly.md). For $N=2^p$, each level of the [even--odd fast Fourier transform recursion](even-odd-fast-fourier-transform-recursion.md) needs work proportional to $N$, and there are $p=\log_2N$ levels. This gives the $O(N\log N)$ [time complexity](time-complexity.md) without changing the [discrete Fourier transform](discrete-fourier-transform-split.md) being computed.

James W. Cooley and John W. Tukey published _An Algorithm for the Machine Calculation of Complex Fourier Series_ in _Mathematics of Computation_ 19 (1965), pp. 297–301. Their original paper factors a composite length as $N=r_1\cdots r_p$, derives an operation count $N(r_1+\cdots+r_p)$, and discusses powers of two and in-place storage. Its opening explicitly builds on earlier [algorithms](algorithm-split.md) by I. J. Good; the 1965 paper is a landmark computational formulation, rather than the invention of the underlying [Fourier analysis](fourier-analysis-split.md). Its positive-exponent convention also illustrates why a [Fast Fourier transform](fast-fourier-transform.md)'s exponent sign must be specified.[Cooley and Tukey 1965, original paper, pp. 297–300, equations (1)–(12); scan of the published article](https://janmr.com/files/papers/cooley-tukey.pdf)

**Table of contents**

- [FFT butterfly](fft-butterfly.md)
- [Even--odd fast Fourier transform recursion](even-odd-fast-fourier-transform-recursion.md)

## ↑ Ancestors (7)

1. [Fast Fourier transform](fast-fourier-transform.md)
2. [Discrete Fourier transform](discrete-fourier-transform-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Fast Fourier transform](fast-fourier-transform.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-57/8/solution.md)
