<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [semi-additive category](../../../../../../semi-additive-category.md) has [commutative-monoid enrichment](../../../../../../commutative-monoid-enrichment.md): each [hom-set](../../../../../../hom-set.md) is a [commutative monoid](../../../../../../commutative-monoid.md), and [composition in a category](../../../../../../composition-in-a-category.md) preserves addition and zero in each variable. In the finite-biproduct convention, which we use here, it also has finite [products in a category](../../../../../../product-category-theory.md) and [coproducts in a category](../../../../../../coproduct.md). A [preadditive category](../../../../../../preadditive-category.md) has [abelian groups](../../../../../../abelian-group.md) as its [hom-sets](../../../../../../hom-set.md), with composition additive in each variable; this definition alone does not require finite [products in a category](../../../../../../product-category-theory.md) or a [zero object](../../../../../../zero-object.md).

Let $P=\prod_{i=1}^n A_i$ with projections $p_i$. Define $i_j:A_j\to P$ by $p_i i_j=1_{A_j}$ for $i=j$ and $p_i i_j=0$ otherwise. Bilinearity gives

$$
p_k\left(\sum_j i_jp_j\right)=p_k,
$$

so product uniqueness gives $\sum_j i_jp_j=1_P$. For a family $f_j:A_j\to X$, set $f=\sum_j f_jp_j$. Then $fi_j=f_j$. If $h:P\to X$ has the same restrictions, $h=h\sum_j i_jp_j=\sum_j f_jp_j=f$. Thus the [product in a category](../../../../../../product-category-theory.md) is also the [coproduct in a category](../../../../../../coproduct.md), with its canonical injections. Conversely, the analogous construction from a finite [coproduct in a category](../../../../../../coproduct.md) gives projections and the same identities, proving that it is a [product in a category](../../../../../../product-category-theory.md).

For the empty family, a [terminal object](../../../../../../terminal-object.md) $T$ has a singleton endomorphism monoid, so $1_T=0$. Every map $T\to X$ equals its composite with $1_T=0$, hence equals the zero map; this map exists by enrichment. Therefore $T$ is also an [initial object](../../../../../../initial-object.md), a [zero object](../../../../../../zero-object.md). The dual argument applies to an [initial object](../../../../../../initial-object.md). Consequently **finite [products in a category](../../../../../../product-category-theory.md) and [coproducts in a category](../../../../../../coproduct.md) coincide canonically as [biproducts](../../../../../../biproduct.md)**, including the nullary case.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [7](../../7.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
