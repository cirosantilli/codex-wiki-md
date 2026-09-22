<h1 id="19c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Inductively, $p_n$ is monic of degree $n$, because the leading term of $p_{n+1}$ comes only from $xp_n$. Assume $p_0,\ldots,p_n$ are mutually orthogonal. The definitions give

$$
\langle p_{n+1},p_n\rangle
=\langle xp_n,p_n\rangle-\alpha_n\langle p_n,p_n\rangle=0.
$$

Using the preceding recurrence in the form

$$
xp_{n-1}=p_n+\alpha_{n-1}p_{n-1}+\beta_{n-1}p_{n-2}
$$

gives

$$
\langle xp_n,p_{n-1}\rangle
=\langle p_n,xp_{n-1}\rangle
=\langle p_n,p_n\rangle,
$$

so $\langle p_{n+1},p_{n-1}\rangle=0$ by the definition of $\beta_n$. If $j\leq n-2$, then $xp_j$ lies in the span of $p_{j-1},p_j,p_{j+1}$, all orthogonal to $p_n$, and the remaining recurrence terms are also orthogonal to $p_j$. Hence $\langle p_{n+1},p_j\rangle=0$. Induction proves that the recurrence defines monic [orthogonal polynomials](../../../../../../orthogonal-polynomial.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [19C](../../19c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
