<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

With the negative exponential convention of the specified [quantum Fourier transform](../../../../../../quantum-fourier-transform.md), the amplitude of computational outcome $k$ is

$$
\langle k|U|\psi_m\rangle
=\frac1N\sum_{l=0}^{N-1}e^{2\pi i(m-k)l/N}.
$$

If $k=m$, every summand is one. Otherwise this finite [geometric series](../../../../../../geometric-series.md) has ratio $q\ne1$ with $q^N=1$, so it equals $(1-q^N)/(1-q)=0$. Thus

$$
\boxed{U|\psi_m\rangle=|m\rangle.}
$$

The [Born rule](../../../../../../born-rule.md) gives outcome $m$ with probability one when performing a [quantum measurement in the computational basis](../../../../../../quantum-measurement-in-the-computational-basis.md). Recover the promised phase as $\phi_m=2\pi m/N$ modulo $2\pi$. Using the opposite Fourier sign would instead return the label $-m\bmod N$, so the sign convention matters.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
