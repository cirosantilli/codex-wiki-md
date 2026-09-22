<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a finite symmetric generating alphabet $\Sigma$, the [growth function of a finitely generated group](../../../../../../growth-function-of-a-finitely-generated-group.md) is

$$
\boxed{\beta_{G,\Sigma}(n)=|B_\Sigma(1,n)|=\#\{g\in G:|g|_\Sigma\le n\}}.
$$

It counts distinct elements, not words. Relations affect which words coincide, while the resulting coarse growth type is independent of the finite generating set.

Let $f:G\to H$ be a [quasi-isometry](../../../../../../quasi-isometry.md) between the vertex [word metrics](../../../../../../word-metric.md), with constants $\lambda,\epsilon$. A [quasi-isometry](../../../../../../quasi-isometry.md) of the metric graphs can be rounded to vertices with only bounded changes of these constants. If $f(g)=f(g')$, its lower distortion bound gives $d_G(g,g')\le\lambda\epsilon$. Thus every nonempty fibre has at most $M=\beta_G(\lceil\lambda\epsilon\rceil)$ elements, independently of its centre. Also $f(B_G(1,n))$ lies in the ball of radius $\lambda n+\epsilon$ about $f(1)$. Left translation in $H$ preserves ball cardinalities, so

$$
\beta_G(n)\le M\beta_H(\lceil\lambda n+\epsilon\rceil).
$$

Apply the same argument to a [quasi-inverse of a quasi-isometry](../../../../../../quasi-inverse-of-a-quasi-isometry.md) to get the reverse comparison. Enlarging all constants to an integer $K$ gives the two inequalities required by the paper's $\lesssim$ relation, and therefore **$\beta_G\sim_e\beta_H$**. This proves [quasi-isometry](../../../../../../quasi-isometry.md) invariance of the stated growth class.

For the exponential upper bound, put $q=|\Sigma|$. Every element in the radius-$n$ ball has a representative of length at most $n$. Hence

$$
\beta_G(n)\le\sum_{j=0}^nq^j\le(q+1)^n\qquad(n\ge0),
$$

where the last inequality follows by comparison with the binomial expansion of $(q+1)^n$; it also holds for the empty alphabet of the trivial group. Thus **every [finitely generated group](../../../../../../finitely-generated-group.md) has at most exponential growth**, with no finite-relator assumption needed.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
