<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Here use the [left lifting property against monomorphisms](../../../../../../left-lifting-property-against-monomorphisms.md) as the definition of “strong”; epimorphicity will be established separately. In a lifting square write $g:C\to D$, $m:A\to B$, $k:C\to A$ and $l:D\to B$, with $mk=lg$ and $m$ a [monomorphism](../../../../../../monomorphism.md). Any two lifts agree because $mt=mt'=l$.

First let $g$ be the [coequalizer](../../../../../../coequalizer.md) of $r,s:E\rightrightarrows C$. Every [coequalizer](../../../../../../coequalizer.md) is an [epimorphism](../../../../../../epimorphism.md): if $ug=vg$, the uniqueness clause for the [coequalizer](../../../../../../coequalizer.md) applied to this common composite gives $u=v$. Moreover,

$$
mkr=lgr=lgs=mks,
$$

so $kr=ks$ by [monomorphism](../../../../../../monomorphism.md) cancellation. The [coequalizer](../../../../../../coequalizer.md) therefore supplies $t:D\to A$ with $tg=k$. Then $mtg=mk=lg$, and [epimorphism](../../../../../../epimorphism.md) cancellation gives $mt=l$. This proves that [regular epimorphisms are strong epimorphisms](../../../../../../regular-epimorphisms-are-strong-epimorphisms.md).

If $g:C\to D$ is also a [monomorphism](../../../../../../monomorphism.md), take $m=g$, $k=1_C$ and $l=1_D$. Its lift satisfies $tg=1_C$ and $gt=1_D$. Hence **[monic lifting-only strong morphisms are invertible](../../../../../../monic-lifting-only-strong-morphisms-are-invertible.md)**.

Next suppose $gf:A\to C$ has the [left lifting property against monomorphisms](../../../../../../left-lifting-property-against-monomorphisms.md). Given a lifting square for $g:B\to C$, with $mk=lg$, precompose its top arrow with $f$. A lift for $gf$ gives $t:C\to X$ with $mt=l$ and $tgf=kf$. Crucially, one does not cancel $f$: instead $mtg=lg=mk$, and the [monomorphism](../../../../../../monomorphism.md) $m$ gives $tg=k$. Thus **the right factor of a strong composite is strong**, proving [right-factor cancellation for lifting-only strong morphisms](../../../../../../right-factor-cancellation-for-lifting-only-strong-morphisms.md).

Finally, in $u=iv$ with $u$ strong and $i$ monic, the preceding result makes $i$ strong. The monic-strong argument then makes **$i$ an isomorphism**. None of these arguments assumed that a lifting-only strong morphism was already epic.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
