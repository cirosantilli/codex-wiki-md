<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Start with $(|a\rangle+|b\rangle)/\sqrt2$ and a zeroed second register. Apply the coherent construction from part (a)(iv) to obtain

$$
\frac1{\sqrt2}\left(
|a\rangle\operatorname{QFT}_Q|a\rangle
+|b\rangle\operatorname{QFT}_Q|b\rangle\right).
$$

Now run the inverse of the phase-estimation map from part (b) on the two registers. It erases the first label in both branches:

$$
|0^m\rangle\frac{
\operatorname{QFT}_Q|a\rangle+
\operatorname{QFT}_Q|b\rangle}{\sqrt2}
=|0^m\rangle\operatorname{QFT}_Q
\frac{|a\rangle+|b\rangle}{\sqrt2}.
$$

Discarding the zeroed register leaves the required [quantum Fourier transform](../../../../../../quantum-fourier-transform.md) of the superposition. The coherent use of a computed label followed by its inverse is an [uncomputation](../../../../../../uncomputation.md).

## ↑ Ancestors (11)

1. [C](../c.md)
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
