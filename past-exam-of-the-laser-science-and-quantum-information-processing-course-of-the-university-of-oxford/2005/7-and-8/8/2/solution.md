<h1 id="8/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Define the [Hadamard basis](../../../../../hadamard-basis.md) $|\pm\rangle=(|0\rangle\pm|1\rangle)/\sqrt2$ and write $s=e^{-i\phi}$. After $U_\phi$ the two-[qubit](../../../../../qubit.md) [quantum state](../../../../../quantum-state.md) is

$$
U_\phi|++\rangle=\frac{|00\rangle+s|01\rangle+|10\rangle+|11\rangle}{2}.
$$

Applying the [Hadamard gate](../../../../../hadamard-gate.md) to the first [qubit](../../../../../qubit.md) gives the normalized [quantum state](../../../../../quantum-state.md)

$$
|\chi_2(\phi)\rangle
=\frac{2|00\rangle+(1+s)|01\rangle+(s-1)|11\rangle}{2\sqrt2}.
$$

For $\phi=n\pi$, $s=(-1)^n$, so

$$
\boxed{|\chi_2(n\pi)\rangle=
\begin{cases}
|0\rangle|+\rangle,&n\text{ even},\\
(|00\rangle-|11\rangle)/\sqrt2=|\phi^-\rangle,&n\text{ odd}.
\end{cases}}
$$

The first is a [product state](../../../../../product-state.md). The second is exactly the minus [Bell state](../../../../../bell-state-split.md) in the printed [phase gate](../../../../../phase-gate.md) convention; its [reduced density matrices](../../../../../reduced-density-matrix.md) are $I/2$.

For three [qubits](../../../../../qubit.md), let $U_{12}$ use the ordered pair $(1,2)$ and $U_{23}$ the ordered pair $(2,3)$. The two diagonal [quantum gates](../../../../../quantum-logic-gate.md) commute. For $\phi=n\pi$ their action before the final [Hadamard gates](../../../../../hadamard-gate.md) is

$$
U_{23}U_{12}|+++\rangle
=\frac1{\sqrt8}\sum_{a,b,c=0}^1(-1)^{n[(1-a)b+(1-b)c]}|abc\rangle.
$$

If $n$ is even this is $|+++\rangle$, and $H_1H_3$ gives $|0\rangle|+\rangle|0\rangle$. If $n$ is odd, group the [quantum superposition](../../../../../quantum-superposition.md) by the middle [qubit](../../../../../qubit.md):

$$
U_{23}U_{12}|+++\rangle
=\frac{|+\rangle_1|0\rangle_2|-\rangle_3
-|-\rangle_1|1\rangle_2|+\rangle_3}{\sqrt2}.
$$

Since $H_{\rm Had}|+\rangle=|0\rangle$ and $H_{\rm Had}|-\rangle=|1\rangle$, the final states are

$$
\boxed{|\chi_3(n\pi)\rangle=
\begin{cases}
|0\rangle|+\rangle|0\rangle,&n\text{ even},\\
\displaystyle|G\rangle=\frac{|001\rangle-|110\rangle}{\sqrt2},&n\text{ odd}.
\end{cases}}
$$

The odd case is a [GHZ state](../../../../../greenberger-horne-zeilinger-state.md): each individual [qubit](../../../../../qubit.md) has [reduced density matrix](../../../../../reduced-density-matrix.md) $I/2$, and it is related to $(|000\rangle+|111\rangle)/\sqrt2$ by the local [Pauli gates](../../../../../pauli-gate.md) $Z_1X_3$. Conversely, applying those gates converts $|G\rangle$ to that standard form. They have not been applied in the printed network, so the actual output used in the next part is $|G\rangle=(|001\rangle-|110\rangle)/\sqrt2$.

## ↑ Ancestors (13)

1. [2](../2.md)
2. [8](../../8.md)
3. [7 and 8](../../../7-and-8-split.md)
4. [2005](../../../split.md)
5. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../../split.md)
6. [Laser science and quantum information processing course of the University of Oxford](../../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
7. [Year 4 of the physics course of the University of Oxford](../../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
