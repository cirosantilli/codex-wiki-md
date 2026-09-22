<h1 id="6/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

In a [semi-additive category](../../../../../../semi-additive-category.md), hom-sets are [commutative monoids](../../../../../../commutative-monoid.md) and composition is additive in both variables. Write $S=\coprod_iA_i$, $P=\prod_iA_i$, with injections $\nu_i$ and projections $\pi_i$. The canonical $c:S\to P$ has $\pi_ic\nu_j=1_{A_i}$ when $i=j$ and zero otherwise. Define

$$
d=\sum_{i=1}^n\nu_i\pi_i:P\to S.
$$

Bilinearity gives

$$
\pi_kcd=\sum_i(\pi_kc\nu_i)\pi_i=\pi_k,\qquad
dc\nu_j=\sum_i\nu_i(\pi_ic\nu_j)=\nu_j.
$$

The universal properties of the [product in a category](../../../../../../product-category-theory.md) and [coproduct in a category](../../../../../../coproduct.md) imply $cd=1_P$ and $dc=1_S$. For the empty family, $S$ is initial and $P$ terminal. Their endomorphisms are necessarily the identity and the zero morphism; the zero map $P\to S$ therefore also gives inverse composites. Thus the comparison is an isomorphism for every finite family, giving a [biproduct](../../../../../../biproduct.md):

$$
\boxed{c^{-1}=\sum_{i=1}^n\nu_i\pi_i.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [6](../../6.md)
3. [Paper 119](../../../paper-119-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
