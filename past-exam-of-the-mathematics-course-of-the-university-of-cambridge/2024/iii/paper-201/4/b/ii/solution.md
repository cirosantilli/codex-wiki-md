<h1 id="4/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $\sigma_x=\inf\{t\geq0:\widetilde B_t=x\}$. Continuity gives $\{S\geq x\}=\{\sigma_x<\infty\}$. On this event, the [Strong Markov property](../../../../../../../strong-markov-property.md) says that

$$
(\widetilde B_{\sigma_x+t}-x)_{t\geq0}
$$

is an independent Brownian motion with drift $-\mu$. It reaches level $y$ with probability $\mathbb P(S\geq y)$. Therefore

$$
\boxed{\mathbb P(S\geq x+y)
=\mathbb P(\sigma_x<\infty)\mathbb P(S\geq y)
=\mathbb P(S\geq x)\mathbb P(S\geq y).}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 201](../../../../paper-201-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
