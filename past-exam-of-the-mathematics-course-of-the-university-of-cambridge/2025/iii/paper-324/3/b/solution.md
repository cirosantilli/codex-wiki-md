<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The shift $S|x\rangle=|x-1\bmod Q\rangle$ acts on a Fourier state as

$$
\begin{aligned}
S\operatorname{QFT}_Q|a\rangle
&=\frac1{\sqrt Q}\sum_x\omega^{ax}|x-1\rangle\\
&=\omega^a\operatorname{QFT}_Q|a\rangle.
\end{aligned}
$$

Thus $\operatorname{QFT}_Q|a\rangle$ is an [eigenvector](../../../../../../eigenvector.md) of $S$ with eigenphase $a/Q$. Apply the unitary part of [exact quantum phase estimation](../../../../../../exact-quantum-phase-estimation.md) for $S$ to a zeroed control register and this Fourier state. It writes the eigenphase label coherently:

$$
\boxed{
|0^m\rangle\operatorname{QFT}_Q|a\rangle
\longmapsto
|a\rangle\operatorname{QFT}_Q|a\rangle}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
