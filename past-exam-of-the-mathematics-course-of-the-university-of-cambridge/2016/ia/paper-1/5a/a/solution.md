<h1 id="5a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [suffix notation](../../../../../../einstein-notation.md) with indices ranging from $1$ to $3$, and sum over repeated indices. By the component definitions of the [dot product](../../../../../../dot-product.md) and [cross product](../../../../../../cross-product.md),

$$
\mathbf a\cdot(\mathbf b\times\mathbf c)
=a_i\epsilon_{ijk}b_jc_k.
$$

The [Levi-Civita symbol](../../../../../../levi-civita-symbol.md) is unchanged by a cyclic permutation of its three indices: the cycle is two transpositions and hence has positive sign. Thus $\epsilon_{ijk}=\epsilon_{kij}$. Commuting the scalar components gives

$$
a_i\epsilon_{ijk}b_jc_k
=c_k\epsilon_{kij}a_ib_j
=c_k(\mathbf a\times\mathbf b)_k.
$$

Therefore the [scalar triple product](../../../../../../scalar-triple-product.md) obeys

$$
\boxed{\mathbf a\cdot(\mathbf b\times\mathbf c)
=\mathbf c\cdot(\mathbf a\times\mathbf b).}
$$

**Cyclically moving the vectors preserves the scalar triple product; interchanging just two reverses its sign.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5A](../../5a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
