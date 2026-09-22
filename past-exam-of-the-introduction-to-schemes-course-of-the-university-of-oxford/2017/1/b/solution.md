<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**No.** Let $k=\mathbb F_2$ be the [field with two elements](../../../../field-with-two-elements.md), put $A=k[\varepsilon]/(\varepsilon^2)$, and take the [closed immersion](../../../../closed-immersion.md)

$$
\boxed{f:\operatorname{Spec}k\hookrightarrow\operatorname{Spec}A}
$$

induced by the [ring homomorphism](../../../../ring-homomorphism.md) $q:A\twoheadrightarrow k$ with $q(\varepsilon)=0$.

For every [field](../../../../field.md) $K$, a [ring homomorphism](../../../../ring-homomorphism.md) $\alpha:A\to K$ must send $\varepsilon$ to zero: $\alpha(\varepsilon)^2=0$, and a [field](../../../../field.md) has no nonzero [nilpotent elements](../../../../nilpotent.md). Consequently $\alpha$ factors uniquely through $q$. Passing from [ring homomorphisms](../../../../ring-homomorphism.md) to [morphisms of schemes](../../../../morphism-of-schemes.md) between [affine schemes](../../../../affine-scheme.md) gives a [bijection](../../../../bijection.md)

$$
f(\operatorname{Spec}K):\operatorname{Hom}_{\mathrm{Sch}}(\operatorname{Spec}K,\operatorname{Spec}k)
\xrightarrow{\ \sim\ }
\operatorname{Hom}_{\mathrm{Sch}}(\operatorname{Spec}K,\operatorname{Spec}A).
$$

This concerns all [morphisms of schemes](../../../../morphism-of-schemes.md), without requiring them to be over $k$: if $K$ does not have [characteristic](../../../../characteristic-of-a-field.md) two, both sets are empty; otherwise each contains exactly one element.

Nevertheless, $f$ is not an [isomorphism of schemes](../../../../isomorphism-of-schemes.md). Its map on [global sections](../../../../global-section.md) is $q$, whose [kernel of a ring homomorphism](../../../../kernel-of-a-ring-homomorphism.md) contains the nonzero element $\varepsilon$, so $q$ is not a [ring isomorphism](../../../../ring-isomorphism.md). The target is the [nonreduced scheme](../../../../nonreduced-scheme.md) defined by the [dual numbers](../../../../dual-number.md), whereas the source is a [reduced scheme](../../../../reduced-scheme.md). This illustrates why [field-valued points do not detect nilpotents](../../../../field-valued-points-do-not-detect-nilpotents.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the introduction to schemes course of the University of Oxford](../../../split.md)
5. [Introduction to schemes course of the University of Oxford](../../../../introduction-to-schemes-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
