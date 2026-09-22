<h1 id="18h/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The chain is a [birth-death chain](../../../../../../../birth-death-chain.md). Detailed balance between $0$ and $1$ gives

$$
\pi_0p=\pi_1q^{-1},
\qquad\text{so}\qquad
\pi_1=qp\,\pi_0.
$$

For $i\geq1$, detailed balance between $i$ and $i+1$ gives

$$
\pi_iq^{-(i+2)}=\pi_{i+1}q^{-(i+1)},
\qquad
\pi_{i+1}=\frac{\pi_i}{q}.
$$

Consequently

$$
\pi_i=qp\,\pi_0q^{-(i-1)},\qquad i\geq1.
$$

The expected occupation time of the positive even states during a return cycle to state $1$ is therefore

$$
\frac{\pi_2+\pi_4+\cdots}{\pi_1}
=\sum_{r=1}^{\infty}q^{-(2r-1)}
=\boxed{\frac{q}{q^2-1}}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [18H](../../../18h.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ib](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
