# Quantum phase estimation with a maximally mixed target

↑ **Parent:** [Quantum phase estimation](quantum-phase-estimation.md)

For a $d$-dimensional [unitary operator](unitary-operator.md) $V=\sum_{j=1}^de^{i\phi_j}|v_j\rangle\langle v_j|$, a [maximally mixed state](maximally-mixed-state.md) $I/d$ on its target is the equal mixture of these [orthonormal](orthonormal-set.md) [eigenvectors](eigenvector.md). Therefore [quantum phase estimation](quantum-phase-estimation.md) with register size $L$ produces label $m$ with [probability](probability.md)

$$
p(m)=\frac1d\sum_{j=1}^d|a_m(\phi_j)|^2,\qquad a_m(\phi)=\frac1L\sum_{x=0}^{L-1}e^{ix(\phi-2\pi m/L)}.
$$

This follows by [linearity](linearity.md) of [unitary time evolution](unitary-time-evolution.md) and the [Born rule](born-rule.md) on the spectral mixture. If every [eigenphase](eigenphase.md) has an exact $L$-grid label, that label has [probability](probability.md) equal to its multiplicity divided by $d$. Otherwise the exact distribution has tails, and the nearest labels are guaranteed only the [nearest-integer success bound for quantum phase estimation](nearest-integer-success-bound-for-quantum-phase-estimation.md) weighted by the corresponding spectral [probabilities](probability.md).

## ↑ Ancestors (6)

1. [Quantum phase estimation](quantum-phase-estimation.md)
2. [Quantum Fourier transform](quantum-fourier-transform.md)
3. [Quantum theory](quantum-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-57/4/c/solution.md)
