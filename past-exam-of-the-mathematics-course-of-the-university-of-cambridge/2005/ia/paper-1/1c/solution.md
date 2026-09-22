<h1 id="1c/solution">Solution</h1>

↑ **Parent:** [1C](../1c.md)

For the unheaded continuation, write the [vector triple product](../../../../../vector-triple-product.md) as

$$
[\mathbf a\times(\mathbf b\times\mathbf c)]_i=\epsilon_{ijk}a_j\epsilon_{klm}b_lc_m.
$$

The [Levi-Civita symbol](../../../../../levi-civita-symbol.md) contraction is $\epsilon_{ijk}\epsilon_{klm}=\delta_{il}\delta_{jm}-\delta_{im}\delta_{jl}$. One way to check its sign is to fix distinct $i,j$: the only nonzero term has $k$ the remaining index, and the pairs $(l,m)=(i,j),(j,i)$ contribute $+1,-1$ respectively. When $i=j$, both sides vanish. Contracting with the [vectors](../../../../../vector.md) now gives both requested notations:

$$
\boxed{[\mathbf a\times(\mathbf b\times\mathbf c)]_i=b_i a_jc_j-c_i a_jb_j,\qquad \mathbf a\times(\mathbf b\times\mathbf c)=\mathbf b(\mathbf a\cdot\mathbf c)-\mathbf c(\mathbf a\cdot\mathbf b).}
$$

If $\mathbf a$ and $\mathbf b$ are [orthogonal](../../../../../orthogonal-vectors.md), then $\mathbf a\cdot\mathbf b=0$. With the specified $\mathbf c$, the perpendicularity of the [cross product](../../../../../cross-product.md) gives $\mathbf a\cdot\mathbf c=|\mathbf a|^2$. Therefore

$$
\boxed{\mathbf a\times(\mathbf b\times\mathbf c)=|\mathbf a|^2\mathbf b.}
$$

The same answer covers the degenerate case in which one of these two [vectors](../../../../../vector.md) is zero.

## ↑ Ancestors (10)

1. [1C](../1c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
