<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [quantum variational principle](../../../../../quantum-variational-principle.md) turns the ground-state problem into minimization of a [Rayleigh quotient](../../../../../rayleigh-quotient.md):

$$
E[\psi]=\frac{\langle\psi|H|\psi\rangle}{\langle\psi|\psi\rangle}\geq E_0.
$$

The [Hamiltonian](../../../../../hamiltonian.md) must be a [self-adjoint operator](../../../../../self-adjoint-operator.md) bounded below, and the nonzero trial state must have finite form [energy](../../../../../energy-split.md). Expanding a normalized trial state in exact [energy eigenstates](../../../../../energy-eigenstate.md) gives $E[\psi]=\sum_n|c_n|^2E_n$, a weighted average no smaller than $E_0$. Equality requires support only in the ground-state eigenspace. The spectral version also accommodates continuous [spectrum](../../../../../spectrum-functional-analysis.md); a lowest normalizable [eigenstate](../../../../../eigenstate.md) is not required merely to bound the spectral infimum.

The [variational method](../../../../../variational-method.md) chooses a trial family with the correct [boundary conditions](../../../../../boundary-condition.md), [fermionic exchange symmetry](../../../../../fermi-dirac-statistics.md) and other required [quantum numbers](../../../../../quantum-number.md), evaluates its [energy](../../../../../energy-split.md) and minimizes over its parameters. It gives an **upper bound on [ground-state energy](../../../../../ground-state-energy.md)**. Enlarging a nested trial family can only improve or preserve its optimal bound. A low [energy](../../../../../energy-split.md) does not by itself establish a highly accurate [wavefunction](../../../../../wave-function-split.md), especially near degeneracy; [energy](../../../../../energy-split.md) errors are second order in small admixtures orthogonal to a nondegenerate exact [ground state](../../../../../ground-state.md).

For example, a normalized Gaussian trial for a one-dimensional [quantum harmonic oscillator](../../../../../quantum-harmonic-oscillator-split.md) is $\psi_\beta=(\beta/\pi)^{1/4}e^{-\beta x^2/2}$, with $\beta>0$. Its [energy](../../../../../energy-split.md) is

$$
E(\beta)=\frac{\hbar^2\beta}{4m}+\frac{m\omega^2}{4\beta},\qquad
\boxed{\beta_{\rm opt}=m\omega/\hbar,\quad E_{\min}=\hbar\omega/2.}
$$

The two terms balance kinetic localization cost against the potential cost of spreading out. This [Gaussian variational energy for the harmonic oscillator](../../../../../gaussian-variational-energy-for-the-harmonic-oscillator.md) happens to attain the exact answer because the family contains the exact [ground state](../../../../../ground-state.md).

<a id="2/a/image-gaussian-variational-energy-and-its-exact-harmonic-oscillator-minimum"></a>
![](../../../../../past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2015/paper-1-variational.png)

**[Figure 1](#2/a/image-gaussian-variational-energy-and-its-exact-harmonic-oscillator-minimum). Gaussian variational energy and its exact harmonic-oscillator minimum**.

A trial expansion $\psi=\sum_j c_j\chi_j$ in a finite, possibly nonorthogonal basis gives the [generalized eigenvalue problem](../../../../../generalized-eigenvalue-problem.md) $H\mathbf c=ES\mathbf c$, with $H_{ij}=\langle\chi_i|H|\chi_j\rangle$ and $S_{ij}=\langle\chi_i|\chi_j\rangle$. Its lowest Ritz value minimizes the quotient in that subspace. For excited states, the [excited-state variational constraint](../../../../../excited-state-variational-constraint.md) imposes exact [orthogonality](../../../../../orthogonal-vectors.md) to the lower [eigenstates](../../../../../eigenstate.md) to obtain a corresponding upper bound; the [Courant–Fischer min-max principle](../../../../../courant-fischer-min-max-principle.md) yields upper bounds for ordered Ritz [eigenvalues](../../../../../eigenvalue.md) from a common subspace. [orthogonality](../../../../../orthogonal-vectors.md) only to an independently approximate [ground state](../../../../../ground-state.md) does not automatically provide an excited-state bound: residual true-ground-state contamination can lower the trial [energy](../../../../../energy-split.md) below the desired excited [energy](../../../../../energy-split.md). Symmetry can impose exact [orthogonality](../../../../../orthogonal-vectors.md) when the relevant states have different symmetry sectors.

## ↑ Ancestors (14)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the advanced quantum physics course of the University of Cambridge](../../../../split.md)
6. [Advanced Quantum Physics course of the University of Cambridge](../../../../../advanced-quantum-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
