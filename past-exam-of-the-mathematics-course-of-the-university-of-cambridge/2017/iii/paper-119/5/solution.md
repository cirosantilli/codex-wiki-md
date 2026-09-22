<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A [regular category](../../../../../regular-category.md) has finite [categorical limits](../../../../../categorical-limit.md), [coequalizers](../../../../../coequalizer.md) of [kernel pairs](../../../../../kernel-pair.md), and [regular epimorphism](../../../../../regular-epimorphism.md)–[monomorphism](../../../../../monomorphism.md) image factorizations whose [regular epimorphisms](../../../../../regular-epimorphism.md) are stable under every [pullback in a category](../../../../../pullback-category-theory.md). Equivalently, finite limits, pullback-stable [regular epimorphism](../../../../../regular-epimorphism.md)–[monomorphism](../../../../../monomorphism.md) factorizations suffice. In particular, every [strong epimorphism](../../../../../strong-epimorphism.md) in a [regular category](../../../../../regular-category.md) is regular.

For the weaker hypotheses here, interpret an [image factorization](../../../../../image-factorization.md) as $f=me$ with $m:I\hookrightarrow B$ the least [subobject](../../../../../subobject.md) through which $f$ factors, and $e:A\to I$ a [strong epimorphism](../../../../../strong-epimorphism.md). With [pullback in a category](../../../../../pullback-category-theory.md) constructions, the least-subobject characterization itself implies that $e$ is strong: in a lifting square against a [monomorphism](../../../../../monomorphism.md), pull that monomorphism back to $I$; since $e$ factors through this pullback, image minimality forces its mono into $I$ to be invertible, giving the required diagonal. Thus the two descriptions of images agree under the stated hypotheses.

For $a:A'\hookrightarrow A$, define $\exists_f(A')$ as the [image factorization](../../../../../image-factorization.md) subobject of $fa:A'\to B$. For $b:B'\hookrightarrow B$, the [pullback in a category](../../../../../pullback-category-theory.md) universal property and image minimality give

$$
\exists_f(A')\le B'\iff fa\text{ factors through }b
\iff A'\le f^*(B').
$$

Hence

$$
\boxed{\exists_f\dashv f^*.}
$$

This is an [adjunction](../../../../../adjoint-functors.md) between the [posets](../../../../../partially-ordered-set.md) of [subobjects](../../../../../subobject.md).

For [Frobenius reciprocity for subobjects](../../../../../frobenius-reciprocity-for-subobjects.md), factor $fa=me$ through its image $m:I\hookrightarrow B$, and put $P=I\times_BB'$. Its mono into $B$ represents $\exists_f(A')\cap B'$. The [pullback in a category](../../../../../pullback-category-theory.md) of $e$ along the [monomorphism](../../../../../monomorphism.md) $P\to I$ has domain canonically $A'\times_BB'$, which represents $A'\cap f^*(B')$. If [strong epimorphisms](../../../../../strong-epimorphism.md) are stable under pullback along [monomorphisms](../../../../../monomorphism.md), that pulled-back arrow is strong, so its composite with $P\hookrightarrow B$ is an [image factorization](../../../../../image-factorization.md). This gives

$$
\boxed{\exists_f(A'\cap f^*B')=\exists_f(A')\cap B'.}
$$

Equality here is equality of [subobjects](../../../../../subobject.md), hence an isomorphism of their representatives.

Conversely, let $e:X\to Y$ be a [strong epimorphism](../../../../../strong-epimorphism.md) and $b:B'\hookrightarrow Y$ be monic. Its image is all of $Y$: in any [image factorization](../../../../../image-factorization.md) of $e$, the lifting property makes the mono invertible. Apply [Frobenius reciprocity for subobjects](../../../../../frobenius-reciprocity-for-subobjects.md) to $f=e$ and $A'=X$. The induced [morphism](../../../../../morphism.md) $p:X\times_YB'\to B'$ has image all of $B'$, because the image of $bp$ in $Y$ is $B'$. Its [image factorization](../../../../../image-factorization.md) therefore has invertible mono, so $p$ is a [strong epimorphism](../../../../../strong-epimorphism.md). This proves the converse.

We now use the [glued ring categories counterexample to regularity](../../../../../glued-ring-categories-counterexample-to-regularity.md). All [rings](../../../../../ring.md) and [ring homomorphisms](../../../../../ring-homomorphism.md) are unital; the zero [ring](../../../../../ring.md), where $0=1$, is allowed. It is the [terminal object](../../../../../terminal-object.md) of $\mathbf{Rng}$, and there is no unital [ring homomorphism](../../../../../ring-homomorphism.md) from it to a nonzero [ring](../../../../../ring.md). Denote the common zero [ring](../../../../../ring.md) by $Z$, and the newly adjoined [strict initial object](../../../../../strict-initial-object.md) by $\bot$. Nonzero objects in different copies have no [morphisms](../../../../../morphism.md) between them. There is one [morphism](../../../../../morphism.md) from every object to $Z$ and from $\bot$ to every object, and no [morphism](../../../../../morphism.md) into $\bot$ except its identity.

Finite [products in a category](../../../../../product-category-theory.md) and [equalizers](../../../../../equaliser.md) can be described explicitly. The [terminal object](../../../../../terminal-object.md) is $Z$. The [product in a category](../../../../../product-category-theory.md) of two nonzero objects in one copy is their ordinary [ring](../../../../../ring.md) product; the [product in a category](../../../../../product-category-theory.md) of nonzero objects in different copies is $\bot$, since only $\bot$ can map to both. A product with $Z$ is the other factor, and one with $\bot$ is $\bot$. For parallel [morphisms](../../../../../morphism.md) between nonzero objects in the same copy, the ordinary ring [equalizer](../../../../../equaliser.md) works; it is nonzero because its subring contains distinct $0$ and $1$. All other parallel pairs are equal, and their [equalizer](../../../../../equaliser.md) is the identity of the domain. Thus the [construction of small limits from products and equalizers](../../../../../construction-of-small-limits-from-products-and-equalizers.md) gives all finite [categorical limits](../../../../../categorical-limit.md).

Within either ring copy, [monomorphisms](../../../../../monomorphism.md) are precisely injective [ring homomorphisms](../../../../../ring-homomorphism.md): maps from $\mathbb Z[x]$ detect unequal elements. The only monos from outside a copy are the maps $\bot\to X$, and the only [subobjects](../../../../../subobject.md) of $Z$ are $\bot$ and $Z$. Indeed a nonzero [ring](../../../../../ring.md) $R$ is not subterminal, since $\mathbb Z[x]\to R$ can send $x$ to $0$ or to $1$.

Ordinary ring-image factorizations remain [image factorizations](../../../../../image-factorization.md) in the glued [category](../../../../../category-split.md). Their surjective parts remain [strong epimorphisms](../../../../../strong-epimorphism.md): a lifting square into a nonzero ring stays in one copy; a square into $Z$ with mono $\bot\to Z$ would require a nonexistent map from a noninitial domain to $\bot$. Maps with domain $\bot$ are already monic and have identity strong part. Conversely, a [strong epimorphism](../../../../../strong-epimorphism.md) within a ring copy has surjective ring image, since its mono image part must be invertible. A map $\bot\to X$ with $X\ne\bot$ is monic but noninvertible, and therefore cannot be strong. This classifies the [strong epimorphisms](../../../../../strong-epimorphism.md) as the identities of $\bot$ and the surjective homomorphisms in the copies, including maps to $Z$.

Pullback along a [monomorphism](../../../../../monomorphism.md) within a copy preserves those surjections, using the given regularity of $\mathbf{Rng}$. Pullback along $\bot\to X$ gives $1_\bot$, and these exhaust the additional monos, including those into $Z$. Thus [strong epimorphisms](../../../../../strong-epimorphism.md) are stable under pullback along monos, so [Frobenius reciprocity for subobjects](../../../../../frobenius-reciprocity-for-subobjects.md) holds.

However, let $e:\mathbb Z_{\mathcal D}\to Z$ be the surjective [ring homomorphism](../../../../../ring-homomorphism.md) in the first copy, and pull it back along $\mathbb Z[x]_{\mathcal E}\to Z$ in the other copy. The resulting arrow is

$$
\bot\longrightarrow\mathbb Z[x]_{\mathcal E}.
$$

It is not even an [epimorphism](../../../../../epimorphism.md), since the distinct evaluation [ring homomorphisms](../../../../../ring-homomorphism.md) $x\mapsto0$ and $x\mapsto1$ to $\mathbb Z_{\mathcal E}$ agree after composing with $\bot\to\mathbb Z[x]_{\mathcal E}$. Since $e$ is strong, it would be a [regular epimorphism](../../../../../regular-epimorphism.md) in a [regular category](../../../../../regular-category.md), whose pullbacks must be regular, in particular epic. Therefore **the glued category has finite limits and images and satisfies Frobenius reciprocity, but is not regular**.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
