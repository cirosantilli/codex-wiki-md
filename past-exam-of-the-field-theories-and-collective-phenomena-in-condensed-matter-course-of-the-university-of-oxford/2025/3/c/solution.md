<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $Q=c^\dagger c+d^\dagger d$ and $P=cd+d^\dagger c^\dagger$. Expanding the [number operators](../../../../number-operator.md) and restoring the displayed order with the [canonical anticommutation relations](../../../../canonical-anticommutation-relations.md) gives

$$
\begin{aligned}
a^\dagger a+b^\dagger b
&=(u^2-v^2)Q+2v^2-2uvP,\\
ab+b^\dagger a^\dagger
&=2uv(Q-1)+(u^2-v^2)P.
\end{aligned}
$$

The minus sign in the first line follows from $c^\dagger d^\dagger+dc=-(cd+d^\dagger c^\dagger)$. Substitution into the [Hamiltonian operator](../../../../hamiltonian-quantum-mechanics.md) yields

$$
H=\bigl[\varepsilon(u^2-v^2)+2\Delta uv\bigr]Q
+\bigl[\Delta(u^2-v^2)-2\varepsilon uv\bigr]P
+2\varepsilon v^2-2\Delta uv.
$$

Let $E=\sqrt{\varepsilon^2+\Delta^2}>0$. A convenient real [Bogoliubov transformation](../../../../bogoliubov-transformation.md) has

$$
\boxed{u=\sqrt{\frac{E+\varepsilon}{2E}},\qquad
v=\sqrt{\frac{E-\varepsilon}{2E}}
=\frac{\Delta}{\sqrt{2E(E+\varepsilon)}}.}
$$

These obey $u^2+v^2=1$, $u^2-v^2=\varepsilon/E$ and $2uv=\Delta/E$. Equivalently $u=\cos\theta$, $v=\sin\theta$ with $0<\theta<\pi/4$ and $\tan(2\theta)=\Delta/\varepsilon$. The coefficient of $P$ vanishes, while the coefficient of $Q$ is $E$. The constant is

$$
2\varepsilon v^2-2\Delta uv
=\varepsilon\left(1-\frac\varepsilon E\right)-\frac{\Delta^2}{E}
=\varepsilon-E.
$$

Thus the diagonalized [two-mode fermion pairing Hamiltonian](../../../../two-orbital-fermionic-pairing-hamiltonian.md) is

$$
\boxed{H=E(c^\dagger c+d^\dagger d)+\varepsilon-E,
\qquad \lambda=\sqrt{\varepsilon^2+\Delta^2},\quad
\mu=\varepsilon-\sqrt{\varepsilon^2+\Delta^2}.}
$$

The two transformed [fermionic occupation numbers](../../../../fermionic-occupation-number.md) independently take values zero or one. The [energy eigenvalues](../../../../energy-eigenvalue-split.md) and their [eigenspace](../../../../eigenspace.md) dimensions are therefore

$$
\boxed{\begin{array}{c|c|c}
n_c+n_d&\text{energy}&\text{degeneracy}\\\hline
0&\varepsilon-E&1\\
1&\varepsilon&2\\
2&\varepsilon+E&1
\end{array}}
$$

The positive [quasiparticle](../../../../quasiparticle.md) [energy](../../../../energy-split.md) $E$ makes the transformed [vacuum state](../../../../vacuum-state.md) the unique [ground state](../../../../ground-state.md). The constant $\mu$ is essential for the correct [ground-state energy](../../../../ground-state-energy.md).

As a separate sign and spectrum check, use the original [fermionic Fock space](../../../../fermionic-fock-space.md) basis. Both singly occupied states are [energy eigenstates](../../../../energy-eigenstate.md) with [energy](../../../../energy-split.md) $\varepsilon$, since the pairing terms annihilate them. In the ordered even-[fermion parity](../../../../fermion-parity.md) basis $(|0\rangle,a^\dagger b^\dagger|0\rangle)$,

$$
H_{\mathrm{even}}=
\begin{pmatrix}0&-\Delta\\-\Delta&2\varepsilon\end{pmatrix}.
$$

The off-diagonal signs follow from $b^\dagger a^\dagger=-a^\dagger b^\dagger$ and $ab\,a^\dagger b^\dagger|0\rangle=-|0\rangle$. Its [characteristic polynomial](../../../../characteristic-polynomial.md) is $z^2-2\varepsilon z-\Delta^2$, giving the remaining two [eigenvalues](../../../../eigenvalue.md) $\varepsilon\pm E$, in agreement with the [Bogoliubov transformation](../../../../bogoliubov-transformation.md).

## ↑ Ancestors (12)

1. [C](../c.md)
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
