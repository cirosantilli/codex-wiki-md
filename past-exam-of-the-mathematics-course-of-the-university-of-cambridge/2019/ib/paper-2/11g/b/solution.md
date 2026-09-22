<h1 id="11g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Proceed by induction on $d=\deg f$. A nonconstant [polynomial](../../../../../../polynomial-split.md) over a [field](../../../../../../field.md) has an irreducible factor $h$. Part (a) gives an extension $k_1/k$ containing a root $\alpha_1$ of $h$, hence of $f$. The factor theorem gives

$$
f(X)=(X-\alpha_1)f_1(X),
\qquad f_1\in k_1[X],
$$

where $f_1$ is monic of degree $d-1$. Apply the induction hypothesis over $k_1$ and compose the resulting field extensions. The final field $F$ contains roots $\alpha_1,\ldots,\alpha_d$ and

$$
\boxed{f(X)=\prod_{i=1}^d(X-\alpha_i)}.
$$

Equivalently, every polynomial has a [splitting field](../../../../../../splitting-field.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [11G](../../11g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
