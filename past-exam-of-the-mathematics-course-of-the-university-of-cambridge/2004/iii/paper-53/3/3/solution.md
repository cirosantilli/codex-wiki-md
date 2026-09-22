<h1 id="3/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Assume the three physical [phase-flip channels](../../../../../../phase-flip-channel.md) act independently, with the same probability $p$ on each qubit, and encoding, recovery and decoding are ideal. Zero or one physical error is corrected. Hence

$$
\boxed{P_{\mathrm{rec}}=(1-p)^3+3p(1-p)^2=1-3p^2+2p^3.}
$$

The probability of an uncorrectable two- or three-site error is $p_L=3p^2(1-p)+p^3=3p^2-2p^3$.

One must also choose the logical convention consistently with the output phase error specified here. The usual [phase-flip repetition code](../../../../../../phase-flip-repetition-code.md) with codewords $|+++\rangle$ and $|---\rangle$ has residual operator $Z_1Z_2Z_3$ after two or three physical errors: their [error syndrome](../../../../../../error-syndrome.md) equals that of the complementary zero- or one-error pattern. This operator exchanges those codewords, so plain inverse encoding would give logical $X$, not $Z$.

To obtain the stated logical phase-flip convention, use the [logical Hadamard convention for a phase-flip repetition code](../../../../../../logical-hadamard-convention-for-a-phase-flip-repetition-code.md). Put a logical [Hadamard gate](../../../../../../hadamard-gate.md) before that encoding and after its decoding. The encoded state is

$$
\frac{\alpha+\beta}{\sqrt2}|+++\rangle+\frac{\alpha-\beta}{\sqrt2}|---\rangle,
$$

where the plus and minus states in these codewords are the real [Hadamard basis](../../../../../../hadamard-basis.md) states. The uncorrectable exchange is now conjugated to $HXH=Z$. With that convention the decoded [density operator](../../../../../../density-matrix.md) and its [trace distance](../../../../../../trace-distance.md) are exactly

$$
\boxed{\rho_{\mathrm{dec}}=(1-p_L)\rho+p_LZ\rho Z,\qquad d(\rho,\rho_{\mathrm{dec}})=2(3p^2-2p^3)|\alpha\beta|.}
$$

For $0<p<1/2$, $p-p_L=p(1-p)(1-2p)>0$, so coding reduces the [trace distance](../../../../../../trace-distance.md). The displayed recovery probability means success of correction as a quantum operation on an arbitrary unknown input. If the particular input is a $Z$ eigenstate, even the logical phase-error branch represents the same physical state, and the probability of recovering that particular state is one.

Independence is an extra noise assumption needed for the numerical probability. If all three physical qubits flip together with probability $p$, each marginal still has the given [phase-flip channel](../../../../../../phase-flip-channel.md), but the logical failure probability is $p$, not $3p^2-2p^3$. More generally, for a classical joint phase-error distribution with a random number $K$ of flips, $P_{\mathrm{rec}}=\Pr(K\leq1)$ and $p_L=\Pr(K\geq2)$; the same decoded mixture holds in the stated logical convention. Thus marginal error probabilities alone do not determine the requested recovery probability. A complex environment overlap likewise requires the coherent rotation to be retained or separately compensated before this stochastic phase-error analysis applies.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [3](../../3.md)
3. [Paper 53](../../../paper-53-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
