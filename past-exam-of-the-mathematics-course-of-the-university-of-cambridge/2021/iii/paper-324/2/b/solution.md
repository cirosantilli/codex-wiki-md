<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Expand $|b\rangle=\sum_i b_i|\lambda_i\rangle$ in the nondegenerate eigenbasis of $A$. Apply [quantum phase estimation](../../../../../../quantum-phase-estimation.md) to $U_+=e^{2\pi iA}$, using $U_-$ when inverse powers are needed, to coherently attach the eigenvalue:

$$
\sum_i b_i|\lambda_i\rangle|\lambda_i\rangle_{\rm val}.
$$

On an ancillary qubit perform the eigenvalue-controlled rotation

$$
|0\rangle\longmapsto
\sqrt{1-e^{2(\lambda_i-1)}}|0\rangle
+e^{\lambda_i-1}|1\rangle.
$$

Uncompute the value register and measure the ancilla. Conditional on outcome one, the system is proportional to

$$
\sum_i b_ie^{\lambda_i}|\lambda_i\rangle=e^A|b\rangle,
$$

and normalization gives the desired $|\psi\rangle$.

The success probability is

$$
\boxed{P_S=e^{-2}\langle b|e^{2A}|b\rangle}.
$$

Since every $\lambda_i>0$,

$$
\boxed{P_S>e^{-2}},
$$

a positive lower bound independent of $|b\rangle$. The promised precision assumptions permit the eigenvalue-controlled arithmetic and rotation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
