<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Before the gates, write the two [Bell states](../../../../bell-state-split.md) as

$$
|\Phi^+\rangle_{12}|\Phi^+\rangle_{34}
=\frac12\sum_{a,b=0}^1|a\rangle_1|a\rangle_2|b\rangle_3|b\rangle_4.
$$

The [CNOT gate](../../../../controlled-not-gate.md) sends the last bit to $b\oplus a$. Projection onto outcome 0 on [qubit](../../../../qubit.md) 4 therefore requires $b=a$. After the [Hadamard gate](../../../../hadamard-gate.md) on [qubit](../../../../qubit.md) 2, projection onto its outcome 0 contributes $1/\sqrt2$ for either remaining value of $a$. The unnormalized surviving state is

$$
\frac{|00\rangle_{13}+|11\rangle_{13}}{2\sqrt2}=\frac12|\Phi^+\rangle_{13}.
$$

Thus

$$
\boxed{|\psi\rangle_{13}=|\Phi^+\rangle_{13},\qquad P(00_{24})=\frac14.}
$$

This is [entanglement swapping](../../../../entanglement-swapping.md): [photons](../../../../photon.md) 1 and 3 become entangled even though the joint measurement acts only on their original partners.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
