<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $p=|\alpha|^2$, so $|\beta|^2=1-p$. The [projective measurement](../../../../projective-measurement.md) has outcome 0 with [probability](../../../../probability.md) $p$ and leaves the state $|0\rangle$; outcome 1 has [probability](../../../../probability.md) $1-p$ and leaves $|1\rangle$. Alice knows her actual result, so her conditional description is a [pure state](../../../../pure-state.md). Her [fidelity of quantum states](../../../../fidelity-of-quantum-states.md) with the initial state is $p$ after outcome 0 or $1-p$ after outcome 1. Its outcome average is $p^2+(1-p)^2$.

Bob knows the preparation but not the outcome, so his [density matrix](../../../../density-matrix-split.md) is the nonselective postmeasurement state

$$
\boxed{\rho_B=p|0\rangle\langle0|+(1-p)|1\rangle\langle1|,\qquad
F_B=\langle\psi|\rho_B|\psi\rangle=p^2+(1-p)^2.}
$$

It is mixed for $0<p<1$ and pure only at the endpoints. The relative [phase](../../../../phase-waves.md) has disappeared because the classical outcome record is unavailable to him.

The [undisclosed qubit measurement outcome with an unspecified preparation prior](../../../../undisclosed-qubit-measurement-outcome-with-an-unspecified-preparation-prior.md) requires care: Charlene has no specified prior over preparations. Consequently the information given does not determine a unique posterior [probability](../../../../probability.md) for the two outcomes. Under a symmetric ignorance or maximum-entropy prior, her best assignment is

$$
\boxed{\rho_C=I/2,\qquad F_C=1/2.}
$$

More generally, if her prior mean of $|\alpha|^2$ is $q$, her assignment is $\rho_C=\operatorname{diag}(q,1-q)$ and its [fidelity of quantum states](../../../../fidelity-of-quantum-states.md) with the actual initial state is $pq+(1-p)(1-q)$. Knowing that a measurement occurred guarantees diagonality in its basis, but does not by itself prove $q=1/2$. Different descriptions here reflect different available records, rather than different physical outcomes. [Sections 2.3–2.4, density matrices, ensembles and measurement information](../../../../foundations-i-states-and-ensembles-by-john-preskill.md)

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
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
