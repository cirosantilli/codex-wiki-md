# HHL controlled reciprocal rotation

↑ **Parent:** [HHL algorithm](hhl-algorithm.md)

On a positive [eigenvalue](eigenvalue.md) label $\lambda$ and a clean [quantum ancilla](quantum-ancilla.md), the [HHL algorithm](hhl-algorithm.md) applies a [quantum variable rotation](quantum-variable-rotation.md) with angle $\theta_\lambda=\arcsin(c/\lambda)$, where $0<c\leq\lambda_{\min}$:

$$
|\lambda\rangle|0\rangle\longmapsto|\lambda\rangle\left(\sqrt{1-c^2/\lambda^2}|0\rangle+\frac c\lambda|1\rangle\right).
$$

[Uncomputation](uncomputation.md) of the eigenvalue register followed by conditioning on flag one multiplies each input [eigenvector](eigenvector.md) amplitude by $c/\lambda$. If $|b\rangle$ is normalized, the success probability is $c^2\|A^{-1}|b\rangle\|^2$. Choosing $c=\lambda_{\max}/\kappa$ from a valid [condition number](condition-number.md) bound gives success probability at least $1/\kappa^2$.

## ↑ Ancestors (5)

1. [HHL algorithm](hhl-algorithm.md)
2. [Quantum theory](quantum-theory-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Binary-angle implementation of a quantum variable rotation](binary-angle-implementation-of-a-quantum-variable-rotation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-324/4/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-324/4/a/ii/solution.md)
