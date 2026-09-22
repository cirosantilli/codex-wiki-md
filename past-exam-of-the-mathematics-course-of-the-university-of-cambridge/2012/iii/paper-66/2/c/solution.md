<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The root $\omega$ must be a **primitive $n$th root of unity**, for example $e^{2\pi i/n}$. The printed statement merely says $n$th root; that is insufficient. With $n=2$ and $\omega=1$, the states with $r=0$ and $r=1$ coincide. More generally, a root of order $d<n$ repeats the $r$ labels modulo $d$. For $n=1$ the construction is trivial.

For a [primitive root of unity](../../../../../../primitive-root-of-unity.md), the [generalized Bell basis](../../../../../../generalized-bell-basis.md) obeys

$$
\langle\psi_{rs}|\psi_{r's'}\rangle
=\delta_{ss'}\frac1n\sum_{j=0}^{n-1}\omega^{j(r'-r)}
=\delta_{ss'}\delta_{rr'}.
$$

The last equality follows from the finite [geometric series](../../../../../../geometric-series.md): a nonzero exponent difference modulo $n$ has sum zero, while zero difference has sum $n$. There are $n^2$ orthonormal vectors in an $n^2$-dimensional [Hilbert space](../../../../../../hilbert-space-split.md), so they form a complete basis.

For [qudit teleportation](../../../../../../qudit-teleportation.md), Alice's input is $|\chi\rangle_U=\sum_jc_j|j\rangle$. Alice and Bob share $|\psi_{00}\rangle_{aB}=n^{-1/2}\sum_k|k k\rangle$. Define the [qudit shift and phase operators](../../../../../../qudit-shift-and-phase-operators.md) by $X|j\rangle=|j+1\rangle$ and $Z|j\rangle=\omega^j|j\rangle$. Alice measures $Ua$ in the [generalized Bell basis](../../../../../../generalized-bell-basis.md). On outcome $(r,s)$, Bob's unnormalized state is

$$
\frac1n\sum_jc_j\omega^{-rj}|j+s\rangle_B
=\frac1nX^sZ^{-r}|\chi\rangle_B.
$$

All outcomes have probability $1/n^2$. Alice communicates $(r,s)$ and Bob applies

$$
\boxed{Z^rX^{-s},}
$$

which restores $|\chi\rangle$ exactly. The protocol consumes one maximally entangled pair of $n$-level systems, a local $n^2$-outcome measurement, and a classical message with $n^2$ possibilities. For a fixed-length binary encoding, $\lceil\log_2 n^2\rceil$ bits suffice. No measurement depends on the unknown amplitudes.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
