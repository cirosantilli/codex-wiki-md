<h1 id="3i/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $q=\mathbb P(X=B)$. The merged channel is a [Binary Z-channel](../../../../../../../z-channel.md): its second output occurs with probability $q/2$, while the output has one bit of uncertainty only when $X=B$. In terms of the [binary entropy function](../../../../../../../binary-entropy-function.md) $h_2$,

$$
I(X;Y)=h_2(q/2)-q.
$$

At an interior maximum,

$$
0=\frac{dI}{dq}
=\frac12\log_2\frac{1-q/2}{q/2}-1,
$$

so $(2-q)/q=4$ and $q=2/5$. Consequently

$$
\boxed{C=h_2(1/5)-\frac25
=\log_2\frac54\text{ bits}}.
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3I](../../../3i.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
