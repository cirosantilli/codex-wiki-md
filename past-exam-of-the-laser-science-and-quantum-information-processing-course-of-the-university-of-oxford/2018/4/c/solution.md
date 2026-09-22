<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $d$-dimensional unitaries, $\operatorname{tr}(U^\dagger U)=d$. The relative propagator $W=U^\dagger V$ is unitary, and its eigenvalues lie on the unit circle. The triangle inequality gives $|\operatorname{tr}W|\leq d$, with equality precisely when all eigenvalues have the same [phase](../../../../phase-waves.md), or $V=e^{i\gamma}U$. Therefore the specified [trace-overlap gate fidelity](../../../../trace-overlap-gate-fidelity.md) lies between zero and one, is insensitive to [global phase](../../../../global-phase.md), and equals one exactly when the implemented gate has the same physical action as the target. It compares propagators independently of any particular input state; it is not the identically defined quantity as average state or average gate fidelity.

For target $R_x(\pi)$ and actual $R_x[\pi(1+\epsilon)]$, the relative propagator is $R_x(\pi\epsilon)$. Its trace is $2\cos(\pi\epsilon/2)$, so

$$
\boxed{\mathcal F_1=\left|\cos\frac{\pi\epsilon}{2}\right|=1-\frac{\pi^2}{8}\epsilon^2+O(\epsilon^4),\qquad \alpha=\frac{\pi^2}{8}.}
$$

The absolute value is unnecessary in a sufficiently small neighbourhood of zero error, but belongs in the exact expression.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
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
