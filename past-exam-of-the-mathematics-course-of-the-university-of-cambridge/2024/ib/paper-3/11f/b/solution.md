<h1 id="11f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The inequalities imply

$$
B_{d_1}(x,r/\beta)\subseteq B_{d_2}(x,r)
\quad\text{and}\quad
B_{d_2}(x,\alpha r)\subseteq B_{d_1}(x,r).
$$

Thus the two metrics induce the same [open sets](../../../../../../open-set.md) and are equivalent.

The converse fails. On $\mathbb R$, let

$$
d_1(x,y)=|x-y|,
\qquad
d_2(x,y)=|\arctan x-\arctan y|.
$$

The metrics are equivalent because $\arctan:\mathbb R\to(-\pi/2,\pi/2)$ is a homeomorphism, but

$$
\frac{d_2(0,n)}{d_1(0,n)}\longrightarrow0,
$$

so no positive lower comparison constant exists. This is an [equivalent metrics need not be bi-Lipschitz equivalent](../../../../../../equivalent-metrics-need-not-be-bi-lipschitz-equivalent.md) example.

Equivalent metrics on the codomain also need not give the same [uniform convergence](../../../../../../uniform-convergence.md). Take $X=\mathbb N$, $Y=\mathbb R$, and use the two metrics above. Define

$$
f(k)=k,
\qquad
f_n(k)=\begin{cases}2n,&k=n,\\k,&k\ne n.
\end{cases}
$$

Then

$$
\sup_kd_2(f_n(k),f(k))
=\arctan(2n)-\arctan n\longrightarrow0,
$$

so $f_n\to f$ uniformly for $d_2$, whereas

$$
\sup_kd_1(f_n(k),f(k))=n,
$$

so convergence is not uniform for $d_1$. This is the [equivalent codomain metrics need not preserve uniform convergence](../../../../../../equivalent-codomain-metrics-need-not-preserve-uniform-convergence.md) phenomenon.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [11F](../../11f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
