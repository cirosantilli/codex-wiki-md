<h1 id="1e/solution">Solution</h1>

↑ **Parent:** [1E](../1e.md)

The [dual space](../../../../../dual-space.md) is $V^*=\operatorname{Hom}_{\mathbb R}(V,\mathbb R)$, the vector space of real-valued [linear maps](../../../../../linear-map.md) on $V$, with pointwise addition and scalar multiplication. Choose a [basis](../../../../../basis.md) $e_1,\ldots,e_n$ of $V$. Every $v$ has unique coordinates $v=\sum_i x_ie_i$, so $e^i(v)=x_i$ defines a [linear functional](../../../../../linear-functional.md), with $e^i(e_j)=\delta_{ij}$.

If $\sum_i a_ie^i=0$, evaluation on $e_j$ gives $a_j=0$, proving linear independence. For any $\ell\in V^*$, linearity gives $\ell(v)=\sum_i x_i\ell(e_i)$, hence $\ell=\sum_i\ell(e_i)e^i$. Thus the [dual basis](../../../../../dual-basis.md) spans the [dual space](../../../../../dual-space.md) as well, proving

$$
\boxed{\dim V^*=n=\dim V.}
$$

## ↑ Ancestors (10)

1. [1E](../1e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
