<h1 id="3g/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [reliable transmission rate](../../../../../../reliable-transmission-rate.md) $R$ means that length-$n$ codes can carry $M_n$ messages with $n^{-1}\log_2M_n$ tending to at least $R$ while the [probability measure](../../../../../../probability-measure.md) of the decoding-error event tends to zero. By the [Shannon second coding theorem](../../../../../../noisy-channel-coding-theorem.md), the supremum of reliable rates is the [binary symmetric channel capacity](../../../../../../binary-symmetric-channel-capacity.md)

$$
C(p)=1-h_2(p),
\qquad
h_2(p)=-p\log_2p-(1-p)\log_2(1-p).
$$

For small positive $p$, the [binary entropy function](../../../../../../binary-entropy-function.md) has the [asymptotic expansion](../../../../../../asymptotic-expansion.md)

$$
h_2(p)=p\log_2\frac1p+\frac{p}{\ln2}+O(p^2),
$$

so $C(p)$ starts at one bit per channel use and decreases rapidly from one as errors are introduced.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3G](../../3g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
