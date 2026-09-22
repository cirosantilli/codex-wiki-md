<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

There is a normalization error in the original PDF: the first term contains $I$ rather than $\rho$. For a normalized [qubit](../../../../../../qubit.md) [density operator](../../../../../../density-matrix.md), that printed expression has [trace](../../../../../../matrix-trace.md) $2(1-p)+p=2-p$, so it is not a [quantum channel](../../../../../../quantum-channel.md) except at $p=1$. The intended [depolarizing channel](../../../../../../quantum-depolarizing-channel.md) is the [Pauli channel](../../../../../../pauli-channel.md) that leaves the input unchanged with [probability](../../../../../../probability.md) $1-p$ and applies each nonidentity [Pauli matrix](../../../../../../pauli-matrices.md) with [probability](../../../../../../probability.md) $p/3$, for $0\leq p\leq1$. Its [Kraus operators](../../../../../../kraus-operator.md) are

$$
K_0=\sqrt{1-p}\,I,\qquad K_k=\sqrt{p/3}\,\sigma_k\quad(k=1,2,3),
$$

and $\sum_{k=0}^3K_k^\dagger K_k=I$, proving that it is trace-preserving and a [completely positive map](../../../../../../completely-positive-map.md).

Write the input in its [Bloch vector](../../../../../../bloch-vector.md) representation,

$$
\rho=\frac12(I+\mathbf r\cdot\boldsymbol\sigma),\qquad |\mathbf r|\leq1.
$$

Conjugation by a [Pauli matrix](../../../../../../pauli-matrices.md) keeps its own [Bloch vector](../../../../../../bloch-vector.md) component and reverses the other two. More explicitly, $\sigma_k\sigma_j\sigma_k=\sigma_j$ for $j=k$ and $-\sigma_j$ for $j\ne k$. Hence

$$
\sum_{k=1}^3\sigma_k\rho\sigma_k
=\frac12(3I-\mathbf r\cdot\boldsymbol\sigma)
=2I-\rho.
$$

The corrected [quantum channel](../../../../../../quantum-channel.md) therefore gives

$$
\Phi_p(\rho)=(1-p)\rho+\frac p3(2I-\rho)
=\frac12\left[I+\left(1-\frac{4p}{3}\right)\mathbf r\cdot\boldsymbol\sigma\right].
$$

Thus its action is

$$
\boxed{\mathbf r\longmapsto\left(1-\frac{4p}{3}\right)\mathbf r.}
$$

The [Bloch sphere](../../../../../../bloch-sphere.md) is sent to a sphere of radius $|1-4p/3|$ about the origin of the [Bloch ball](../../../../../../bloch-ball.md). At $p=0$ the action is the identity. For $0<p<3/4$ the [Bloch vector](../../../../../../bloch-vector.md) shrinks without changing direction. At $p=3/4$ every input becomes the maximally mixed [density operator](../../../../../../density-matrix.md) $I/2$. For $3/4<p\leq1$, the [Bloch vector](../../../../../../bloch-vector.md) reverses direction and shrinks, reaching factor $-1/3$ at $p=1$. The reversal is compatible with complete positivity because this remains a probabilistic mixture of [Pauli matrices](../../../../../../pauli-matrices.md). The parameter here is the total nonidentity-error [probability](../../../../../../probability.md), not the retention parameter used in some definitions of the [quantum depolarizing channel](../../../../../../quantum-depolarizing-channel.md).

For completeness, retain the PDF literally and call its output $F_p(\rho)$. The same calculation gives

$$
F_p(\rho)=\left(1-\frac p2\right)I-\frac p6\mathbf r\cdot\boldsymbol\sigma,
\qquad\operatorname{Tr}F_p(\rho)=2-p.
$$

This has no normalized-output [Bloch ball](../../../../../../bloch-ball.md) interpretation as printed. If it is manually normalized, then

$$
\frac{F_p(\rho)}{2-p}
=\frac12\left[I-\frac{p}{3(2-p)}\mathbf r\cdot\boldsymbol\sigma\right].
$$

That different transformation sends $p=0$ to $I/2$, rather than to the input, and agrees with the intended answer only at $p=1$. The literal and corrected conventions therefore cannot be silently identified.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
