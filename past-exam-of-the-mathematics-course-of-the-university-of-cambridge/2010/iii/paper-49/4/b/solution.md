<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The inverse [quantum Fourier transform](../../../../../../quantum-fourier-transform.md) in the original PDF has matrix elements $N^{-1/2}e^{-2\pi iky/N}$ multiplying $|y\rangle\langle k|$. The converted TeX incorrectly repeats $y$ in the bra; using the actual PDF operator,

$$
F^\dagger|\psi\rangle
=\frac1N\sum_{y=0}^{N-1}\left(\sum_{x=0}^{N-1}e^{2\pi i(a-y)x/N}\right)|y\rangle.
$$

If $y=a$, every summand of the inner sum is one, so it equals $N$. If $y\ne a$, let $q=e^{2\pi i(a-y)/N}$. Then $q\ne1$ and $q^N=1$, and the finite [geometric series](../../../../../../geometric-series.md) gives $\sum_{x=0}^{N-1}q^x=(1-q^N)/(1-q)=0$. This is [orthogonality of roots of unity](../../../../../../orthogonality-of-roots-of-unity.md). Hence

$$
\boxed{F^\dagger|\psi\rangle=|a\rangle.}
$$

A [quantum measurement in the computational basis](../../../../../../quantum-measurement-in-the-computational-basis.md) consequently returns the integer $a$ with probability one.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 49](../../../paper-49-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
