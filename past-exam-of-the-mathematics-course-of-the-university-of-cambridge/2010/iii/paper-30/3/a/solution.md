<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Start from the [Erlang loss formula](../../../../../../erlang-loss-formula.md) and reverse the order in its denominator:

$$
\frac1{E(N\nu,NC)}=\sum_{j=0}^{NC}\frac{(NC)!}{(NC-j)!(N\nu)^j}=\sum_{j=0}^{NC}\prod_{\ell=0}^{j-1}\frac{NC-\ell}{N\nu}.
$$

For each fixed $j$, the product tends to $(C/\nu)^j$. If $\nu>C$, it is bounded by this same summable [geometric series](../../../../../../geometric-series.md). Extend the summand by zero for $j>NC$ and apply the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) with [counting measure](../../../../../../counting-measure.md) to obtain

$$
\frac1{E(N\nu,NC)}\longrightarrow\sum_{j=0}^\infty(C/\nu)^j=\frac1{1-C/\nu}.
$$

If $\nu\leq C$, retain the first $K+1$ summands. Their limiting sum is at least $K+1$, so the reciprocal tends to infinity as $K$ can be arbitrarily large. This includes $\nu=C$ without a separate normal approximation. Therefore

$$
\boxed{E(N\nu,NC)\longrightarrow\max\{0,1-C/\nu\}.}
$$

Here $C$ and $N$ are positive integers, as appropriate for circuit counts; taking $\lfloor NC\rfloor$ gives the same limit for a positive real capacity scale. This is the [proportional scaling limit of the Erlang loss formula](../../../../../../proportional-scaling-limit-of-the-erlang-loss-formula.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
