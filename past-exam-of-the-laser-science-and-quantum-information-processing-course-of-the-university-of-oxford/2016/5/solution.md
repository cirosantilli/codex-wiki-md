<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For $|\alpha|^2+|\beta|^2=1$, the [density operator](../../../density-matrix-split.md) and its computational-basis matrix are

$$
\hat\rho=|\psi\rangle\langle\psi|,\qquad\rho=\begin{pmatrix}|\alpha|^2&\alpha\beta^*\\\alpha^*\beta&|\beta|^2\end{pmatrix}.
$$

It is a [Hermitian matrix](../../../hermitian-operator.md) and satisfies $\rho^2=\rho$, so $\operatorname{tr}\rho^2=1$. Its eigenvalues are one and zero. Thus **a pure qubit's density matrix is not unitary**: it is singular, and $\rho^\dagger\rho=\rho\ne I$.

Transposing gives $\rho^T=|\psi^*\rangle\langle\psi^*|$. It reflects the Bloch vector $(x,y,z)$ to $(x,-y,z)$. Choose the positive axis states $|+\rangle$, $|+i\rangle=(|0\rangle+i|1\rangle)/\sqrt2$ and $|0\rangle$; their target kets are respectively $|+\rangle$, $|-i\rangle$ and $|0\rangle$.

Nonunitarity alone does not make a quantum operation unphysical. The [qubit transpose map](../../../qubit-transpose-map.md) fails [complete positivity](../../../completely-positive-map.md): applying it to one half of a Bell pair gives a matrix with a negative eigenvalue. A physical approximation must instead be a valid [quantum channel](../../../quantum-channel.md).

Use the [squared quantum fidelity](../../../squared-quantum-fidelity.md) specified in the question, comparing each actual output to the transposed target. For a pure input Bloch vector $\mathbf r$, the identity approximation has $F_I=1-y^2$. Conjugation by the [Pauli X gate](../../../pauli-x-gate.md) produces $(x,-y,-z)$, giving $F_X=1-z^2$. Measuring in the computational basis and preparing the corresponding basis state is the dephasing channel $(x,y,z)\mapsto(0,0,z)$, giving $F_Z=(1+z^2)/2$. Therefore

$$
\begin{array}{c|ccc|c}
\text{approximation}&+x&+y&+z&\text{average}\\\hline
I&1&0&1&2/3\\
X&1&1&0&2/3\\
\text{measure and prepare}&1/2&1/2&1&2/3
\end{array}
$$

The stipulated three-axis averages also agree with the uniform Bloch-sphere averages, since each squared coordinate averages to $1/3$.

The complete perfect-fidelity input sets, up to a global phase, are:

- For the identity, $y=0$: all states whose two amplitudes can be chosen real, the Bloch sphere's $xz$ great circle.
- For X, $z=0$: all equal-magnitude superpositions $(|0\rangle+e^{i\phi}|1\rangle)/\sqrt2$, its equator.
- For measurement and preparation, $z^2=1$: only $|0\rangle$ and $|1\rangle$.

Each condition follows by setting the corresponding fidelity formula to one, so these lists include all perfect cases rather than just the three test inputs.

## ↑ Ancestors (11)

1. [5](../5.md)
2. [2016](../../2016-split.md)
3. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../split.md)
4. [Laser science and quantum information processing course of the University of Oxford](../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
5. [Year 4 of the physics course of the University of Oxford](../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
