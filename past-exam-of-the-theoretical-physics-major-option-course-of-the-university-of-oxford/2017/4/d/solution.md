<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Choose the current convention corresponding to $\delta\varphi=i\alpha\varphi$. [Noether's theorem](../../../../noether-conserved-quantity-for-a-mechanical-point-symmetry.md) gives

$$
J^\mu=i\bigl[(\partial^\mu\varphi^*)\varphi-\varphi^*\partial^\mu\varphi\bigr]
=\frac{2r^2}{f}\partial^\mu\pi.
$$

For the requested terms with no $\sigma$ and $f=\sqrt2v$, the [Lagrangian](../../../../lagrangian.md) is $\tfrac12(\partial\pi)^2$ and the current becomes $J^\mu=f\partial^\mu\pi$. The supplied covariant oscillator normalization cancels the invariant measure when the [annihilation operator](../../../../annihilation-operator.md) contracts with $a^\dagger(p)$, so

$$
\langle0|\pi(x)|\pi(p)\rangle=e^{-ip\cdot x},\qquad
\boxed{\langle0|J^\mu(x)|\pi(p)\rangle=-ifp^\mu e^{-ip\cdot x}.}
$$

The [momentum](../../../../momentum-split.md) is on the massless shell, $p^2=0$. Differentiating once more therefore gives

$$
\boxed{\langle0|\partial_\mu J^\mu(x)|\pi(p)\rangle=-fp^2e^{-ip\cdot x}=0.}
$$

This [Goldstone current matrix element in a phase-only scalar theory](../../../../goldstone-current-matrix-element-in-a-phase-only-scalar-theory.md) shows that a conserved current can have a nonzero [matrix](../../../../matrix.md) element proportional to a null [momentum](../../../../momentum-split.md). Thus current conservation is fully consistent with the current creating a massless one-particle state from the [vacuum](../../../../vacuum.md); the nonzero coefficient $f$ is its Goldstone-current [coupling](../../../../coupling.md). It is the divergence that vanishes, not the current [matrix](../../../../matrix.md) element. Reversing the current convention reverses the nonzero [matrix](../../../../matrix.md) element but leaves this zero divergence unchanged.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
