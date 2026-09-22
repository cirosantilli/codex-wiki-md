<h1 id="4/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For independent attempts, measuring after each application of $A$ produces a success with probability $p$. Recognize the answer with the verifier and restart on failure. The number $T$ of attempts has a [geometric distribution](../../../../../../geometric-distribution.md), with $\Pr(T=k)=(1-p)^{k-1}p$. Summing the tail probabilities gives

$$
\boxed{\mathbb E T=\sum_{k=0}^\infty(1-p)^k=\frac1p.}
$$

This counts applications of $A$; it presumes $p>0$ and a fresh preparation for each attempt. If $p=0$, neither repetition nor the amplification construction can create a good component from this input.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [4](../../4.md)
3. [Paper 53](../../../paper-53-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
