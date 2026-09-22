<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $B$ be the selected block, and write $\alpha=\mathbb P(B=1)$. Because both the input and output [alphabets](../../../../../alphabet.md) are disjoint across blocks, $B$ is determined by either the input or the output. The mutual-information chain rule therefore gives

$$
I(X;Y)=H(B)+I(X;Y\mid B)\leq h_2(\alpha)+\alpha C_1+(1-\alpha)C_2.
$$

For any fixed $\alpha$, [equality](../../../../../equality-mathematics.md) is achievable by using a capacity-achieving distribution inside each block. It remains to maximize this binary expression.

Put $S=2^{C_1}+2^{C_2}$ and $r=2^{C_1}/S$. A direct expansion of [binary relative entropy](../../../../../binary-relative-entropy.md) yields

$$
h_2(\alpha)+\alpha C_1+(1-\alpha)C_2
=\log_2S-d\bigl((\alpha,1-\alpha),(r,1-r)\bigr).
$$

Part 1(a) makes the [maximum](../../../../../maximum-of-a-subset-of-a-total-order.md) $\log_2S$, uniquely at $\alpha=r$. Hence

$$
\boxed{C=\log_2(2^{C_1}+2^{C_2}),\qquad\mathbb P(B=i)=\frac{2^{C_i}}{2^{C_1}+2^{C_2}}.}
$$

The block choice itself communicates information, in addition to any information sent within the selected block.

This is [capacity of a disjoint sum of channels](../../../../../capacity-of-a-disjoint-sum-of-channels.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the communication Theory course of the University of Oxford](../../../../split.md)
6. [Communication Theory course of the University of Oxford](../../../../../communication-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
