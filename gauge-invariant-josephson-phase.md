# Gauge-invariant Josephson phase

↑ **Parent:** [Josephson effect](josephson-effect.md)

Write the superconducting [order parameters](order-parameter.md) as $\psi_j=|\psi_j|e^{i\theta_j}$, using a field of pair [electric charge](electric-charge-split.md) $q=-2e$. For a specified path across the [superconducting weak link](superconducting-weak-link.md), define

$$
\phi=\theta_2-\theta_1-\frac{q}{\hbar}\int_1^2\mathbf A\cdot d\mathbf l
=\theta_2-\theta_1+\frac{2e}{\hbar}\int_1^2\mathbf A\cdot d\mathbf l.
$$

Here $\mathbf A$ is the magnetic [vector potential](vector-potential.md). To check electromagnetic [gauge invariance](gauge-invariance.md), use a scalar function $\chi$ and transform

$$
\mathbf A'=\mathbf A+\nabla\chi,\qquad
\psi_j'=e^{iq\chi_j/\hbar}\psi_j.
$$

The change of $\theta_2-\theta_1$ is $q(\chi_2-\chi_1)/\hbar$, exactly cancelled by the change of the [line integral](line-integral.md). Thus $\phi$ is unchanged although each local [quantum phase](quantum-phase.md) changes. This is the same charge/sign bookkeeping discussed in [gauge-coupling sign in Ginzburg-Landau superconductivity](gauge-coupling-sign-in-ginzburg-landau-superconductivity.md). Different physical paths can enclose [magnetic flux](magnetic-flux.md), so fixing the path matters.

For stationary reservoirs with equal internal pair [chemical potentials](chemical-potential-split.md) and a time-independent [vector potential](vector-potential.md), the local [Schrödinger equation](schrodinger-equation.md) gives $\dot\theta_j=-qU_j/\hbar$ after dropping the common internal term. With [electric potentials](electric-potential.md) $U_j$ and $V=U_2-U_1$, subtraction gives $\dot\phi=-qV/\hbar=2eV/\hbar$. For a general circuit, $V$ denotes the corresponding measured electrochemical voltage and the electromagnetic contribution must be treated consistently. A bare difference of phases without the [vector potential](vector-potential.md) term is insufficient in an arbitrary gauge.

## ↑ Ancestors (7)

1. [Josephson effect](josephson-effect.md)
2. [Josephson junction](josephson-junction.md)
3. [Superconductivity](superconductivity-split.md)
4. [Statistical physics](statistical-physics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Current-biased Josephson phase dynamics](current-biased-josephson-phase-dynamics.md)
- [Current-phase relation of a superconducting weak link](current-phase-relation-of-a-superconducting-weak-link.md)
- [Josephson effect](josephson-effect.md)
- [Josephson junction](josephson-junction.md)
- [Solution](past-exam-of-the-superconductivity-and-quantum-coherence-course-of-the-university-of-cambridge/2013/paper-1/3/solution.md)
- [Solution](past-exam-of-the-superconductivity-and-quantum-coherence-course-of-the-university-of-cambridge/2014/paper-1/1/e/solution.md)
- [Solution](past-exam-of-the-superconductivity-and-quantum-coherence-course-of-the-university-of-cambridge/2015/paper-1/1/a/solution.md)
- [Solution](past-exam-of-the-superconductivity-and-quantum-coherence-course-of-the-university-of-cambridge/2016/paper-1/1/d/solution.md)
- [Tilted Josephson washboard potential](tilted-josephson-washboard-potential.md)
