# Expectation value

↑ **Parent:** [Observable](observable.md)

The [expectation value](expectation-value.md) of a [quantum observable](observable.md) is the [expected value](expected-value.md) of its measurement outcome [random variable](random-variable-split.md) in a specified [quantum state](quantum-state.md). It predicts the mean of outcomes from many identical [quantum state preparations](quantum-state-preparation.md). It need not equal any one possible outcome: for a [spin one-half](spin-one-half.md) particle, equal [probabilities](probability.md) of $+\hbar/2$ and $-\hbar/2$ give mean zero even though zero is never an outcome of that [spin](spin.md) component. Here $\hbar$ is the reduced [Planck constant](planck-constant.md).

Let $A=A^\dagger$ be a [Hermitian operator](hermitian-operator.md) on a finite-dimensional [Hilbert space](hilbert-space-split.md), and let $|\psi\rangle$ be a normalized [pure state](pure-state.md), $\langle\psi|\psi\rangle=1$. The [spectral theorem](spectral-theorem.md) writes

$$
A=\sum_r a_rP_r,\qquad P_rP_s=\delta_{rs}P_r,\qquad \sum_rP_r=I.
$$

The $a_r$ are distinct real [eigenvalues](eigenvalue.md), $P_r$ are [orthogonal projections](orthogonal-projection.md) onto their [eigenspaces](eigenspace.md), and $I$ is the [identity operator](identity-operator.md). For an ideal [projective measurement](projective-measurement.md) of $A$, the [Born rule](born-rule.md) and the [expectation value](expectation-value.md) give

$$
p_r=\langle\psi|P_r|\psi\rangle=\|P_r|\psi\rangle\|^2,\qquad
\sum_rp_r=1,\qquad
\langle A\rangle_\psi=\sum_ra_rp_r=\langle\psi|A|\psi\rangle.
$$

Thus the [expectation value](expectation-value.md) is a [probability](probability.md)-weighted average of [eigenvalues](eigenvalue.md), including all vectors in a degenerate [eigenspace](eigenspace.md) in its $P_r$. In an [orthonormal eigenbasis](orthonormal-eigenbasis.md), $|\psi\rangle=\sum_jc_j|j\rangle$, this is $\sum_j a_j|c_j|^2$, where repeated $a_j$ are allowed. The weighted average lies between the smallest and largest [eigenvalues](eigenvalue.md); it can lie in a gap between them. The statistical meaning and operator expression are connected in this way in the authored treatment of average energies.[The Feynman Lectures on Physics, Volume III, Chapter 20: Operators, §20–2, equations (20.11)–(20.20): outcome frequencies, weighted mean, and operator expectation](the-feynman-lectures-on-physics-volume-iii-by-richard-feynman-and-others/chapter-20-operators.md)

If a nonzero [vector](vector.md) $|v\rangle$ has not been normalized, use $\langle v|A|v\rangle/\langle v|v\rangle$; the denominator is essential. A [global phase](global-phase.md) cancels between the bra and ket, so $|\psi\rangle$ and $e^{i\gamma}|\psi\rangle$ have the same [expectation value](expectation-value.md) and outcome [probabilities](probability.md).

The outcome [variance](variance-split.md) measures the spread about this mean, whereas the [quantum uncertainty](quantum-uncertainty.md) is its [standard deviation](standard-deviation.md):

$$
\operatorname{Var}_\psi(A)=\sum_rp_r(a_r-\langle A\rangle_\psi)^2
=\langle A^2\rangle_\psi-\langle A\rangle_\psi^2
=(\Delta A)^2.
$$

For a [pure state](pure-state.md), zero [variance](variance-split.md) means that $|\psi\rangle$ lies entirely in one [eigenspace](eigenspace.md). That [eigenspace](eigenspace.md) need not be one-dimensional. Knowing only a mean generally does not determine the entire outcome [probability distribution](probability-distribution.md).

For a [mixed state](mixed-state.md), the same formulas use its [density matrix](density-matrix.md) $\rho$, a [positive operator](positive-operator.md) with [trace](matrix-trace.md) one:

$$
p_r=\operatorname{Tr}(\rho P_r),\qquad
\langle A\rangle_\rho=\operatorname{Tr}(\rho A),\qquad
\operatorname{Var}_\rho(A)=\operatorname{Tr}(\rho A^2)-\operatorname{Tr}(\rho A)^2.
$$

A [pure state](pure-state.md) is the special case $\rho=|\psi\rangle\langle\psi|$. For a [quantum state ensemble](quantum-state-ensemble.md) $\rho=\sum_kw_k\rho_k$, the [expectation value](expectation-value.md) is $\sum_kw_k\langle A\rangle_{\rho_k}$. This linearity is useful when preparations vary between trials; different [quantum state ensembles](quantum-state-ensemble.md) can have the same [density matrix](density-matrix.md).

These formulas require no operator-domain qualifications in finite dimension. For an unbounded [self-adjoint operator](self-adjoint-operator.md), the [spectral theorem](spectral-theorem.md) instead gives a spectral [probability measure](probability-measure.md); a finite mean requires an integrable absolute first moment, and finite [variance](variance-split.md) requires a finite second moment. Writing $\langle\psi|A|\psi\rangle$ as an operator [inner product](inner-product.md) additionally requires $|\psi\rangle$ in the [operator domain](operator-domain.md) of $A$. The [quadratic form of a positive quantum Hamiltonian](quadratic-form-of-a-positive-quantum-hamiltonian.md) explains the useful wider form-domain version.

**Table of contents**

- [Spin expectation value](spin-expectation-value.md)
- [Estimating a quantum expectation value](estimating-a-quantum-expectation-value.md)
  - [Stern-Gerlach expectation estimation](stern-gerlach-expectation-estimation.md)

## ↑ Ancestors (7)

1. [Observable](observable.md)
2. [Quantum state](quantum-state.md)
3. [Quantum system](quantum-system.md)
4. [Quantum mechanics](quantum-mechanics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (42)

- [Energy eigenspace](energy-eigenspace.md)
- [Energy eigenvalue](energy-eigenvalue.md)
- [Energy form of a half-well sine state](energy-form-of-a-half-well-sine-state.md)
- [Equality case of the Heisenberg uncertainty relation](equality-case-of-the-heisenberg-uncertainty-relation.md)
- [Estimating a quantum expectation value](estimating-a-quantum-expectation-value.md)
- [Excited state](excited-state.md)
- [Exclusion versus particle position](exclusion-versus-particle-position.md)
- [Expectation value](expectation-value.md)
- [Ground state](ground-state.md)
- [Heisenberg uncertainty relation](heisenberg-uncertainty-relation.md)
- [One-point correlation function](one-point-correlation-function.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-1/18f/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-2/9f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-2/18d/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-1/18a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-3/7g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-54/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-54/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-4/6b/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-3/7b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-4/6a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-61/3/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-61/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-57/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-4/6b/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-3/16b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ib/paper-1/15a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-1/14b/f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-324/1/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-4/4d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-2/35b/a/solution.md)
- [Pauli correlation tensor](pauli-correlation-tensor.md)
- [Quadratic form of a positive quantum Hamiltonian](quadratic-form-of-a-positive-quantum-hamiltonian.md)
- [Quadratic-norm proof of the Heisenberg uncertainty relation](quadratic-norm-proof-of-the-heisenberg-uncertainty-relation.md)
- [Quantum state tomography](quantum-state-tomography.md)
- [Quantum variational principle](quantum-variational-principle.md)
- [Radius deformation as a Higgs mechanism](radius-deformation-as-a-higgs-mechanism.md)
- [Robertson uncertainty principle](robertson-uncertainty-principle.md)
- [Spin expectation value](spin-expectation-value.md)
- [Spin uncertainty state dependence](spin-uncertainty-state-dependence.md)
- [Stern-Gerlach experiment](stern-gerlach-experiment.md)
- [Variational method](variational-method.md)
