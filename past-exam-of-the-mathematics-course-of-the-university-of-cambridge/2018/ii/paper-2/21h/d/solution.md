<h1 id="21h/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [Simplicial approximation theorem](../../../../../../simplicial-approximation-theorem.md) states that if $K$ is a finite simplicial complex, $L$ is a simplicial complex, and $f:|K|\to|L|$ is continuous, then for some $r\geq0$ there is a simplicial approximation $g:K^{(r)}\to L$ to $f$.

The target open stars form an open cover of $|L|$, so their inverse images under $f$ form an open cover of the compact metric space $|K|$. The [Lebesgue number lemma](../../../../../../lebesgue-number-lemma.md) supplies $\delta>0$ such that every subset of diameter below $\delta$ lies in one inverse image. Choose $r$ so large that every vertex star in $K^{(r)}$ has diameter below $\delta$; this is possible because its diameter is at most twice $\mu(K^{(r)})$ and the mesh tends to zero.

For each vertex $v$ choose a vertex $w(v)$ of $L$ such that

$$
f(\operatorname{st}_{K^{(r)}}(v))
\subseteq\operatorname{st}_L(w(v)).
$$

If $v_0,\ldots,v_q$ span a simplex, a point in its relative interior belongs to all their open stars. Its image belongs to all the open stars of $w(v_0),\ldots,w(v_q)$, so these target vertices span a simplex. Thus $v\mapsto w(v)$ extends to a simplicial map $g$, and its defining inclusion says exactly that $g$ approximates $f$. This proves the theorem.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [21H](../../21h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
