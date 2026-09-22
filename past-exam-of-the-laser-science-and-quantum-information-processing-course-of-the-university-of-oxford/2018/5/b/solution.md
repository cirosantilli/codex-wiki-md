<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the lower-qubit controlled rotation, the control is the upper [qubit](../../../../qubit.md) and only the subspace $|10\rangle,|11\rangle$ rotates. Write $u=\cos(\theta/2)$ and $v=\sin(\theta/2)$. Unitary conjugation of its diagonal populations gives $cu^2+dv^2$ and $cv^2+du^2$, together with off-diagonal coherences. The ideal crush gradient stipulated in the source removes those coherences without changing populations. Therefore

$$
\boxed{c'=\frac{c+d+\cos\theta(c-d)}2,\qquad d'=\frac{c+d-\cos\theta(c-d)}2,\qquad \alpha=\cos\theta.}
$$

The other two populations remain $a,b$. This [controlled-transfer gate](../../../../controlled-transfer-gate.md) is not unitary as a complete operation because it includes [dephasing](../../../../dephasing-channel.md).

For an upper-qubit target, the lower [qubit](../../../../qubit.md) is the control: the mixed subspace is $|01\rangle,|11\rangle$. Thus

$$
\boxed{(a,b,c,d)\longmapsto\left(a,\frac{b+d+\cos\theta(b-d)}2,c,\frac{b+d-\cos\theta(b-d)}2\right).}
$$

The population $a$ of $|00\rangle$ is unaffected in either direction because its control bit is zero. The [dephasing](../../../../dephasing-channel.md) step also leaves this diagonal population unchanged, so any sequence of these controlled-transfer gates preserves $a$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
