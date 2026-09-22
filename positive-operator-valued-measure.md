# Positive operator-valued measure

↑ **Parent:** [Generalized measurement postulate](generalized-measurement-postulate.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Positive_operator-valued_measure)

A [positive operator-valued measure](positive-operator-valued-measure.md) is a family of [positive operators](positive-operator.md) $E_i$ satisfying $\sum_i E_i=I$. Each $E_i$ is called an effect and determines a [probability](probability.md) $p_i=\operatorname{Tr}(E_i\rho)$ for input [density operator](density-matrix-split.md) $\rho$. The effects need not be [orthogonal projections](orthogonal-projection.md) or commute. This permits measurements with more outcomes than the dimension of the [Hilbert space](hilbert-space-split.md), such as the [trine qubit POVM](trine-qubit-povm.md). Coupling to a [quantum ancilla](quantum-ancilla.md) and measuring the larger system supplies a physical route to generalized measurements. [Preskill, Quantum Information, §§3.1.2–3.1.4](https://www.preskill.caltech.edu/ph229/notes/chap3.pdf).

For an elementary unsharp $Z$ example on a [qubit](qubit.md), take

$$
E_\pm=\frac12(I\pm\eta Z),\qquad 0\leq\eta\leq1.
$$

On the [eigenstate](eigenstate.md) $|0\rangle$, $p_\pm=(1\pm\eta)/2$; at $\eta=1/2$ they are $3/4$ and $1/4$. At $\eta=0$ the outcome is a fair coin independent of the input, and at $\eta=1$ these effects specify a sharp $Z$ [projective measurement](projective-measurement.md). Choosing $K_\pm=\sqrt{E_\pm}$ specifies one [quantum instrument](quantum-instrument.md), but $U_\pm\sqrt{E_\pm}$ for outcome-dependent [unitary operators](unitary-operator.md) has the same effects and different state updates. Thus [POVM does not determine the post-measurement state](povm-does-not-determine-the-post-measurement-state.md).

**Table of contents**

- [POVM on the occupied support](povm-on-the-occupied-support.md)
- [POVM–ensemble duality for the maximally mixed state](povm-ensemble-duality-for-the-maximally-mixed-state.md)
- [Pure positive operator-valued measure](pure-positive-operator-valued-measure.md)
- [Trine qubit POVM](trine-qubit-povm.md)
- [Informationally complete POVM](informationally-complete-povm.md)
  - [Tetrahedral qubit POVM](tetrahedral-qubit-povm.md)
- [Binary rank-one qubit POVM](binary-rank-one-qubit-povm.md)

## ↑ Ancestors (6)

1. [Generalized measurement postulate](generalized-measurement-postulate.md)
2. [Measurement in quantum mechanics](quantum-measurement-split.md)
3. [Quantum theory](quantum-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (13)

- [Born statistical scattering interpretation](born-statistical-scattering-interpretation.md)
- [Local-energy measurement verification](local-energy-measurement-verification.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-61/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-33/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-58/3/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-48/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-51/2/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-67/3/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-323/5/a/i/solution.md)
- [Solution](past-exam-of-the-quantum-information-course-of-the-university-of-cambridge/2012/paper-1/3/a/solution.md)
- [Perfect discrimination of pure states requires orthogonality](perfect-discrimination-of-pure-states-requires-orthogonality.md)
- [Positive operator-valued measure](positive-operator-valued-measure.md)
- [Measurement in quantum mechanics](quantum-measurement-split.md)
