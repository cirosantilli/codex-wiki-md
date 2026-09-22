<h1 id="11g/solution">Solution</h1>

↑ **Parent:** [11G](../11g.md)

For a [discrete memoryless channel](../../../../../discrete-memoryless-channel.md), its [channel capacity](../../../../../channel-capacity.md) in bits per use is $C=\max_{P_X}I(X;Y)$. The [Shannon second coding theorem](../../../../../noisy-channel-coding-theorem.md) identifies this with the supremum of rates achievable by arbitrarily long block codes with error [probability](../../../../../probability.md) tending to zero: every rate below $C$ is achievable, and no rate above $C$ can have vanishing error. The channel is used independently at each transmission, and coding rate is measured using base-two logarithms.

Let $q$ be the [probability](../../../../../probability.md) of using the second input symbol. The second output symbol occurs with [probability](../../../../../probability.md) $q/2$, so $H(Y)=h_2(q/2)$. The first input has deterministic output and the second has one bit of conditional output [Shannon entropy](../../../../../information-entropy.md); hence $H(Y\mid X)=q$ and

$$
I(X;Y)=h_2(q/2)-q.
$$

For $0<q<1$, its derivative is $\frac12\log_2[(2-q)/q]-1$, which vanishes at $q=2/5$. [Strict concavity](../../../../../strict-concavity.md) of [binary entropy](../../../../../binary-entropy.md) makes this the unique global maximum. Substituting gives

$$
\boxed{C=h_2(1/5)-2/5=\log_2 5-2.}
$$

Thus Shannon's theorem supplies operational coding rates arbitrarily close to this value from below, and rules out reliable transmission above it.

## ↑ Ancestors (10)

1. [11G](../11g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
