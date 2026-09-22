<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Use the [Schmidt decomposition](../../../../../../schmidt-decomposition.md) of the bipartite [pure state](../../../../../../pure-state.md):

$$
|\psi\rangle_{QR}=\sum_{j=1}^r\sqrt{p_j}\,|u_j\rangle_Q|v_j\rangle_R,\qquad p_j>0,\quad\sum_jp_j=1.
$$

The two [reduced density matrices](../../../../../../reduced-density-matrix.md), obtained by [partial trace](../../../../../../partial-trace.md), are

$$
\rho_Q=\sum_jp_j|u_j\rangle\langle u_j|,\qquad\rho_R=\sum_jp_j|v_j\rangle\langle v_j|.
$$

Their nonzero [eigenvalues](../../../../../../eigenvalue.md) are identical, even if the two ambient dimensions differ. Zero [eigenvalues](../../../../../../eigenvalue.md) contribute no [Von Neumann entropy](../../../../../../von-neumann-entropy-split.md), so

$$
\boxed{H(Q)_\psi=H(R)_\psi=-\sum_jp_j\log_2p_j.}
$$

This common [Von Neumann entropy](../../../../../../von-neumann-entropy-split.md) is the [entanglement entropy](../../../../../../entanglement-entropy.md) of the bipartite [pure state](../../../../../../pure-state.md).

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
