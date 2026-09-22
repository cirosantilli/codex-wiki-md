# FFT butterfly

↑ **Parent:** [Cooley-Tukey FFT algorithm](cooley-tukey-fft-algorithm.md)

An [FFT butterfly](fft-butterfly.md) combines corresponding outputs of two half-sized transforms using a twiddle factor $w$. Sharing the product $wb$ costs one complex multiplication and two additions. For the unnormalized positive-exponent inverse [discrete Fourier transform](discrete-fourier-transform.md) of length $2m$, use $w=e^{2\pi i\ell/(2m)}$ at index $\ell$.

## ↑ Ancestors (7)

1. [Cooley-Tukey FFT algorithm](cooley-tukey-fft-algorithm.md)
2. [Discrete Fourier transform](discrete-fourier-transform.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (5)

- [FFT butterfly](fft-butterfly.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-57/8/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-2/39a/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-2/39a/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-2/39a/4/solution.md)
