<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [algebraic dual of a direct sum](../../../../../../algebraic-dual-of-a-direct-sum.md) is a product, rather than another [direct sum](../../../../../../direct-sum.md). The map

$$
R:V^*\longrightarrow\prod_{i\ge1}V_i^*,\qquad\ell\longmapsto(\ell|_{V_i})_i
$$

is injective, since the summands span $V$. Given any family $(\ell_i)_i$, define $\ell((v_i)_i)=\sum_i\ell_i(v_i)$. This sum is finite for each vector, regardless of whether the family of functionals has finite support. It defines a [linear functional](../../../../../../linear-functional.md) and is inverse to $R$. Hence this is a natural vector-space isomorphism.

The [algebraic contragredient representation](../../../../../../algebraic-contragredient-representation.md) is $(\pi^*(g)\ell)(v)=\ell(\pi(g^{-1})v)$. On the $i$th coordinate,

$$
(\pi^*(g)\ell)_i(v_i)=\ell_i(\chi_i(g)^{-1}v_i)=\chi_i(g)^{-1}\ell_i(v_i).
$$

Thus $R$ intertwines the actions and gives

$$
\boxed{(V^*,\pi^*)\cong\prod_{i\ge1}(V_i^*,\chi_i^{-1}).}
$$

No smoothness restriction has yet been imposed on that product.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
