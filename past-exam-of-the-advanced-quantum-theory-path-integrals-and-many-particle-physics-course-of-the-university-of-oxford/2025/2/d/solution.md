<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [canonical anticommutation relations](../../../../canonical-anticommutation-relations.md) make $(a^\dagger b^\dagger)^2=0$, so the proposed [exponential function](../../../../exponential-function.md) terminates exactly:

$$
|\widetilde0\rangle=A\bigl(|0\rangle+B|11\rangle\bigr).
$$

Use the inverse [Bogoliubov transformation](../../../../bogoliubov-transformation.md) $c=ua-vb^\dagger$, $d=va^\dagger+ub$, and the actions $a|11\rangle=b^\dagger|0\rangle$ and $b|11\rangle=-a^\dagger|0\rangle$. The two [vacuum state](../../../../vacuum-state.md) conditions become

$$
c|\widetilde0\rangle=A(uB-v)b^\dagger|0\rangle=0,\qquad
d|\widetilde0\rangle=A(v-uB)a^\dagger|0\rangle=0.
$$

Both therefore require $B=v/u$. Normalizing this [quantum state](../../../../quantum-state.md) gives $1=A^2(1+B^2)$. Choosing positive $A$, which fixes an irrelevant overall [global phase](../../../../global-phase.md), yields $A=u$ because $u^2+v^2=1$. Thus the [two-mode fermionic paired vacuum](../../../../two-mode-fermionic-paired-vacuum.md) is

$$
\boxed{|\widetilde0\rangle=u|0\rangle+v a^\dagger b^\dagger|0\rangle,\qquad
A=\sqrt{\frac{E+\varepsilon}{2E}},\qquad
B=\frac\Delta{E+\varepsilon}
=\sqrt{\frac{E-\varepsilon}{E+\varepsilon}},\quad
E=\sqrt{\varepsilon^2+\Delta^2}.}
$$

The other sign for $A$ describes the same physical [quantum state](../../../../quantum-state.md). The positive relative coefficient is fixed by the paper's pairing order and the convention $|11\rangle=a^\dagger b^\dagger|0\rangle$.

As a direct [eigenvector](../../../../eigenvector.md) check, $\Delta v=(E-\varepsilon)u$ and $\Delta u=(E+\varepsilon)v$ imply

$$
\begin{pmatrix}0&-\Delta\\-\Delta&2\varepsilon\end{pmatrix}
\binom uv=(\varepsilon-E)\binom uv.
$$

It is therefore the unique [ground state](../../../../ground-state.md), as also follows from positive [quasiparticle](../../../../quasiparticle.md) excitation [energy](../../../../energy-split.md) $E$. It has definite even [fermion parity](../../../../fermion-parity.md) but is not an [eigenstate](../../../../eigenstate.md) of the original total [number operator](../../../../number-operator.md): the empty-pair and occupied-pair [probabilities](../../../../probability.md) are $u^2$ and $v^2$. In particular $\langle N_a\rangle=\langle N_b\rangle=v^2$. The pair amplitude is $\langle ab\rangle=-uv$, consistently with $ab|11\rangle=-|0\rangle$.

For the limiting check $\Delta\to0^+$ at fixed positive $\varepsilon$, $A\to1$, $B\to0$, so $|\widetilde0\rangle\to|0\rangle$. For $\varepsilon\to0^+$ at fixed positive $\Delta$, $A\to1/\sqrt2$, $B\to1$, giving equal amplitudes for the empty and occupied pair. These checks also fix which branch of the [Bogoliubov transformation](../../../../bogoliubov-transformation.md) produces the [ground state](../../../../ground-state.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../../advanced-quantum-theory-path-integrals-and-many-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
