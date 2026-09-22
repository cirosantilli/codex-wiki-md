<h1 id="10d/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

If $f(b_1b_2)=b_1\oplus b_2$, then

$$
(-1)^{f(b_1b_2)}=(-1)^{b_1+b_2},
$$

so

$$
|f\rangle
=\frac{|0\rangle-|1\rangle}{\sqrt2}
\otimes
\frac{|0\rangle-|1\rangle}{\sqrt2}
=H^{\otimes2}|11\rangle.
$$

In either promised case, construct $|f\rangle$ by the one-query procedure in part (a), apply the [Walsh-Hadamard transform](../../../../../../../walsh-hadamard-transform.md) $H^{\otimes2}$ to its two qubits, and perform a [quantum measurement in the computational basis](../../../../../../../quantum-measurement-in-the-computational-basis.md). The outcome is certainly $00$ for case (i) and certainly $11$ for case (ii). Therefore

$$
\boxed{00\Longrightarrow\text{constant},\qquad
11\Longrightarrow f(b_1b_2)=b_1\oplus b_2.}
$$

This is a two-bit instance of [Bernstein-Vazirani phase kickback](../../../../../../../bernstein-vazirani-phase-kickback.md), and also a promised [Deutsch-Jozsa test](../../../../../../../deutsch-jozsa-algorithm.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [10D](../../../10d.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
