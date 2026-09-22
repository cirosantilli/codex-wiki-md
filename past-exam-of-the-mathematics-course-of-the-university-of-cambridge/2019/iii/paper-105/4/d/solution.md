<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Fix $W\Subset V\Subset U$. The standard local regularization of the maximal [graph norm](../../../../../../graph-norm.md) domain supplies smooth compactly supported approximants $u_k$ on $V$ such that

$$
u_k\longrightarrow u\quad\text{in }H^1(V),
\qquad
Lu_k\longrightarrow Lu\quad\text{in }L^2(V).
$$

Apply part 4(c), with $V$ as the outer domain, to $u_k-u_m$. It gives

$$
\|D^2(u_k-u_m)\|_{L^2(W)}
\leq C\left(\|L(u_k-u_m)\|_{L^2(V)}
+\|u_k-u_m\|_{H^1(V)}\right)\longrightarrow0.
$$

Thus $(u_k)$ is Cauchy in $H^2(W)$. Its $H^1$ limit is $u$, so $u\in H^2(W)$. Since $W\Subset U$ was arbitrary, the definition of a [Local Sobolev space](../../../../../../local-sobolev-space.md) gives

$$
\boxed{u\in H^2_{\mathrm{loc}}(U).}
$$

This is the [Interior H2 regularity for continuous nondivergence coefficients](../../../../../../interior-h2-regularity-for-continuous-nondivergence-coefficients.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
