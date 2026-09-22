<h1 id="s03/3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Replacing $L$ by the [angular momentum operator](../../../../../angular-momentum-operator-split.md) gives the [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md)

$$
\hat H=\frac{\hat L^2}{2I}=-\frac{\hbar^2}{2I}\frac{\partial^2}{\partial\phi^2}.
$$

The time-dependent [Schrödinger equation](../../../../../schrodinger-equation.md) is therefore

$$
\boxed{i\hbar\frac{\partial\Psi}{\partial t}=-\frac{\hbar^2}{2mr^2}\frac{\partial^2\Psi}{\partial\phi^2}.}
$$

For a [stationary state](../../../../../stationary-state.md), separate variables as $\Psi(\phi,t)=\psi(\phi)T(t)$. Dividing by the product separates a function of $t$ from one of $\phi$:

$$
i\hbar\frac{\dot T}{T}=-\frac{\hbar^2}{2I}\frac{\psi''}{\psi}=E.
$$

Thus $T=e^{-iEt/\hbar}$ up to a constant, and the time-independent [Schrödinger equation](../../../../../schrodinger-equation.md) is $-\hbar^2\psi''/(2I)=E\psi$.

Diagonalize the commuting [angular momentum operator](../../../../../angular-momentum-operator-split.md) at the same time: $-i\hbar\psi'=\ell\psi$ has solutions $Ae^{i\ell\phi/\hbar}$. A [single-valued wavefunction](../../../../../single-valued-wavefunction.md) requires $e^{2\pi i\ell/\hbar}=1$, hence $\ell=n\hbar$ with $n\in\mathbb Z$. Normalizing with the angular probability measure $d\phi$ gives

$$
\int_0^{2\pi}|A|^2\,d\phi=1,\qquad
\boxed{\psi_n(\phi)=\frac{e^{in\phi}}{\sqrt{2\pi}},\qquad
\Psi_n(\phi,t)=\frac{e^{in\phi-iE_nt/\hbar}}{\sqrt{2\pi}},\quad n\in\mathbb Z.}
$$

These form an [orthonormal basis](../../../../../orthonormal-basis.md) under $\int_0^{2\pi}\psi_m^*\psi_n\,d\phi=\delta_{mn}$. The [periodic boundary conditions](../../../../../periodic-boundary-conditions.md) apply to both the [wavefunction](../../../../../wave-function-split.md) and its first [derivative](../../../../../derivative.md), ensuring the physical self-adjoint [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md). For probability per [arc length](../../../../../arc-length.md) $ds=r\,d\phi$, the normalization instead reads $\psi_n=e^{in\phi}/\sqrt{2\pi r}$; the two conventions describe the same probabilities. General states are [superpositions](../../../../../superposition-principle.md) of these [energy eigenstates](../../../../../energy-eigenstate.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [3](../../3.md)
3. [S03](../../../s03.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the short options paper of the physics Prelims of the University of Oxford](../../../../split.md)
6. [Short options paper of the physics Prelims of the University of Oxford](../../../../../short-options-paper-of-the-physics-prelims-of-the-university-of-oxford.md)
7. [Year 1 of the physics course of the University of Oxford](../../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
