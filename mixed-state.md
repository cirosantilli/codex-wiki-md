# Mixed state

↑ **Parent:** [Density matrix](density-matrix.md)

A mixed state is a [density operator](density-matrix.md) that is not a rank-one [orthogonal projection](orthogonal-projection.md). In finite [dimension](dimension-vector-space.md) it is characterized by $\operatorname{Tr}(\rho^2)<1$, so its [purity of a density operator](purity-of-a-density-operator.md) distinguishes it from a [pure state](pure-state.md).

Compare a [pure state](pure-state.md) [quantum superposition](quantum-superposition.md) with an equal classical choice between two [computational-basis states](computational-basis-state.md) of a [qubit](qubit.md):

$$
|+\rangle=\frac{|0\rangle+|1\rangle}{\sqrt2},\qquad
\rho_+=|+\rangle\langle+|=\frac12\begin{pmatrix}1&1\\1&1\end{pmatrix},\qquad
\rho_{\mathrm{mix}}=\frac12|0\rangle\langle0|+\frac12|1\rangle\langle1|=\frac I2.
$$

A $Z$ [projective measurement](projective-measurement.md) in the [computational basis](computational-basis.md) gives $P(0)=P(1)=1/2$ for both [density operators](density-matrix.md). An $X$ [projective measurement](projective-measurement.md) in the [Hadamard basis](hadamard-basis.md) $|\pm\rangle=(|0\rangle\pm|1\rangle)/\sqrt2$ distinguishes them: the [Born rule](born-rule.md) gives $P(+)=1$ for $\rho_+$ and $P(+)=1/2$ for $\rho_{\mathrm{mix}}$. These comparisons use separate copies of each preparation; measuring $Z$ first changes the state tested by a subsequent $X$ measurement.

<a id="image-equal-computational-basis-populations-can-hide-different-coherence-and-x-measurement-statistics"></a>
![](density-matrix-coherence-versus-mixture.png)

**[Figure 3](#image-equal-computational-basis-populations-can-hide-different-coherence-and-x-measurement-statistics). Equal computational-basis populations can hide different coherence and X-measurement statistics**.

The off-diagonal entries of $\rho_+$ encode [quantum coherence](quantum-coherence-in-a-specified-basis.md) in the [computational basis](computational-basis.md). Such [quantum coherence](quantum-coherence-in-a-specified-basis.md) depends on the [basis](basis.md): $\rho_+$ is diagonal in the [Hadamard basis](hadamard-basis.md) but remains a [pure state](pure-state.md). Mixedness is independent of the [basis](basis.md), because a [unitary](unitary-connection.md) change of [basis](basis.md) preserves the [eigenvalues](eigenvalue.md) and the [purity of a density operator](purity-of-a-density-operator.md).

Even the [quantum state ensemble](quantum-state-ensemble.md) is not unique:

$$
\frac I2=\frac12|0\rangle\langle0|+\frac12|1\rangle\langle1|
=\frac12|+\rangle\langle+|+\frac12|-\rangle\langle-|.
$$

The off-diagonal entries of the two [Hadamard basis](hadamard-basis.md) projectors cancel. Thus the [density operator](density-matrix.md) retains precisely what measurements on the system can reveal, while an accessible preparation label carries additional information. A [mixed state](mixed-state.md) can also be the [reduced density matrix](reduced-density-matrix.md) of an [entangled state](entangled-state.md), even when the whole system is in a [pure state](pure-state.md); classical ignorance about a selected component is not its only physical origin. [Preskill, Physics 229 notes, chapter 2, section 2.3.1, equations (2.54)–(2.60)](https://www.preskill.caltech.edu/ph229/notes/chap2.pdf)

## ↑ Ancestors (5)

1. [Density matrix](density-matrix.md)
2. [Quantum theory](quantum-theory-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (29)

- [Born rule](born-rule.md)
- [Canonical ensemble](canonical-ensemble.md)
- [Density matrix](density-matrix.md)
- [Energy eigenspace](energy-eigenspace.md)
- [Expectation value](expectation-value.md)
- [Fidelity of commuting mixed states](fidelity-of-commuting-mixed-states.md)
- [Fuchs-van de Graaf inequalities](fuchs-van-de-graaf-inequalities.md)
- [Infinite square well](infinite-square-well.md)
- [Maximally mixed state](maximally-mixed-state.md)
- [Measurement characterization of quantum fidelity](measurement-characterization-of-quantum-fidelity.md)
- [Mixed state](mixed-state.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-60/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-60/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-60/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-52/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-52/2/f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-53/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-53/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-324/3/b/ii/solution.md)
- [Pure-state trace distance and fidelity identity](pure-state-trace-distance-and-fidelity-identity.md)
- [Purity of a density operator](purity-of-a-density-operator.md)
- [Quantum state tomography](quantum-state-tomography.md)
- [Quantum superposition](quantum-superposition.md)
- [Quantum theory](quantum-theory-split.md)
- [Qubit](qubit.md)
- [Qubit state](qubit-state.md)
- [Spin expectation value](spin-expectation-value.md)
- [Squared quantum fidelity](squared-quantum-fidelity.md)
- [Trace distance between qubit states](trace-distance-between-qubit-states.md)
