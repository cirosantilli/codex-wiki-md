# Near-grid quantum phase estimation

↑ **Parent:** [Quantum phase estimation](quantum-phase-estimation.md)

For register size $N=2^t$ and [eigenphase](eigenphase.md) $\phi=2\pi n/N+\epsilon$, the amplitude of decoded label $m$ is $N^{-1}\sum_{k=0}^{N-1}e^{ik(\phi-2\pi m/N)}$. The [finite geometric series](finite-geometric-series.md) gives $P(n)=\sin^2(N\epsilon/2)/[N^2\sin^2(\epsilon/2)]$. If $N|\epsilon|\ll1$, this is $1-(N^2-1)\epsilon^2/12+O(N^4\epsilon^4)$. Thus the nearest exactly representable phase is returned with [probability](probability.md) near one, not with certainty unless the offset vanishes.

// Target: quantum-error-correction.bigb

## ↑ Ancestors (6)

1. [Quantum phase estimation](quantum-phase-estimation.md)
2. [Quantum Fourier transform](quantum-fourier-transform.md)
3. [Quantum theory](quantum-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-58/2/ii/solution.md)
