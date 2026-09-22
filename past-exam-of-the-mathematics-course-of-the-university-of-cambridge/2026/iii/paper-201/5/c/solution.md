<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Apply part (b) to $u_n$. Its zero [boundary value](../../../../../../dirichlet-boundary-condition.md) gives

$$
u_n(x)=-\frac12\mathbb E_x\int_0^T\Delta u_n(B_s)\,ds.
$$

The assumptions say that $\Delta u_n(y)\to0$ for every $y\in D$ and that $|\Delta u_n|\leq C$ uniformly. Thus the integrand converges pointwise to zero and is dominated by $CT$, whose expectation is finite by part (a). The [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) gives $u_n(x)\to0$ for every $x\in D$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
