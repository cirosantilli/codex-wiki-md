<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Expand the possibly unnormalized second-[qubit](../../../../qubit.md) kets as $|\alpha\rangle=a_0|0\rangle+a_1|1\rangle$ and $|\beta\rangle=b_0|0\rangle+b_1|1\rangle$. The joint [quantum state](../../../../quantum-state.md) is

$$
|\psi\rangle=a_0|00\rangle+a_1|01\rangle+b_0|10\rangle+b_1|11\rangle.
$$

The [Born rule](../../../../born-rule.md) in the orthonormal [computational basis](../../../../computational-basis.md) gives $P_{00}=|a_0|^2$, $P_{01}=|a_1|^2$, and similarly for the two outcomes beginning with one. Ignoring the second outcome therefore gives

$$
\boxed{P_0=|a_0|^2+|a_1|^2=\langle\alpha|\alpha\rangle,\qquad
P_1=|b_0|^2+|b_1|^2=\langle\beta|\beta\rangle.}
$$

Equivalently these are the squared norms of $(|0\rangle\langle0|\otimes I)|\psi\rangle$ and $(|1\rangle\langle1|\otimes I)|\psi\rangle$. Orthogonality of the first [qubit](../../../../qubit.md)'s basis gives $P_0+P_1=\langle\psi|\psi\rangle=1$, even if $\langle\alpha|\beta\rangle$ is nonzero. For a nonzero-probability outcome, the conditional second-[qubit](../../../../qubit.md) [quantum state](../../../../quantum-state.md) is the corresponding ket divided by $\sqrt{P_i}$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
