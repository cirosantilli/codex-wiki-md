<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose a [Cartan subalgebra](../../../../../../cartan-subalgebra.md), [simple roots](../../../../../../simple-root.md) $\alpha_1,\ldots,\alpha_r$, and [root vectors](../../../../../../root-vector.md) $e_i,f_i$ normalized by $[e_i,f_i]=h_i=\alpha_i^\vee$. Let

$$
\rho^\vee=\tfrac12\sum_{\alpha\in R^+}\alpha^\vee,\qquad h=2\rho^\vee=\sum_i c_i h_i,
\qquad e=\sum_i e_i,\qquad f=\sum_i c_i f_i.
$$

Here the [coroots](../../../../../../coroot.md) lie in the [Cartan subalgebra](../../../../../../cartan-subalgebra.md), and $\alpha_i(\rho^\vee)=1$. This last identity is the [Weyl vector](../../../../../../half-sum-of-positive-roots.md) identity applied to the [dual root system](../../../../../../dual-root-system.md). For distinct [simple roots](../../../../../../simple-root.md), $\alpha_i-\alpha_j$ is not a root, hence $[e_i,f_j]=0$. Consequently

$$
[e,f]=\sum_i c_i h_i=h,\qquad [h,e]=2e,\qquad[h,f]=-2f.
$$

These are exactly the [sl2 Lie algebra](../../../../../../sl2-lie-algebra.md) relations. For nonzero $\mathfrak g$ the resulting homomorphism from $\mathfrak{sl}_2$ is nonzero and therefore injective, since $\mathfrak{sl}_2$ is simple. Its image is a [Principal sl2 subalgebra](../../../../../../principal-sl2-subalgebra.md). Equivalently its raising element is a [principal nilpotent element](../../../../../../principal-nilpotent-element.md), a nilpotent element with [Lie algebra centralizer](../../../../../../centralizer-of-an-element-of-a-lie-algebra.md) of [dimension](../../../../../../dimension-vector-space.md) equal to the rank. The construction works for a [semisimple Lie algebra](../../../../../../semisimple-lie-algebra-split.md) with several simple factors by taking the triple in every factor, giving one diagonally embedded $\mathfrak{sl}_2$. This is the [construction of a principal sl2 triple](../../../../../../construction-of-a-principal-sl2-triple.md).

For a representation $V$, restrict to this subalgebra and take its [formal character](../../../../../../formal-character-of-a-weight-module.md). If $V_\mu$ is the [weight space](../../../../../../weight-space.md) for the original [Cartan subalgebra](../../../../../../cartan-subalgebra.md), the resulting [q-character of a highest-weight representation](../../../../../../q-character-of-a-highest-weight-representation.md), or the analogous q-character for any finite-dimensional representation, is

$$
\boxed{\operatorname{ch}_q V=\operatorname{tr}_V(q^{2\rho^\vee})=\sum_\mu\dim(V_\mu)\,q^{\mu(2\rho^\vee)}.}
$$

It is independent of conjugating the chosen principal triple. In particular a root $\beta=\sum_i k_i\alpha_i$ has grading $\beta(h)=2\sum_i k_i$. Some conventions use $q^{h/2}$ instead; that convention divides all exponents here by two. The normalization above agrees with the ordinary [sl2 Lie algebra](../../../../../../sl2-lie-algebra.md) character in the preceding part.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
