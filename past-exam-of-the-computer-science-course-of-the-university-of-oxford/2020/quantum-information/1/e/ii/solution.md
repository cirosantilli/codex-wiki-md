<h1 id="1/e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Compute the parity into the second wire, phase that wire with the [T gate](../../../../../../t-gate.md), then uncompute with the same [controlled-NOT gate](../../../../../../controlled-not-gate.md). The answer is

$$
\boxed{G=\mathrm{CNOT}\,(I\otimes T)\,\mathrm{CNOT}.}
$$

For computational bits $x,y$, the successive states are $|x,y\rangle\mapsto|x,x\oplus y\rangle\mapsto e^{i\pi(x\oplus y)/4}|x,x\oplus y\rangle\mapsto e^{i\pi(x\oplus y)/4}|x,y\rangle$. The parity $x\oplus y$ is one precisely on the two odd-parity inputs. Thus, in the ordered [computational basis](../../../../../../computational-basis.md) $00,01,10,11$, the [matrix](../../../../../../matrix.md) is exactly $\operatorname{diag}(1,e^{i\pi/4},e^{i\pi/4},1)$, with no omitted overall phase. This is a [two-qubit parity phase gate](../../../../../../two-qubit-parity-phase-gate.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [E](../../e.md)
3. [1](../../../1.md)
4. [Quantum information](../../../../quantum-information-split.md)
5. [2020](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
