<h1 id="6/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

In the [category of complete join-semilattices](../../../../../../category-of-complete-join-semilattices.md), define addition of arrows pointwise by

$$
(f+g)(a)=f(a)\vee g(a),
$$

and let the zero arrow be the constant-bottom map. These form [commutative monoids](../../../../../../commutative-monoid.md). Pointwise join of join-preserving maps again preserves all joins, including the empty join, and composition is additive in each variable. Thus the category has the required semi-additive enrichment.

For an arbitrary set-indexed family $(A_i)$, the product poset $P=\prod_iA_i$, with coordinatewise joins, is the [product in a category](../../../../../../product-category-theory.md). Define $\nu_i:A_i\to P$ by putting an element in coordinate $i$ and bottom in all others. Given join-preserving $f_i:A_i\to B$, define

$$
h((a_i))=\bigvee_i f_i(a_i).
$$

This preserves arbitrary joins by interchanging the two joins, and $h\nu_i=f_i$. It is unique because every tuple is $\bigvee_i\nu_i(a_i)$. Therefore $P$ is also the [coproduct in a category](../../../../../../coproduct.md) with these injections, and its canonical coproduct-to-product map is the identity. This proves the [biproducts of complete join-semilattices](../../../../../../biproducts-of-complete-join-semilattices.md) property, even for arbitrary set-indexed families, and in particular makes this a [semi-additive category](../../../../../../semi-additive-category.md) with the hypotheses of part (ii).

The two-element chain has distinct identity and constant-bottom endomorphisms, so the category is not equivalent to $\mathbf1$. Its addition is idempotent rather than cancellative; for example $1_A+1_A=1_A$ itself supplies an absorbing endomorphism. Hence

$$
\boxed{\mathbf{CSLat}\text{ is a nontrivial semi-additive counterexample}.}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
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
