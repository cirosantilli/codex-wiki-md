<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [reflexive pair](../../../../../../reflexive-pair.md) $f,g:A\rightrightarrows B$ has a common section $r:B\to A$ with $fr=gr=1_B$. Form the [pushout in a category](../../../../../../pushout-in-a-category.md) of $f$ and $g$, and write its two maps from $B$ as $j_1,j_2$. Its relation $j_1f=j_2g$, composed with $r$, gives $j_1=j_2=q$. Thus $qf=qg$. Any $h:B\to C$ with $hf=hg$ gives the compatible pair $(h,h)$ for this pushout and therefore factors uniquely through $q$. This proves the [coequalizer of a reflexive pair from a pushout](../../../../../../coequalizer-of-a-reflexive-pair-from-a-pushout.md) construction.

There is a genuine transcription difference: the original PDF says finite products in the finite-colimit assertion, while the TeX says finite coproducts. The PDF assertion is false with products. Even retaining a pushout-existence assumption, the full subcategory of the [Category of sets](../../../../../../category-of-sets.md) on nonempty sets has finite products, pushouts, and all coequalizers, but no [initial object](../../../../../../initial-object.md), hence no empty colimit. Regard the poset with elements $0,a,b,u_0,u_1,\ldots$, order

$$
0<a,b<u_{n+1}<u_n\quad(n\geq0),
$$

and incomparable $a,b$ as a [category](../../../../../../category-split.md). It has finite meets and top $u_0$, hence finite [products in a category](../../../../../../product-category-theory.md). Every [reflexive pair](../../../../../../reflexive-pair.md) in a poset is an equal pair and has its identity as a [coequalizer](../../../../../../coequalizer.md). But $a,b$ have no least upper bound, so they have no [coproduct in a category](../../../../../../coproduct.md).

For the corrected construction using finite coproducts, let $D:\mathcal J\to\mathcal C$ be a finite [diagram in a category](../../../../../../diagram-category-theory.md). Put

$$
X=\coprod_{j\in\mathcal J}D(j),\qquad
Y=\coprod_{a:i\to j}D(i).
$$

Define $s,t:Y\rightrightarrows X$ on the summand indexed by $a:i\to j$ as $\nu_i$ and $\nu_jD(a)$. Maps $h:X\to Z$ with $hs=ht$ are exactly [cocone under a diagram](../../../../../../cocone-under-a-diagram.md) data on $D$. Hence their universal [coequalizer](../../../../../../coequalizer.md) is its [colimit](../../../../../../colimit.md). Replace $s,t$ by the [reflexive pair](../../../../../../reflexive-pair.md)

$$
[s,1_X],[t,1_X]:Y\amalg X\rightrightarrows X,
$$

whose common section is the second injection and whose coequalizer is unchanged. This proves [construction of finite colimits from coproducts and reflexive coequalizers](../../../../../../construction-of-finite-colimits-from-coproducts-and-reflexive-coequalizers.md), including the empty diagram via the empty coproduct:

$$
\boxed{\text{Finite coproducts and reflexive coequalizers suffice for all finite colimits.}}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 119](../../../paper-119-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
