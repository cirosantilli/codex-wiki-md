<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Present the [Grothendieck topos](../../../../../grothendieck-topos.md) as $\mathcal E=\mathbf{Sh}(\mathcal C,J)$ for a small [site](../../../../../site-category-theory.md). Let $a:\widehat{\mathcal C}\to\mathcal E$ be [sheafification](../../../../../sheafification.md) and $i$ the inclusion. The standard [sheafification](../../../../../sheafification.md) construction supplies $a\dashv i$, with $a$ preserving [finite limits](../../../../../finite-limit.md). Concretely, matching-family constructions commute with [finite limits](../../../../../finite-limit.md), and their directed refinement over covering sieves does so as well. Limits of sheaves are computed in the [presheaf category](../../../../../presheaf-category.md), so $\mathcal E$ has [finite limits](../../../../../finite-limit.md); its [colimits](../../../../../colimit.md) are sheafifications of presheaf [colimits](../../../../../colimit.md).

For sheaves $A,B$, form the presheaf exponential

$$
E(c)=\operatorname{Nat}(y c\times A,B).
$$

It is a sheaf. Indeed, for a covering sieve $S\hookrightarrow y c$, one has $aS\cong a(y c)$. Exponential [adjunction](../../../../../adjoint-functors.md), [sheafification](../../../../../sheafification.md) [adjunction](../../../../../adjoint-functors.md) and left exactness give

$$
\operatorname{Nat}(S,E)
\cong\operatorname{Nat}(S\times A,B)
\cong\operatorname{Hom}_{\mathcal E}(aS\times A,B)
\cong\operatorname{Hom}_{\mathcal E}(a(y c)\times A,B)
\cong\operatorname{Nat}(y c,E).
$$

These are the restriction comparisons, proving the sheaf condition. Restricting the presheaf exponential [adjunction](../../../../../adjoint-functors.md) to sheaves now makes $E=B^A$ in $\mathcal E$.

The [subobject classifier](../../../../../subobject-classifier.md) is the sheaf $\Omega_J$ of [J-closed sieves](../../../../../j-closed-sieve.md). A sieve $S$ on $c$ is J-closed when, for every $f:d\to c$, $f^*S\in J(d)$ implies $f\in S$. Pullback of sieves defines its restrictions, and the maximal sieve defines truth. Local sieve data glue by taking the J-closure of their compatible generated sieve; uniqueness follows because membership in a J-closed sieve is local. This proves that $\Omega_J$ is a sheaf.

For a subsheaf $A\hookrightarrow B$, the characteristic morphism sends $b\in B(c)$ to

$$
\chi_A(b)=\{f:d\to c:B(f)(b)\in A(d)\}.
$$

This sieve is J-closed because local membership in a subsheaf descends by its gluing axiom. Pulling truth back recovers exactly $A$. Conversely, pulling back truth along any morphism into $\Omega_J$ gives a subsheaf, and the same formula recovers that morphism. **[Finite limits](../../../../../finite-limit.md), exponentials and this classifier make every [Grothendieck topos](../../../../../grothendieck-topos.md) an [elementary topos](../../../../../elementary-topos.md).**

Here are the explicit [Heyting operations on subsheaves](../../../../../heyting-operations-on-subsheaves.md) of an object $B$. Intersections give meets:

$$
(A\wedge D)(c)=A(c)\cap D(c),\qquad
\left(\bigwedge_i A_i\right)(c)=\bigcap_i A_i(c).
$$

The top is $B$. Arbitrary joins are local unions:

$$
\boxed{
b\in\left(\bigvee_iA_i\right)(c)
\ \Longleftrightarrow\
\{f:d\to c:B(f)b\in A_i(d)\text{ for some }i\}\in J(c).}
$$

Equivalently, $b$ locally lies in one of the $A_i$, with the index allowed to vary across the covering arrows. This is the J-closure of the pointwise union, or its [sheafification](../../../../../sheafification.md). It is the smallest subsheaf containing every $A_i$, since any such subsheaf must contain sections locally in it.

The bottom is the empty join, namely the initial [subobject](../../../../../subobject.md). Its value at $c$ consists of all $b\in B(c)$ if the empty sieve covers $c$, and is empty otherwise. This detail matters on [sites](../../../../../site-category-theory.md) with empty covers; it is not safe to use an always-empty presheaf as the initial sheaf.

Implication is described without any pointwise-complement assumption:

$$
\boxed{
(A\Rightarrow D)(c)=
\{b\in B(c):
\text{ for every }f:d\to c,\ B(f)b\in A(d)\Longrightarrow B(f)b\in D(d)\}.}
$$

Restrictions preserve this condition. It is also local: pull a covering sieve back along an arbitrary $f$, use membership in $A$ on those restrictions, then descend their membership in $D$. Thus it is a subsheaf. It satisfies the defining [Heyting algebra](../../../../../heyting-algebra.md) [adjunction](../../../../../adjoint-functors.md)

$$
C\leq(A\Rightarrow D)\quad\Longleftrightarrow\quad C\cap A\leq D.
$$

For the forward direction take the identity restriction. For the reverse direction every restriction of a section of $C$ remains in $C$, so membership in $A$ forces membership in $D$. Negation is $\neg A=A\Rightarrow0$. These formulas give the complete Heyting algebra structure on $\operatorname{Sub}_{\mathcal E}(B)$; in general negation is a pseudocomplement rather than a set-theoretic complement.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 23](../../paper-23-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
