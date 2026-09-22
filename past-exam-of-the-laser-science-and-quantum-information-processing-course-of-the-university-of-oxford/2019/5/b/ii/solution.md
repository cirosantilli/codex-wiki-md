<h1 id="5/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A two-query network begins in $|0\rangle_x|0\rangle_y$, calls $U_f$, flips the input with $X_x$, calls $U_f$ again, and measures the answer wire in Z. The successive states are

$$
|0,0\rangle\longmapsto|0,f(0)\rangle
\longmapsto|1,f(0)\rangle
\longmapsto|1,f(0)\oplus f(1)\rangle.
$$

The measured answer is zero for constant functions and one for balanced functions. The circuit is drawn in [i](../../../4/b/i.md).

Explicit [oracle](../../../../../boolean-quantum-oracle.md) circuits follow from the form $f(x)=a\oplus bx$:

$$
\boxed{U_f=(I\otimes X^a)\operatorname{CNOT}_{x\to y}^{\,b}.}
$$

Thus the four circuits, respectively for the truth tables in [i](../i.md), are the identity on both wires; a NOT on the answer wire; a [CNOT](../../../../../controlled-not-gate.md) from input to answer; and a [CNOT](../../../../../controlled-not-gate.md) together with an answer NOT. The latter commute, so their order is immaterial. These circuits leave the input wire unchanged and [XOR](../../../../../exclusive-or.md) precisely $f(x)$ into the answer.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [2019](../../../../2019-split.md)
5. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../../split.md)
6. [Laser science and quantum information processing course of the University of Oxford](../../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
7. [Year 4 of the physics course of the University of Oxford](../../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
