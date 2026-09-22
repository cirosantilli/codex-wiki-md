<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A [regular category](../../../../../regular-category.md) has [finite limits](../../../../../finite-limit.md), [coequalizers](../../../../../coequalizer.md) of [kernel pairs](../../../../../kernel-pair.md), and [regular epimorphisms](../../../../../regular-epimorphism.md) stable under pullback. Equivalently, every morphism factors as a regular epimorphism followed by a monomorphism, and these factorizations are stable under pullback. A [regular functor](../../../../../regular-functor.md) preserves finite limits and regular epimorphisms, hence also preserves these [image factorizations](../../../../../image-factorization.md).

For this question, the [capital regular category](../../../../../capital-regular-category.md) convention is the one in which every [well-supported object](../../../../../well-supported-object.md) is a [well-pointed object in a category](../../../../../well-pointed-object-in-a-category.md). Here an object $A$ is well-supported if $A\to1$ is a regular epimorphism. It is well-pointed if a [subobject](../../../../../subobject.md) $m:B\hookrightarrow A$ through which every point $1\to A$ factors must be the whole object. This convention is documented in [Definitions 1.1–1.3](https://www2.math.ethz.ch/EMIS/journals/TAC/volumes/16/31/16-31.pdf). It imposes no such point-detection requirement on objects whose support is a proper subobject of $1$. In particular, it should not be replaced here by the stronger assertion that $\mathcal A(1,-)$ reflects every isomorphism.

First prove two facts about a capital regular category $\mathcal A$. Every well-supported object $A$ has a point. Otherwise $A\times A$ is well-supported and has no points, so its diagonal $A\hookrightarrow A\times A$ contains all points and is invertible. That makes $A$ a [subterminal object](../../../../../subterminal-object.md); the regular epimorphism $A\to1$ is then also monic and hence invertible, contradicting the absence of a point. If $e:X\to Y$ is a regular epimorphism and $y:1\to Y$ is a point, its [pullback in a category](../../../../../pullback-category-theory.md) is a well-supported object over $1$, so it has a point lifting $y$. Thus the [representable functor](../../../../../representable-functor.md)

$$
\Gamma=\mathcal A(1,-):\mathcal A\to\mathbf{Set}
$$

preserves regular epimorphisms; it already preserves all existing limits. Hence **$\Gamma$ is a regular functor**. Second, if $\Gamma X$ is a singleton, its unique point $x:1\to X$ is a monomorphism, $X$ is well-supported, and $x$ contains all points of $X$. Well-pointedness makes $x$ invertible. Thus $\Gamma$ reflects terminal objects, even though it need not reflect arbitrary isomorphisms.

Now let $\mathcal C$ be a [small category](../../../../../small-category.md) that is a [regular category](../../../../../regular-category.md). For each object $B$, its [slice category](../../../../../slice-category.md) $\mathcal C/B$ is small and regular: finite limits, images and the stability of regular epimorphisms are computed using the corresponding constructions in $\mathcal C$. By the permitted capitalization result choose a [conservative functor](../../../../../conservative-functor.md) that is regular,

$$
J_B:\mathcal C/B\to\mathcal A_B,
$$

with $\mathcal A_B$ a small capital regular category. The base-change functor $B^*:\mathcal C\to\mathcal C/B$, given by $X\mapsto(X\times B\to B)$, preserves finite limits and regular epimorphisms. So does

$$
R_B=\Gamma_BJ_BB^*:\mathcal C\to\mathbf{Set}.
$$

Taking these as the coordinates defines a regular functor

$$
R:\mathcal C\to\mathbf{Set}^{\operatorname{ob}\mathcal C}.
$$

The exponent is a [set](../../../../../set-split.md) of indices, so this is a power of the [Category of sets](../../../../../category-of-sets.md), with finite limits and regular epimorphisms computed coordinatewise.

To prove reflection of isomorphisms, suppose $R(f)$ is invertible for $f:A\to B$. In $\mathcal C/B$, the object $(A,f)$ is the pullback of $B^*f:(A\times B\to B)\to(B\times B\to B)$ along the point given by the diagonal $B\to B\times B$. Applying $\Gamma_BJ_B$ shows that $\Gamma_BJ_B(A,f)$ is the fibre of the bijection $R_B(f)$ over this diagonal point, and is a singleton. The preceding lemma gives $J_B(A,f)\cong1$ through its canonical arrow to $1$. Since $J_B$ reflects isomorphisms, $(A,f)\to(B,1_B)$ is invertible. Its underlying morphism is $f$. Therefore

$$
\boxed{R:\mathcal C\to\mathbf{Set}^{\operatorname{ob}\mathcal C}\text{ is regular and reflects isomorphisms}.}
$$

In the small-category setting of this representation result, the elementary condition for replacing the power by one copy of $\mathbf{Set}$ is:

$$
\boxed{\text{Every object is either well-supported or a strict initial object}.}
$$

This is [almost total support for a regular category](../../../../../almost-total-support-for-a-regular-category.md). “Strict initial” means initial and every arrow into it is invertible; the condition allows the case in which all objects are well-supported and no initial object exists.

For necessity, let $V:\mathcal C\to\mathbf{Set}$ be regular and conservative. If $VA\ne\varnothing$, factor $A\to1$ through its [support of an object in a regular category](../../../../../support-of-an-object-in-a-regular-category.md) $S\hookrightarrow1$. Preservation of images gives $VS=1$. Conservativity makes $S\to1$ invertible, so $A$ is well-supported. If $VA=\varnothing$, then for every $X$ the projection $A\times X\to A$ is sent to the bijection $\varnothing\to\varnothing$, hence is invertible. Its inverse followed by the other projection supplies an arrow $A\to X$. For any two such arrows, their equalizer is sent to a bijection onto $VA$, hence is invertible, proving uniqueness. Thus $A$ is initial. If $X\to A$ exists, then $VX\to\varnothing$ exists, so $VX=\varnothing$ and that arrow is sent to a bijection. Conservativity makes it invertible. Hence $A$ is strict initial.

For sufficiency, choose the permitted conservative regular functor $J:\mathcal C\to\mathcal A$ into a small capital regular category, and put $V=\Gamma J$. This is regular. A well-supported object of $\mathcal C$ is sent to a well-supported object of $\mathcal A$, which has a point. A non-well-supported object is strict initial by the condition, and is consequently a proper subterminal object. The functor $J$ preserves subterminality and reflects the noninvertibility of its arrow to $1$; its image is a proper subterminal object and has no points. Thus $VA$ is empty exactly on the non-well-supported objects.

Suppose $Vf$ is a bijection for $f:A\to B$. If both sets are empty, $A$ and $B$ are strict initial objects and $f$ is invertible. Otherwise $A,B$ are well-supported. Factor $Jf$ as a regular epimorphism followed by a monomorphism $m:I\hookrightarrow JB$. Surjectivity of $Vf$ makes every point of $JB$ factor through $m$; capitality of $\mathcal A$ makes $m$ invertible. Hence $Jf$ is a regular epimorphism. Its kernel pair $P=JA\times_{JB}JA$ is well-supported, because $P\to JA$ and $JA\to1$ are regular epimorphisms. Injectivity of $Vf$ implies that every point of $P$ has equal coordinates, and therefore factors through the diagonal $JA\hookrightarrow P$. Since $P$ is well-pointed, this diagonal is invertible. Thus $Jf$ is also monic, hence an isomorphism, and conservativity of $J$ makes $f$ invertible. This proves sufficiency with actual point and image arguments, rather than asserting that global sections of every capital regular category is conservative.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 21](../../paper-21-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
