<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a normalized [orbital](../../../../single-particle-orbital.md) $\int d^2r\,|\phi|^2=1$, the symmetric [Hartree product state](../../../../hartree-product-state.md) and its equivalent [Fock space](../../../../fock-space.md) form are

$$
\boxed{\Phi(\mathbf r_1,\ldots,\mathbf r_N)=\prod_{j=1}^N\phi(\mathbf r_j),\qquad
|N:\phi\rangle=\frac{(a_\phi^\dagger)^N}{\sqrt{N!}}|0\rangle,\quad
a_\phi^\dagger=\int d^2r\,\phi(\mathbf r)\psi^\dagger(\mathbf r).}
$$

There are exactly $N(N-1)/2$ interacting pairs, so the [expectation value](../../../../expectation-value.md) of the grand [Hamiltonian](../../../../hamiltonian.md) is the [functional](../../../../functional.md)

$$
\boxed{\mathcal E_\mu[\phi]=N\int d^2r\left[\frac{\hbar^2}{2m}|\nabla\phi|^2+\frac\kappa2r^2|\phi|^2\right]
+\frac{gN(N-1)}2\int d^2r\,|\phi|^4-\mu N.}
$$

At fixed $N$ the term $-\mu N$ is constant. Enforce [wavefunction normalization](../../../../wavefunction-normalization.md) separately by varying $\mathcal E_\mu-N\eta(\int|\phi|^2-1)$ with respect to $\phi^*$. The resulting stationary [Gross–Pitaevskii equation](../../../../gross-pitaevskii-equation.md) for the normalized [orbital](../../../../single-particle-orbital.md) is

$$
\boxed{\left[-\frac{\hbar^2}{2m}\nabla^2+\frac\kappa2r^2+g(N-1)|\phi|^2\right]\phi=\eta\phi.}
$$

The [Lagrange multiplier](../../../../lagrange-multiplier.md) $\eta$ enforces the norm; fixed-$N$ variation cannot identify it with the independently inserted [chemical potential](../../../../chemical-potential-split.md) merely by differentiating the constant $-\mu N$.

For the standard large-$N$ convention put $\Psi=\sqrt N\phi$, so $n=|\Psi|^2$ and $\int n=N$, and replace $N-1$ by $N$. Varying the resulting grand [energy](../../../../energy-split.md) [functional](../../../../functional.md)

$$
\int d^2r\left[\frac{\hbar^2}{2m}|\nabla\Psi|^2+\left(\frac\kappa2r^2-\mu\right)|\Psi|^2+\frac g2|\Psi|^4\right]
$$

with unrestricted $\Psi$ gives

$$
\boxed{\left[-\frac{\hbar^2}{2m}\nabla^2+\frac\kappa2r^2+g|\Psi|^2\right]\Psi=\mu\Psi.}
$$

Equivalently, at fixed $N$ this same $\mu$ is chosen as the normalization [Lagrange multiplier](../../../../lagrange-multiplier.md). This is the [chemical potential](../../../../chemical-potential-split.md) convention used below. The [contact interaction](../../../../contact-interaction-quantum-mechanics.md) coupling $g$ has dimensions of [energy](../../../../energy-split.md) times area in two dimensions.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the quantum matter course of the University of Oxford](../../../split.md)
5. [Quantum matter course of the University of Oxford](../../../../quantum-matter-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
