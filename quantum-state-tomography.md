# Quantum state tomography

↑ **Parent:** [Measurement in quantum mechanics](quantum-measurement-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_state_tomography)

[Quantum state tomography](quantum-state-tomography.md) estimates a [density operator](density-matrix-split.md) from measurement frequencies on many independently and identically prepared systems. One fixed [projective measurement](projective-measurement.md) reveals only its basis populations, so further measurement settings are generally needed. For a [qubit](qubit.md), write

$$
\rho=\tfrac12(I+r_xX+r_yY+r_zZ),\qquad
r_j=\operatorname{Tr}(\rho\sigma_j)=p_{j,+}-p_{j,-}.
$$

The three [Pauli matrices](pauli-matrices.md) thus turn measured [expectation values](expectation-value.md) into the [Bloch vector](bloch-vector.md). This reconstruction uses the [Bloch ball](bloch-ball.md) representation of arbitrary [qubit](qubit.md) [density operators](density-matrix-split.md). [Preskill, Quantum Information, §2.3.2](https://www.preskill.caltech.edu/ph219/chap2_15.pdf).

Divide the prepared ensemble into groups measured in the $X$, $Y$ and $Z$ bases. For example, positive-outcome frequencies $0.8,0.5,0.9$ give the estimate $\mathbf r=(0.6,0,0.8)$ and

$$
\rho=\begin{pmatrix}0.9&0.3\\0.3&0.1\end{pmatrix}.
$$

Here $|\mathbf r|=1$, so the reconstructed state is the [pure state](pure-state.md) $(3|0\rangle+|1\rangle)/\sqrt{10}$. Its $Z$ frequencies alone also fit the diagonal [mixed state](mixed-state.md) with populations $0.9,0.1$; the $X$ data distinguish them. For the angular [pure state](pure-state.md) in [measurement in quantum mechanics](quantum-measurement-split.md), $r_x=\sin\theta\cos\phi$, $r_y=\sin\theta\sin\phi$ and $r_z=\cos\theta$, so $Y$ resolves the sign of the phase that $X$ alone cannot.

Finite samples introduce statistical uncertainty: with $N$ independent binary trials in one basis, the frequency has [variance](variance-split.md) $p(1-p)/N$. At $p=1/2$ and $N=100$, its [standard deviation](standard-deviation.md) is $0.05$. Fluctuations can place a naive [Bloch vector](bloch-vector.md) estimate outside the [Bloch ball](bloch-ball.md); a physical reconstruction must enforce positivity of the [density operator](density-matrix-split.md). Repeated measurements on one unprepared specimen sample its changing conditional state, rather than independent copies of its original state. Multiple bases are needed in this projective protocol; a single fixed [informationally complete POVM](informationally-complete-povm.md), such as the [tetrahedral qubit POVM](tetrahedral-qubit-povm.md), is an alternative. It still requires an ensemble of trials.

**Table of contents**

- [Interferometric polarization tomography](interferometric-polarization-tomography.md)
- [Single-qubit process tomography](single-qubit-process-tomography.md)

## ↑ Ancestors (5)

1. [Measurement in quantum mechanics](quantum-measurement-split.md)
2. [Quantum theory](quantum-theory-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (11)

- [Informationally complete POVM](informationally-complete-povm.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-52/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-325/1/solution.md)
- [Polarization preparation and dephasing experiment](polarization-preparation-and-dephasing-experiment.md)
- [Projective measurement](projective-measurement.md)
- [Quantum information](quantum-information.md)
- [Measurement in quantum mechanics](quantum-measurement-split.md)
- [Quantum state](quantum-state.md)
- [Quantum state tomography](quantum-state-tomography.md)
- [Qubit](qubit.md)
- [Qubit state](qubit-state.md)
