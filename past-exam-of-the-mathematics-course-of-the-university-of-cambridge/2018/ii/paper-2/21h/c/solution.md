<h1 id="21h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [simplicial map](../../../../../../simplicial-map.md) $g:K\to L$ is a [simplicial approximation](../../../../../../simplicial-approximation.md) to $f:|K|\to|L|$ when

$$
f(\operatorname{st}_K(v))
\subseteq\operatorname{st}_L(g(v))
$$

for every vertex $v$, where $\operatorname{st}$ denotes the [open star in a simplicial complex](../../../../../../open-star-in-a-simplicial-complex.md).

Fix $x$ in a simplex with vertices $v_0,\ldots,v_q$, retaining only vertices with positive barycentric coordinate at $x$. Then $x\in\operatorname{st}_K(v_i)$ for every $i$, so $f(x)$ lies in every $\operatorname{st}_L(g(v_i))$. The vertices $g(v_i)$ and the vertices carrying the barycentric coordinates of $f(x)$ consequently span a common simplex of $L$. Both $f(x)$ and $|g|(x)$ lie in its convex realization. The [straight-line homotopy from a simplicial approximation](../../../../../../straight-line-homotopy-from-a-simplicial-approximation.md)

$$
\boxed{H(x,t)=(1-t)f(x)+t|g|(x)}
$$

is therefore well-defined and continuous, with endpoints $f$ and $|g|$.

## ↑ Ancestors (11)

1. [C](../c.md)
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
