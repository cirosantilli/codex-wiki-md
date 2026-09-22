# Nearest-integer success bound for quantum phase estimation

↑ **Parent:** [Quantum phase estimation](quantum-phase-estimation.md)

For a [unitary operator](unitary-operator.md) [eigenphase](eigenphase.md) $\phi$, an $n$-qubit [quantum phase estimation](quantum-phase-estimation.md) register of size $L=2^n$ has output [probability amplitude](probability-amplitude.md)

$$
a_m(\phi)=\frac1L\sum_{x=0}^{L-1}e^{ix(\phi-2\pi m/L)}.
$$

Choose the nearest integer label $m$ to $L\phi/(2\pi)$, with labels understood modulo $L$, and put $d=L\phi/(2\pi)-m$, taking the representative $|d|\leq1/2$. The [finite geometric series](finite-geometric-series.md) gives $|a_m|=|\sin(\pi d)|/[L|\sin(\pi d/L)|]$. For $0<|d|\leq1/2$, [concavity](concave-function.md) of sine gives $|\sin(\pi d)|\geq2|d|$, while $|\sin(\pi d/L)|\leq\pi|d|/L$. Thus the [probability](probability.md) of the nearest label is at least $4/\pi^2$. At $d=0$ it is exactly one. If two labels tie for nearest, each satisfies the bound.

## ↑ Ancestors (6)

1. [Quantum phase estimation](quantum-phase-estimation.md)
2. [Quantum Fourier transform](quantum-fourier-transform.md)
3. [Quantum theory](quantum-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-33/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-57/4/b/solution.md)
- [Quantum phase estimation with a maximally mixed target](quantum-phase-estimation-with-a-maximally-mixed-target.md)
