<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For finite $p>n$, choose

$$
q=\frac{2p}{p-2},\qquad \frac12=\frac1p+\frac1q.
$$

Since $n\geq3$ and $p>n$, we have $2<q<2^*=2n/(n-2)$. The zero-boundary versions of the [Sobolev embedding theorem](../../../../../../sobolev-embedding-theorem.md) and [Rellich-Kondrachov compactness theorem](../../../../../../rellich-kondrachov-theorem.md) say that $W_0^{1,2}(\Omega)$ embeds continuously into $L^{2^*}$ and compactly into $L^q$ for $q<2^*$ on a bounded open set. These versions hold on arbitrary bounded open sets by zero extension; a boundary extension operator is not needed.

If $(v_j)$ is bounded in $L^2$, then $(Tv_j)$ is bounded in $W_0^{1,2}$ by the preceding part. A subsequence consequently converges in $L^q$ to some $z$. [Hölder's inequality](../../../../../../holder-s-inequality.md) gives

$$
\|w(Tv_j-z)\|_2\leq\|w\|_p\|Tv_j-z\|_q\longrightarrow0.
$$

Multiplication by $w$ is bounded from $L^q$ to $L^2$, and the same estimate proves that $K$ is bounded and well defined. Every bounded input sequence has a subsequence whose images converge in $L^2$, so $\boxed{K\text{ is compact}}$. If $p=\infty$ is included, take $q=2$ and use the same argument. This is the [compact L2 potential perturbation of the Dirichlet Laplacian](../../../../../../compact-l2-potential-perturbation-of-the-dirichlet-laplacian.md) mechanism.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
