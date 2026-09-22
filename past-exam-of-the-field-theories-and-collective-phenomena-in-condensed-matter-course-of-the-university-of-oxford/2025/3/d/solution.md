<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The inverse [Bogoliubov transformation](../../../../bogoliubov-transformation.md) gives $c=ua-vb^\dagger$ and $d=va^\dagger+ub$. Because $(a^\dagger b^\dagger)^2=0$ by the [canonical anticommutation relations](../../../../canonical-anticommutation-relations.md), the exponential truncates:

$$
Ae^{Ba^\dagger b^\dagger}|0\rangle
=A\bigl(|0\rangle+Ba^\dagger b^\dagger|0\rangle\bigr).
$$

The [fermionic signs](../../../../fermionic-sign.md) are fixed by

$$
a\,a^\dagger b^\dagger|0\rangle=b^\dagger|0\rangle,
\qquad
b\,a^\dagger b^\dagger|0\rangle=-a^\dagger|0\rangle.
$$

It follows that

$$
c|\tilde0\rangle=A(uB-v)b^\dagger|0\rangle,
\qquad
d|\tilde0\rangle=A(v-uB)a^\dagger|0\rangle.
$$

Both annihilation conditions hold precisely when $B=v/u$. Normalizing the [paired fermionic vacuum](../../../../two-mode-fermionic-paired-vacuum.md), using the [orthogonality](../../../../orthogonal-vectors.md) of its two [Fock states](../../../../fock-state.md), gives $A^2(1+B^2)=1$. Choose the irrelevant overall phase so that $A>0$. The result is

$$
\boxed{A=u=\sqrt{\frac{E+\varepsilon}{2E}},\qquad
B=\frac vu=\frac{\Delta}{E+\varepsilon}
=\frac{E-\varepsilon}{\Delta},\qquad
E=\sqrt{\varepsilon^2+\Delta^2}.}
$$

Equivalently,

$$
\boxed{|\tilde0\rangle=u|0\rangle+va^\dagger b^\dagger|0\rangle.}
$$

Its positive pair coefficient follows from the specified order $ab+b^\dagger a^\dagger$ in the [Hamiltonian operator](../../../../hamiltonian-quantum-mechanics.md). The state has even [fermion parity](../../../../fermion-parity.md) and is a [quantum superposition](../../../../quantum-superposition.md) of zero and two original particles. In the limit $\Delta\to0^+$, $A\to1$ and $B\to0$, so it reduces to the original [vacuum state](../../../../vacuum-state.md), as expected for $\varepsilon>0$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the field theories and collective phenomena in condensed matter course of the University of Oxford](../../../split.md)
5. [Field theories and collective phenomena in condensed matter course of the University of Oxford](../../../../field-theories-and-collective-phenomena-in-condensed-matter-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
