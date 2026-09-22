<h1 id="40e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The radix-two [Fast Fourier transform](../../../../../../cooley-tukey-fft-algorithm.md) recursively applies part (a) until it reaches one-point transforms, then combines adjacent even and odd transforms in butterfly operations. For $n=8$, the decomposition tree is

$$
\mathcal F_8^{-1}
\longrightarrow2\mathcal F_4^{-1}
\longrightarrow4\mathcal F_2^{-1}
\longrightarrow8\mathcal F_1^{-1},
$$

followed by the reverse sequence of twiddle-factor butterfly combinations. This is the usual three-stage FFT network.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [40E](../../40e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
