<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use basis order $000,001,010,011,100,101,110,111$, with the ancilla first, and put $x=e^{i\phi_1}$, $y=e^{i\phi_2}$. Initially the ancilla is at the north pole of the [Bloch sphere](../../../../bloch-sphere.md). The other two [qubits](../../../../qubit.md) lie on its equator at azimuths $\phi_1,\phi_2$, with [Bloch vectors](../../../../bloch-vector.md) $(\cos\phi_j,\sin\phi_j,0)$.

The four dotted cuts, in left-to-right order, have the explicit normalized vectors

$$
\boxed{v_0=\frac12(1,y,x,xy,0,0,0,0)^{\mathsf T},}
$$



$$
\boxed{v_1=\frac1{2\sqrt2}(1,y,x,xy,1,y,x,xy)^{\mathsf T},}
$$



$$
\boxed{v_2=\frac1{2\sqrt2}(1,y,x,xy,1,x,y,xy)^{\mathsf T},}
$$



$$
\boxed{v_3=\frac14(2,x+y,x+y,2xy,0,y-x,x-y,0)^{\mathsf T}.}
$$

The first [Hadamard gate](../../../../hadamard-gate.md) copies the lower-register amplitudes into two control branches; the [Fredkin gate](../../../../fredkin-gate.md) exchanges them only in the second branch; the final [Hadamard gate](../../../../hadamard-gate.md) adds and subtracts these branches.

Summing the squared magnitudes of the first four entries of $v_3$ gives

$$
P_0=\frac{8+2|x+y|^2}{16}=\frac34+\frac14\cos(\phi_1-\phi_2).
$$

Meanwhile $\langle\phi_2|\phi_1\rangle=(1+e^{i(\phi_1-\phi_2)})/2$, so

$$
\boxed{P_0=\frac{1+|\langle\phi_2|\phi_1\rangle|^2}{2}.}
$$

Identical input [qubits](../../../../qubit.md) give $P_0=1$; orthogonal equatorial inputs give $P_0=1/2$. The factor one half is an ancilla-interference effect, not a direct [projective measurement](../../../../projective-measurement.md) of the lower [qubits](../../../../qubit.md) individually.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
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
