<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $(h_k)$ be a bounded minimizing sequence. A subsequence converges to some $h_*$, and continuity gives $F(h_*)=f$. Since $F$ is smooth and $h_*$ is an unconstrained minimizer,

$$
0=\nabla F(h_*)
=-\mathbb E[Xe^{-h_*\cdot X}\zeta].
$$

Define

$$
\rho=\frac{e^{-h_*\cdot X}\zeta}{F(h_*)}.
$$

Then $\rho>0$, $\mathbb E\rho=1$, and

$$
\mathbb E[\rho X]
=-\frac{\nabla F(h_*)}{F(h_*)}=0.
$$

Thus the normalized exponential tilt is the required [state-price density](../../../../../../state-price-density.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
