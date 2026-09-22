# Dyadic quantum Fourier transform circuit

↑ **Parent:** [Quantum Fourier transform](quantum-fourier-transform.md)

In most-significant-bit-first order, let $x=x_1\cdots x_n$ and $0.x_j\cdots x_n=\sum_{l=j}^n x_l2^{-(l-j+1)}$. On a [computational-basis state](computational-basis-state.md), process wire $j$ with a [Hadamard gate](hadamard-gate.md), then [controlled phase gates](controlled-phase-gate.md) $R_{l-j+1}$ controlled by unprocessed wire $l$ for each $l>j$. Wire $j$ becomes $(|0\rangle+e^{2\pi i0.x_j\cdots x_n}|1\rangle)/\sqrt2$. Reversing the final wire order yields the positive-exponent [quantum Fourier transform](quantum-fourier-transform.md). There are $n$ [Hadamard gates](hadamard-gate.md) and $n(n-1)/2$ [controlled phase gates](controlled-phase-gate.md). Physical reversal costs $\lfloor n/2\rfloor$ [swap operators](swap-operator.md), each expressible as three [controlled-NOT gates](controlled-not-gate.md), themselves implemented with [Hadamard gates](hadamard-gate.md) and a [Controlled-Z gate](controlled-z-gate.md). Thus the entire construction uses $O(n^2)$ gates from the specified family.

## ↑ Ancestors (5)

1. [Quantum Fourier transform](quantum-fourier-transform.md)
2. [Quantum theory](quantum-theory-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-25/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-47/4/solution.md)
