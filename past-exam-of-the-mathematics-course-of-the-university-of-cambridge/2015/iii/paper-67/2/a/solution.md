<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Define the orthonormal history basis

$$
|e_t\rangle=|\psi_t\rangle\otimes|c_t\rangle,\qquad
|c_t\rangle=|1\rangle^{\otimes t}|0\rangle^{\otimes(T-t)},
\quad t=0,\ldots,T,
$$

where $\psi_t=U_t\cdots U_1\psi_0$. Orthogonality follows from the distinct [unary quantum clock](../../../../../../unary-quantum-clock.md) strings, regardless of overlaps between the computational states.

The initialization term acts diagonally:

$$
H_{\rm init}|e_0\rangle=0,\qquad
H_{\rm init}|e_t\rangle=|e_t\rangle\quad(t\geq1).
$$

Each propagation term only couples the two clock strings adjacent to its step. The gate and its adjoint give

$$
H_t|e_{t-1}\rangle=\frac12(|e_{t-1}\rangle-|e_t\rangle),\qquad
H_t|e_t\rangle=\frac12(|e_t\rangle-|e_{t-1}\rangle),
$$

and $H_t|e_j\rangle=0$ for $j\notin\{t-1,t\}$. The same calculation covers the two endpoint terms.

Thus **both Hamiltonians preserve $\mathcal L$**, and in the history basis their restrictions are

$$
\boxed{D:=H_{\rm init}|_{\mathcal L}=I-|e_0\rangle\langle e_0|,
\qquad
E:=H_{\rm final}|_{\mathcal L}
=\frac12\sum_{t=1}^T
(|e_t\rangle-|e_{t-1}\rangle)
(\langle e_t|-\langle e_{t-1}|).}
$$

This [history-subspace propagation Hamiltonian](../../../../../../history-subspace-propagation-hamiltonian.md) is a path [Graph Laplacian](../../../../../../laplacian-matrix.md) with a factor $1/2$. The specified two-clock endpoint formulas assume $T\geq2$; a shorter circuit can first be padded with identity gates.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
