<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Since $0<1-2\epsilon<1$, the off-diagonal multiplier of the [iterated phase-flip channel](../../../../../../iterated-phase-flip-channel.md) tends to zero. Thus

$$
\boxed{\lim_{n\to\infty}D_{\epsilon_n}(\rho)=\frac{\rho+Z\rho Z}{2}
=\begin{pmatrix}u&0\\0&1-u\end{pmatrix}.}
$$

Let $P_0=|0\rangle\langle0|$ and $P_1=|1\rangle\langle1|$ be the [computational basis](../../../../../../computational-basis.md) measurement projectors. The [nonselective projective measurement](../../../../../../nonselective-projective-measurement.md) channel is

$$
P_0\rho P_0+P_1\rho P_1
=u|0\rangle\langle0|+(1-u)|1\rangle\langle1|,
$$

which is exactly the displayed limit. Its diagonal entries retain the original outcome [probabilities](../../../../../../probability.md); the measurement outcome is ignored and the coherences are erased. The limiting evolution is therefore the [completely dephasing channel](../../../../../../rank-one-dephasing.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 51](../../../paper-51-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
