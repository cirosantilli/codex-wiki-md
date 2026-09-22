<h1 id="30k/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $D_n=M_n-M_{n-1}$. Given $\mathcal F_{n-1}$, the new information at time $n$ is only the independent symmetric sign $\xi_n$. Thus

$$
D_n=C_n+B_n\xi_n
$$

for some $\mathcal F_{n-1}$-measurable $C_n,B_n$. Taking conditional expectation and using the martingale property gives $C_n=0$. More explicitly, one can take

$$
B_n=\mathbb E[D_n\xi_n\mid\mathcal F_{n-1}]
=\mathbb E[M_n\xi_n\mid\mathcal F_{n-1}],
$$

which is predictable. Therefore

$$
\boxed{M_n=M_0+\sum_{k=1}^nB_k\xi_k.}
$$

This is the [predictable representation in a Rademacher filtration](../../../../../../predictable-representation-in-a-rademacher-filtration.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [30K](../../30k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
