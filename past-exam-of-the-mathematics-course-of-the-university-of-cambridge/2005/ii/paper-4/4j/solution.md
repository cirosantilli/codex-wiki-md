<h1 id="4j/solution">Solution</h1>

↑ **Parent:** [4J](../4j.md)

Reliable transmission at rate $r$ means that there is a sequence of binary block codes of lengths $n$, message counts $M_n$ with $\liminf n^{-1}\log_2M_n\ge r$, and decoding error [probabilities](../../../../../probability.md) tending to zero. The [Shannon second coding theorem](../../../../../noisy-channel-coding-theorem.md) identifies the supremum of reliable rates with the [channel capacity](../../../../../channel-capacity.md).

For a [binary symmetric channel](../../../../../binary-symmetric-channel.md), the [conditional entropy](../../../../../conditional-entropy.md) of the output given any input bit is $h_2(p)=-p\log_2p-(1-p)\log_2(1-p)$. The output [entropy](../../../../../entropy.md) is at most one bit and attains one for uniform input, so the maximum [mutual information](../../../../../mutual-information.md) is

$$
\boxed{C=1-h_2(p)}.
$$

All rates strictly below $C$ are achievable, and rates above $C$ are not reliable; this states the supremum without claiming achievability of every boundary rate under every convention.

For very small $p$, the capacity is close to one, with $h_2(p)=p\log_2(1/p)+p/\log 2+O(p^2)$. At $p=1/2$, the output is independent of the input and capacity is zero. For $p>1/2$, flipping every received bit converts the channel to crossover [probability](../../../../../probability.md) $1-p<1/2$; its capacity is unchanged because $h_2(p)=h_2(1-p)$. At $p=1$ the deterministic bit flip is perfectly reversible.

## ↑ Ancestors (10)

1. [4J](../4j.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
