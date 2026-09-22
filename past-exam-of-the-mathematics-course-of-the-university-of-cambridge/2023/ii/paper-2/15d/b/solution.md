<h1 id="15d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Applying the transform twice gives

$$
\operatorname{QFT}_N^2|x\rangle
=\frac1N\sum_{z=0}^{N-1}
 \left(\sum_{y=0}^{N-1}\omega_N^{y(x+z)}\right)|z\rangle.
$$

The [root-of-unity filter](../../../../../../root-of-unity-filter.md) makes the inner sum equal to $N$ exactly when $z\equiv-x\pmod N$ and zero otherwise. Hence

$$
\boxed{\operatorname{QFT}_N^2|x\rangle=|-x\bmod N\rangle}.
$$

Applying modular negation twice gives

$$
\boxed{\operatorname{QFT}_N^4=I}.
$$

**Therefore $\operatorname{QFT}_N^2$ is an involution. Every one of its [eigenvalues](../../../../../../eigenvalue.md) $\lambda$ satisfies $\lambda^2=1$, so its spectrum is contained in $\{1,-1\}$, as summarized by the [square of the quantum Fourier transform](../../../../../../square-of-the-quantum-fourier-transform.md).**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [15D](../../15d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
