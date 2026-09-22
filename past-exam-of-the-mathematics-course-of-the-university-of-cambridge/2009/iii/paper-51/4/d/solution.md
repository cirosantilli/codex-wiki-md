<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Independent applications of the [phase-flip channel](../../../../../../phase-flip-channel.md) are a classical mixture of the eight physical [Pauli Z gate](../../../../../../pauli-z-gate.md) error patterns. A specified weight-$k$ pattern has [probability](../../../../../../probability.md) $\epsilon^k(1-\epsilon)^{3-k}$. The recovery from the preceding part succeeds on weight zero and one, and yields the logical [Pauli X gate](../../../../../../pauli-x-gate.md) on weight two and three. There are three weight-two patterns and one weight-three pattern, so the logical failure probability is

$$
p_L=3\epsilon^2(1-\epsilon)+\epsilon^3=3\epsilon^2-2\epsilon^3.
$$

Averaging the corrected branches gives the complete decoded [quantum channel](../../../../../../quantum-channel.md)

$$
\boxed{\rho'=(1-3\epsilon^2+2\epsilon^3)\rho+(3\epsilon^2-2\epsilon^3)X\rho X.}
$$

In particular, the leading logical error is $3\epsilon^2$, rather than an error of first order in $\epsilon$. For the stated range,

$$
\epsilon-p_L=\epsilon(1-\epsilon)(1-2\epsilon)>0.
$$

Thus the failure probability is smaller than the physical error probability. The decoded channel is a bit-flip channel; it is not $D_{p_L}$, whose error operator would be $Z$. This distinction follows from the logical codeword exchange in the [phase-flip repetition code](../../../../../../phase-flip-repetition-code.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 51](../../../paper-51-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
