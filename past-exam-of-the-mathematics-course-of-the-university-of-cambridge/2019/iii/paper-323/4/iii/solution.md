<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $P_+$ be the maximizing projection in the [variational characterization of trace distance](../../../../../../variational-characterization-of-trace-distance.md). Use the binary [POVM](../../../../../../positive-operator-valued-measure.md) $\{P_+,I-P_+\}$ and its [measurement channel](../../../../../../measurement-channel.md). The difference between its two output probability vectors is

$$
(p_1-q_1,p_2-q_2)
=\left(\operatorname{Tr}[P_+(\rho-\sigma)],\operatorname{Tr}[(I-P_+)(\rho-\sigma)]\right)
=(D,-D),
$$

where $D=D(\rho,\sigma)$ and the second equality uses $\operatorname{Tr}(\rho-\sigma)=0$. Since [trace distance](../../../../../../trace-distance.md) between diagonal [density operators](../../../../../../density-matrix.md) is half the [L1 norm](../../../../../../l1-norm.md) of their probability-vector difference,

$$
\boxed{D(\Phi(\rho),\Phi(\sigma))=\frac12(|D|+|-D|)=D(\rho,\sigma)}.
$$

Thus a binary [measurement in quantum mechanics](../../../../../../quantum-measurement-split.md) can preserve the distinguishability of this particular pair exactly. This is the [trace-distance-preserving binary measurement](../../../../../../trace-distance-preserving-binary-measurement.md), which may depend on the two states.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 323](../../../paper-323-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
