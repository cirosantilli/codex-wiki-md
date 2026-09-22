<h1 id="5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Choose an [orthonormal basis](../../../../../../orthonormal-basis.md) of the joint $d^2$-dimensional [Hilbert space](../../../../../../hilbert-space-split.md) whose first vector is the given [purification of a density operator](../../../../../../purification-of-a-density-operator.md) $|\rho\rangle_{QR}$. Apply [rank-one dephasing](../../../../../../rank-one-dephasing.md) to $\sigma_{QR}$ in this basis, and denote the resulting diagonal probabilities by $p_1,\ldots,p_{d^2}$. Their first entry is

$$
p_1=\langle\rho|\sigma_{QR}|\rho\rangle=f^2.
$$

The preceding [entropy increase under nonselective projective measurement](../../../../../../entropy-increase-under-nonselective-projective-measurement.md) and [entropy bound with one prescribed probability](../../../../../../entropy-bound-with-one-prescribed-probability.md) yield

$$
S(\sigma_{QR})\leq H(p)\leq h(f^2)+(1-f^2)\log_2(d^2-1).
$$

Therefore the [quantum Fano inequality](../../../../../../quantum-fano-inequality.md) is

$$
\boxed{S(\sigma_{QR})\leq h(f^2)+(1-f^2)\log_2(d^2-1).}
$$

The quantity $f^2$ is the [entanglement fidelity](../../../../../../entanglement-fidelity.md) of $\mathcal N$ on $\rho_Q$; it is already a squared overlap, so it is $f^2$, rather than $f$, that enters the [binary entropy](../../../../../../binary-entropy.md). The argument is an instance of the [entropy bound from overlap with a pure state](../../../../../../entropy-bound-from-overlap-with-a-pure-state.md) in dimension $d^2$. At $f^2=1$ the output is the original [pure state](../../../../../../pure-state.md) and its [Von Neumann entropy](../../../../../../von-neumann-entropy-split.md) is zero. For $d=1$ the system is trivial and the same zero-entropy conclusion holds without evaluating $\log_2(d^2-1)$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
