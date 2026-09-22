<h1 id="section-vi/7/unlettered-1/solution">Solution</h1>

↑ **Parent:** [Unlettered 1](../unlettered-1.md)

Normalize the [plane waves](../../../../../plane-wave.md) in a periodic crystal of area or volume $\mathcal V$. The [Fourier coefficients](../../../../../fourier-coefficient.md) of the [periodic potential](../../../../../periodic-potential.md) obey

$$
\langle\mathbf k|V|\mathbf k'\rangle=\frac1{\mathcal V}\int_{\mathcal V}V(\mathbf r)e^{-i(\mathbf k-\mathbf k')\cdot\mathbf r}\,d\mathbf r=V_{\mathbf k-\mathbf k'}.
$$

Translation of the integral by any [lattice vector](../../../../../lattice-vector.md) $\mathbf R$ leaves it invariant but multiplies it by $e^{-i(\mathbf k-\mathbf k')\cdot\mathbf R}$. A nonzero result therefore requires $\mathbf k-\mathbf k'$ to be a [reciprocal lattice vector](../../../../../reciprocal-lattice-vector.md).

Near an isolated [Bragg scattering](../../../../../bragg-scattering.md) degeneracy, ordinary nondegenerate [perturbation theory](../../../../../perturbation-theory.md) fails because the free energies coincide. Retain the resonant [plane waves](../../../../../plane-wave.md) $|\mathbf k\rangle$, $|\mathbf k+\mathbf G\rangle$ and apply [degenerate perturbation theory](../../../../../degenerate-perturbation-theory.md). Absorb the constant $V_{\mathbf0}$ into the energy origin. Since a real potential has $V_{-\mathbf G}=V_{\mathbf G}^*$, the projected [Schrödinger equation](../../../../../schrodinger-equation.md) has coefficient matrix

$$
\begin{pmatrix}
\epsilon_0(\mathbf k)-E&V_{-\mathbf G}\\
V_{\mathbf G}&\epsilon_0(\mathbf k+\mathbf G)-E
\end{pmatrix}.
$$

A nonzero eigenstate requires

$$
\boxed{[\epsilon_0(\mathbf k)-E][\epsilon_0(\mathbf k+\mathbf G)-E]-|V_{\mathbf G}|^2=0.}
$$

Off-resonant [plane waves](../../../../../plane-wave.md) give higher-order energy shifts omitted in this leading [nearly-free electron model](../../../../../nearly-free-electron-model.md).

## ↑ Ancestors (13)

1. [Unlettered 1](../unlettered-1.md)
2. [7](../../7.md)
3. [Section VI](../../../section-vi.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the general relativity and cosmology and condensed matter physics paper of Part B of the physics course of the University of Oxford](../../../../split.md)
6. [General relativity and cosmology and condensed matter physics paper of Part B of the physics course of the University of Oxford](../../../../../general-relativity-and-cosmology-and-condensed-matter-physics-paper-of-part-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Year 3 of the physics course of the University of Oxford](../../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
