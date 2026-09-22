<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The PDF circuit has its upper wire controlling both [CNOT gates](../../../../../../controlled-not-gate.md). Its successive states are

$$
|00\rangle\ \longmapsto\ \frac{|00\rangle+|10\rangle}{\sqrt2}
\ \longmapsto\ \frac{|00\rangle+|11\rangle}{\sqrt2}
\ \longmapsto\ \frac{|00\rangle+e^{2i\phi}|11\rangle}{\sqrt2}
\ \longmapsto\ \frac{|00\rangle+e^{2i\phi}|10\rangle}{\sqrt2}.
$$

The first arrow is the upper [Hadamard gate](../../../../../../hadamard-gate.md); the middle phase arises because both ones receive a phase. The second CNOT disentangles and resets the lower wire. Hence the output is

$$
\boxed{\frac{|0\rangle+e^{2i\phi}|1\rangle}{\sqrt2}\otimes|0\rangle.}
$$

This implements doubled logical phase using two parallel [phase gates](../../../../../../phase-gate.md), rather than two serial applications on one [qubit](../../../../../../qubit.md).

## ↑ Ancestors (11)

1. [C](../c.md)
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
