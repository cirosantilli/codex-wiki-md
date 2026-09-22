<h1 id="20h/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [simplicial approximation](../../../../../../simplicial-approximation.md) $g:K\to L$ to $f:|K|\to|L|$ is a vertex map satisfying the open-star condition

$$
f(\operatorname{st}_K(v))\subseteq\operatorname{st}_L(g(v))
$$

for every vertex $v$. Here an open star consists of points whose barycentric coordinate at that vertex is positive. This condition ensures that the images of the vertices of every simplex span a simplex of $L$, and the vertex map extends linearly over simplices.

To triangulate $|K|\times|L|$, order the vertices of each complex consistently. For each product $[v_0,\ldots,v_p]\times[w_0,\ldots,w_q]$, use the simplices whose vertices $(v_i,w_j)$ follow monotone lattice paths from $(0,0)$ to $(p,q)$, taking a step in one coordinate at a time. These prism triangulations agree on faces and cover the product.

If $g,h$ both approximate $f$, choose $x$ in the relative interior of a simplex $\sigma$. Then $x$ belongs to the open star of every vertex $v$ of $\sigma$. Hence $f(x)$ belongs to every open star of $g(v)$ and $h(v)$. Its unique carrier simplex in $L$ contains all these vertices. Thus $g(\sigma)$ and $h(\sigma)$ are faces of that one simplex, proving that $g,h$ are [contiguous simplicial maps](../../../../../../contiguous-simplicial-maps.md).

$$
\boxed{g,h\text{ approximate }f\ \Longrightarrow\ g,h\text{ are contiguous}.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [20H](../../20h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
