<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Define $E|0\rangle=|D_k^N\rangle$ and $E|1\rangle=|D_{k+1}^N\rangle$. From the branch calculation in part (b), outcome $R_0=0,R_1=1$ leaves

$$
\alpha|D_{k+1}^N\rangle+\beta|D_k^N\rangle=E(\beta|0\rangle+\alpha|1\rangle)=EX|\psi\rangle.
$$

Thus **the effective input teleported was $X|\psi\rangle=\beta|0\rangle+\alpha|1\rangle$**. A [Pauli X gate](../../../../../../pauli-x-gate.md) flips every bit and hence maps a [Dicke state](../../../../../../dicke-state.md) with $j$ excitations to one with $N-j$ excitations. Since $N-k=k+1$, applying $X$ at every receiving party interchanges the two logical [basis](../../../../../../basis.md) states and restores $E|\psi\rangle$. Therefore

$$
\boxed{\text{Bob and each other recipient should apply }X.}
$$

In particular Bob's uncorrected [reduced density matrix](../../../../../../reduced-density-matrix.md) is $X\rho X$, and his correction returns it to the [matrix](../../../../../../matrix.md) in part (c). The remaining branches can likewise be corrected: $Z^{\otimes N}$ implements logical $Z$ up to the common [global phase](../../../../../../global-phase.md) $(-1)^k$, while $X^{\otimes N}$ implements logical $X$. Thus the outcome dependence can be removed by local [Pauli gates](../../../../../../pauli-gate.md) even though the resulting copies remain imperfect.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
