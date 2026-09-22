<h1 id="4g/solution">Solution</h1>

↑ **Parent:** [4G](../4g.md)

[Shannon second coding theorem](../../../../../noisy-channel-coding-theorem.md) identifies the [channel capacity](../../../../../channel-capacity.md) of a discrete memoryless channel as $C=\max_{P_X}I(X;Y)$: rates below $C$ admit block codes with error probability tending to zero, whereas a rate above $C$ cannot achieve vanishing error. Entropies here are measured in bits. For a [binary erasure channel](../../../../../binary-erasure-channel.md), a non-erased output determines its input exactly, while an erasure, independent of the input, leaves the original uncertainty unchanged. If $\mathbb P(X=1)=q$, then

$$
H(X)=h_2(q),\qquad H(X\mid Y)=p h_2(q),\qquad
I(X;Y)=(1-p)h_2(q).
$$

The [binary entropy function](../../../../../binary-entropy-function.md) has maximum one at $q=1/2$. Therefore

$$
\boxed{C=1-p\ \text{bits per channel use}}.
$$

This includes the noiseless case $p=0$ and the wholly erased case $p=1$.

## ↑ Ancestors (10)

1. [4G](../4g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
