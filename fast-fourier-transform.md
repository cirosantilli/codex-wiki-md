# Fast Fourier transform

↑ **Parent:** [Discrete Fourier transform](discrete-fourier-transform.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fast_Fourier_transform)

A [Fast Fourier transform](fast-fourier-transform.md) is an efficient [algorithm](algorithm.md) for computing the [discrete Fourier transform](discrete-fourier-transform.md) or [inverse discrete Fourier transform](inverse-discrete-fourier-transform.md). The [discrete Fourier transform](discrete-fourier-transform.md) specifies the mathematical result; a [Fast Fourier transform](fast-fourier-transform.md) specifies how to compute it. Different [Fast Fourier transform](fast-fourier-transform.md) [algorithms](algorithm.md) reorganize the same finite sums, with the selected sign and normalization. The [Cooley-Tukey FFT algorithm](cooley-tukey-fft-algorithm.md) is one important family of [Fast Fourier transforms](fast-fourier-transform.md), using factorization of the record length.[Balakrishnan, Terman, and Verghese, MIT 6.02 notes, §13.2.6, p. 194: the FFT computes the existing transform, 2012](https://ocw.mit.edu/courses/6-02-introduction-to-eecs-ii-digital-communication-systems-fall-2012/06d7972059805d20e6a7db3a52ec23f2_MIT6_02F12_chap13.pdf)

For a power-of-two length, the radix-two [Cooley-Tukey FFT algorithm](cooley-tukey-fft-algorithm.md) has [time complexity](time-complexity.md) $O(N\log N)$ in arithmetic operations, compared with $O(N^2)$ for evaluating every sum independently; these are [Big O notation](big-o-notation.md) growth rates rather than machine timings. It returns the same eight [coefficients](coefficient.md) $(8,4,-2i,0,0,0,2i,4)$ in the example. In exact arithmetic this reorganization introduces no approximation; actual implementations still incur [roundoff error](round-off-error.md).

**Table of contents**

- [Cooley-Tukey FFT algorithm](cooley-tukey-fft-algorithm.md)
  - [FFT butterfly](fft-butterfly.md)
  - [Even--odd fast Fourier transform recursion](even-odd-fast-fourier-transform-recursion.md)

## ↑ Ancestors (6)

1. [Discrete Fourier transform](discrete-fourier-transform.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Cooley-Tukey FFT algorithm](cooley-tukey-fft-algorithm.md)
- [Discrete Fourier transform](discrete-fourier-transform.md)
- [Discrete sine transform Poisson solver](discrete-sine-transform-poisson-solver.md)
- [Fast Fourier transform](fast-fourier-transform.md)
- [Fourier diagonalization of a circulant matrix](fourier-diagonalization-of-a-circulant-matrix.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-57/8/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-2/39a/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-4/40e/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-341/3/c/solution.md)
