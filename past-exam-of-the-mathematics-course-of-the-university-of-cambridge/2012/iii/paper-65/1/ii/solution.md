<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For every [orthogonal projector](../../../../../../orthogonal-projection.md) $P$, positivity gives

$$
\operatorname{Tr}(PX)=\operatorname{Tr}(PQ)-\operatorname{Tr}(PR)
\leq\operatorname{Tr}(PQ)\leq\operatorname{Tr}Q.
$$

These inequalities do not require $P$ to commute with $Q$ or $R$: for example, $\operatorname{Tr}(PR)=\operatorname{Tr}(R^{1/2}PR^{1/2})\geq0$, and apply the same observation to $I-P$ and $Q$.

Let $P_+$ project onto the positive spectral subspace of $X$. Then $P_+Q=Q$ and $P_+R=0$, so $\operatorname{Tr}(P_+X)=\operatorname{Tr}Q=D(\rho,\sigma)$. Hence the [variational characterization of trace distance](../../../../../../variational-characterization-of-trace-distance.md) over projectors is

$$
\boxed{D(\rho,\sigma)=\max_{P=P^\dagger=P^2}\operatorname{Tr}[P(\rho-\sigma)].}
$$

One may include or exclude the zero eigenspace without changing the optimum.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
