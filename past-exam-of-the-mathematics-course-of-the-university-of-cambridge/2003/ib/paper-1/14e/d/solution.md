<h1 id="14e/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the standard [basis](../../../../../../basis.md) $e_1,\ldots,e_n$. For the smallest possible rank, set $\alpha e_j=e_j$ for $j\leq r$ and zero otherwise, and set $\beta e_j=-e_j$ for $j\leq s$ and zero otherwise. Then the maps have ranks $r,s$, while their sum has nonzero diagonal entries only for $r<j\leq s$. Hence

$$
\boxed{\operatorname{rank}(\alpha+\beta)=s-r.}
$$

For full rank when $r+s\geq n$, instead take $\alpha e_j=e_j$ for $j\leq r$ and zero otherwise, and $\beta e_j=e_j$ for $j\geq n-s+1$ and zero otherwise. Their supports cover every basis index because $n-s+1\leq r+1$. The sum has diagonal entries one where just one map is nonzero and two where both are nonzero. None vanish over $\mathbb R$, so these [linear maps](../../../../../../linear-map.md) have ranks $r,s$ and

$$
\boxed{\operatorname{rank}(\alpha+\beta)=n.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [14E](../../14e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
