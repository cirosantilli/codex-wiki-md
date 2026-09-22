<h1 id="18h/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $(y,t)$ be feasible for $R$. Since $d_i>0$ and $d^Ty=1$, the vector $y$ is nonzero. Every entry of $A$ is strictly positive and $y\geq0$, so every component of $Ay$ is strictly positive. The relation

$$
Ay=bt
$$

therefore forces $t>0$.

Set $x=y/t$. Then

$$
x\geq0,\qquad Ax=b,\qquad d^Tx=\frac1t>0,
$$

so $x$ is feasible for $Q$, and

$$
\frac{c^Tx}{d^Tx}
=\frac{c^Ty/t}{1/t}
=c^Ty.
$$

Thus every feasible value of $R$ is a feasible value of the [linear-fractional program](../../../../../../../linear-fractional-programming.md) $Q$. Together with part (i), this proves

$$
\boxed{\max R=\max Q}.
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [18H](../../../18h.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ib](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
