<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $\rho_0=|\phi\rangle\langle\phi|=(I+r_xX+r_yY+r_zZ)/2$. Conjugating by a [Pauli matrix](../../../../../../pauli-matrices.md) keeps its own Bloch component and reverses the other two; for example,

$$
X\rho_0X=\tfrac12(I+r_xX-r_yY-r_zZ).
$$

In the average of the four conjugations, the coefficient of every nonidentity [Pauli matrix](../../../../../../pauli-matrices.md) is zero. Consequently

$$
\boxed{\frac{\rho_0+X\rho_0X+Y\rho_0Y+Z\rho_0Z}{4}=\frac I2.}
$$

The [Pauli operator basis](../../../../../../pauli-operator-basis.md) gives the Bloch representation of a [qubit](../../../../../../qubit.md) [density operator](../../../../../../density-matrix-split.md).[§2.3.2, printed pp. 18–19, equations (2.62)–(2.65)](../../../../../../foundations-i-states-and-ensembles-by-john-preskill.md)

This is the [qubit Pauli twirl](../../../../../../qubit-pauli-twirl.md), the dimension-two case of the [Heisenberg-Weyl twirling channel](../../../../../../heisenberg-weyl-twirling-channel.md). The argument uses only [trace](../../../../../../matrix-trace.md) one, so it also works for mixed [qubit](../../../../../../qubit.md) inputs. The preparation label must be forgotten: conditioning on the label would retain a known pure branch rather than the [maximally mixed state](../../../../../../maximally-mixed-state.md) obtained by the ensemble average.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Quantum information](../../../../quantum-information-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
