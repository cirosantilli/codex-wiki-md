<h1 id="15d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Apply the gates from left to right. The first [Hadamard gate](../../../../../../hadamard-gate.md) and the first [controlled-NOT gate](../../../../../../controlled-not-gate.md) produce the [Bell state](../../../../../../bell-state-split.md)

$$
\frac{|00\rangle+|11\rangle}{\sqrt2}.
$$

The parallel $Z\otimes H$ gates then produce

$$
\frac12\left(|00\rangle+|01\rangle-|10\rangle+|11\rangle\right).
$$

The final controlled-NOT has the lower qubit as control; it interchanges $|01\rangle$ and $|11\rangle$, whose amplitudes here are equal. Thus the output is

$$
\boxed{
|\psi_{\rm out}\rangle
=\frac12\left(|00\rangle+|01\rangle-|10\rangle+|11\rangle\right).}
$$

By [quantum measurement in the computational basis](../../../../../../quantum-measurement-in-the-computational-basis.md), every basis outcome has probability equal to the squared modulus of its amplitude:

$$
\boxed{\Pr(00)=\Pr(01)=\Pr(10)=\Pr(11)=\frac14.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [15D](../../15d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
