<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A [pointed category](../../../../../pointed-category.md) has a [zero object](../../../../../zero-object.md), both initial and terminal. Factoring through that object gives a [zero morphism](../../../../../zero-morphism.md) $0_{A,B}$ between any two objects. In this paper a [semi-additive structure](../../../../../commutative-monoid-enrichment.md) means [commutative-monoid enrichment](../../../../../commutative-monoid-enrichment.md): every hom-set is a [commutative monoid](../../../../../commutative-monoid.md) with additive zero, and composition distributes over addition in both variables. No existence of finite [products in a category](../../../../../product-category-theory.md) is included in this last definition. This convention matters for the final one-object example; under the stronger convention requiring finite [biproducts](../../../../../biproduct.md), that example would not be a [semi-additive category](../../../../../semi-additive-category.md).

Let $c_{A,B}:A+B\to A\times B$ be the given canonical isomorphism. Transfer the coproduct injections across $c_{A,B}$, so $A\times B$ is also a [coproduct in a category](../../../../../coproduct.md), with injections

$$
i_1=\langle1_A,0\rangle,\qquad i_2=\langle0,1_B\rangle.
$$

Write $\nabla_B:B\times B\to B$ for the [morphism](../../../../../morphism.md) whose composites with $i_1,i_2$ are both $1_B$. For $f,g:A\to B$, define the [biproduct-induced addition of morphisms](../../../../../biproduct-induced-addition-of-morphisms.md) by

$$
\boxed{f+g=\nabla_B\langle f,g\rangle=[1_B,1_B]c_{B,B}^{-1}\langle f,g\rangle.}
$$

The zero is the existing [zero morphism](../../../../../zero-morphism.md). We verify the laws from the universal properties, without assuming addition in advance.

All finite canonical maps from coproducts to products are isomorphisms, by induction from the binary ones and the [zero object](../../../../../zero-object.md). Thus both $(B\times B)\times B$ and $B\times(B\times B)$ are ternary [coproducts in a category](../../../../../coproduct.md). The two iterated fold maps to $B$ agree on each of the three injections, hence are equal. Applying this to $\langle f,g,h\rangle$ gives associativity. The interchange $B\times B\to B\times B$ swaps the two injections, so its composite with $\nabla_B$ is $\nabla_B$, giving commutativity. Finally $\langle f,0\rangle=i_1f$, so $f+0=f$, and similarly $0+f=f$.

Precomposition is additive because $\langle f,g\rangle u=\langle fu,gu\rangle$. For $v:B\to C$, the [morphisms](../../../../../morphism.md) $v\nabla_B$ and $\nabla_C(v\times v)$ agree on both injections, so they agree; consequently $v(f+g)=vf+vg$. Composition with a [zero morphism](../../../../../zero-morphism.md) is zero. This proves the [commutative-monoid enrichment](../../../../../commutative-monoid-enrichment.md).

It is unique. In any such enrichment, the additive zero morphisms agree with the pointed ones, since each map to or from the [zero object](../../../../../zero-object.md) belongs to a singleton hom-set. The projections of $i_1p_1+i_2p_2$ from $A\times B$ are respectively $p_1,p_2$ by bilinearity, so

$$
i_1p_1+i_2p_2=1_{A\times B}.
$$

For $A=B$, composing on the left by $\nabla_B$ and on the right by $\langle f,g\rangle$ forces the displayed formula for $f+g$. Thus **the biproducts determine exactly one such enrichment**.

For the last part, the underlying one-object [category](../../../../../category-split.md) has endomorphism [monoid](../../../../../monoid.md) $(\mathbb N,\cdot)$, including $0$, and identity $1$. Its usual addition gives a [commutative-monoid enrichment](../../../../../commutative-monoid-enrichment.md). Any permutation $\sigma$ of the [prime numbers](../../../../../prime-number.md) extends, by unique [prime factorization](../../../../../fundamental-theorem-of-arithmetic.md), to a multiplicative [monoid automorphism](../../../../../monoid-automorphism.md) $\phi_\sigma:\mathbb N\to\mathbb N$, fixing $0,1$. Transport addition by

$$
\boxed{a\mathbin{\oplus_\sigma}b=\phi_\sigma^{-1}\bigl(\phi_\sigma(a)+\phi_\sigma(b)\bigr).}
$$

This is a [commutative monoid](../../../../../commutative-monoid.md) operation with zero $0$, and multiplication distributes over it: applying $\phi_\sigma$ reduces each distributive law to the ordinary one in $\mathbb N$. Thus each operation supplies a [semi-additive structure](../../../../../commutative-monoid-enrichment.md) on the same fixed composition law.

For each [odd prime](../../../../../odd-prime.md) $p$, take $\sigma$ to interchange $2$ and $p$, fixing every other prime. Then

$$
1\mathbin{\oplus_\sigma}1=\phi_\sigma^{-1}(2)=p.
$$

Different choices of $p$ give different additions, and there are infinitely many [prime numbers](../../../../../prime-number.md). Hence there are **infinitely many distinct semi-additive structures**, even though these transported structures are isomorphic as enriched [categories](../../../../../category-split.md). The underlying one-object [category](../../../../../category-split.md) has no [terminal object](../../../../../terminal-object.md), because its endomorphism [set](../../../../../set-split.md) is not a singleton, so it indeed has no finite [products in a category](../../../../../product-category-theory.md).

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
