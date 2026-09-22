<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The transpose map $T(X)=X^T$ in a fixed basis is linear, trace preserving and positive: if $X\geq0$, then for every $v$, $v^\dagger X^Tv=\overline{\bar v^\dagger X\bar v}\geq0$. It is nevertheless not a [completely positive map](../../../../../../completely-positive-map.md). Apply $\operatorname{id}\otimes T$ to the two-qubit [Bell state](../../../../../../bell-state-split.md) $|\Phi^+\rangle=(|00\rangle+|11\rangle)/\sqrt2$. The resulting operator is

$$
\frac12\begin{pmatrix}1&0&0&0\\0&0&1&0\\0&1&0&0\\0&0&0&1\end{pmatrix},
$$

with eigenvalues $1/2,1/2,1/2,-1/2$. The negative eigenvector is $(|01\rangle-|10\rangle)/\sqrt2$. Thus a positive input on system plus reference acquires a negative expectation value. **Transposition is positive but not completely positive**, so it cannot be a deterministic local quantum process on arbitrary entangled states.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
