<h1 id="9/solution">Solution</h1>

↑ **Parent:** [9](../9.md)

A [group homomorphism](../../../../group-homomorphism.md) $h:G\to F$ preserves multiplication: $h(g_1g_2)=h(g_1)h(g_2)$. It sends the [identity element](../../../../identity-element.md) to the identity and [inverse elements](../../../../inverse-element.md) to [inverse elements](../../../../inverse-element.md). Its [group kernel](../../../../kernel-of-a-group-homomorphism.md) is $K=\{g\in G:h(g)=e_F\}$. This contains $e_G$ and is closed under multiplication and [inverse elements](../../../../inverse-element.md), so it is a [subgroup](../../../../subgroup.md). For $k\in K$ and $g\in G$,

$$
h(gkg^{-1})=h(g)e_Fh(g)^{-1}=e_F.
$$

Thus $gKg^{-1}\subseteq K$; applying the same argument with $g^{-1}$ gives equality. Hence **the [group kernel](../../../../kernel-of-a-group-homomorphism.md) is a [normal subgroup](../../../../normal-subgroup.md)**.

Let $S_2=\{e,\tau\}$ with $\tau=(12)$. The [parity of a permutation](../../../../parity-of-a-permutation.md) defines the desired map from $S_3$:

$$
\boxed{h(e)=h((123))=h((132))=e,\qquad h((12))=h((13))=h((23))=\tau.}
$$

The [sign of a permutation](../../../../sign-of-a-permutation.md) is multiplicative, so parity adds modulo two under composition, exactly matching $\tau^2=e$. Thus this is a [group homomorphism](../../../../group-homomorphism.md); it is surjective because a transposition maps to $\tau$. Its [group kernel](../../../../kernel-of-a-group-homomorphism.md) is

$$
\boxed{K=A_3=\{e,(123),(132)\}.}
$$

This is the [alternating group](../../../../alternating-group.md) on three objects, a [normal subgroup](../../../../normal-subgroup.md) of index two in $S_3$.

## ↑ Ancestors (12)

1. [9](../9.md)
2. [Paper 2](../../paper-2-split.md)
3. [2003](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
