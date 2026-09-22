<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

In a small [regular category](../../../../../regular-category.md) $\mathcal C$, the [regular coverage](../../../../../regular-coverage.md) has one-arrow covers: each [regular epimorphism](../../../../../regular-epimorphism.md) $\alpha:B\twoheadrightarrow A$ is a covering family by itself. Identity maps, composites and [pullbacks](../../../../../pullback-category-theory.md) of such arrows are again covers, so this is a basis for a [Grothendieck topology](../../../../../grothendieck-topology.md). A presheaf is a sheaf precisely when every compatible section over a covering arrow descends uniquely along that arrow.

It is [subcanonical](../../../../../subcanonical-topology.md). A section of the [representable presheaf](../../../../../representable-functor.md) $yX=\mathcal C(-,X)$ over $B$ is a map $g:B\to X$. Its matching condition is $g\pi_1=g\pi_2$ on the [kernel pair](../../../../../kernel-pair.md) $B\times_A B$. Since a [regular epimorphism](../../../../../regular-epimorphism.md) is the [coequalizer](../../../../../coequalizer.md) of its kernel pair, there is a unique $\bar g:A\to X$ with $\bar g\alpha=g$. This is exactly the sheaf condition for $yX$.

For a subfunctor $F'\subseteq F$ of a regular-coverage sheaf, define local membership by

$$
F''(A)=\{x\in F(A):F(\alpha)x\in F'(B)\text{ for some regular epi }\alpha:B\to A\}.
$$

This is a subfunctor. If $t:C\to A$ and $\alpha$ witnesses membership, pull back $\alpha$ along $t$; the resulting cover of $C$ witnesses membership of $F(t)x$, because $F'$ is stable under restriction.

It is a sheaf as well. Let $\beta:B\twoheadrightarrow A$ cover and let $y\in F''(B)$ satisfy the kernel-pair matching condition. The sheaf $F$ gives a unique $x\in F(A)$ with $F(\beta)x=y$. Choose a cover $\alpha:C\twoheadrightarrow B$ with $F(\alpha)y\in F'(C)$. The composite $\beta\alpha$ is a cover of $A$ and witnesses $x\in F''(A)$. Uniqueness comes from $F$. Thus the inclusion $F''\hookrightarrow F$ is a mono between sheaves and is closed for the associated [local operator](../../../../../lawvere-tierney-topology.md).

Moreover, any closed [subobject](../../../../../subobject.md) $S\subseteq F$ containing $F'$ is itself a sheaf. If $x\in F''(A)$, its restriction along a witnessing cover lies in $S(B)$, and the sheaf condition for $S$ descends it to a section in $S(A)$. Its image in $F(A)$ is $x$ by uniqueness. Hence $F''$ is the least closed [subobject](../../../../../subobject.md) containing $F'$, and

$$
\boxed{\overline{F'}=F''.}
$$

This proves the [local membership closure for the regular coverage](../../../../../local-membership-closure-for-the-regular-coverage.md), with a single [regular epimorphism](../../../../../regular-epimorphism.md) as witness.

Suppose $yA$ is the union, in the sheaf [topos](../../../../../elementary-topos.md), of a family of subsheaves $F_i$. The union in presheaves is the pointwise union $F'=\bigcup_iF_i$; its closure is the union in sheaves. Thus $1_A\in F''(A)$. A witnessing cover $\alpha:B\twoheadrightarrow A$ belongs to $F_i(B)$ for one index $i$. The two restrictions of $\alpha$ to its kernel pair agree. Since $F_i$ is a subsheaf, this matching section descends in $F_i$ to $1_A\in F_i(A)$. Every map $t:C\to A$ is the restriction of $1_A$ along $t$, so $F_i=yA$. Therefore **every representable sheaf is irreducible**, even with respect to arbitrary unions. There are no empty covering families in this coverage, and $1_A$ also shows that the representable cannot be initial.

Finally, in the [regular syntactic category](../../../../../regular-syntactic-category.md) of a [regular theory](../../../../../regular-theory.md), the context formula $\phi$ defines an object $A$. Each formula $\phi\wedge\psi_i$ defines a mono $A_i\hookrightarrow A$, and the associated representable subsheaf is its interpretation inside $yA$ in the generic model. A derivation of the coherent disjunction says that these finitely many subsheaves have union $yA$. Irreducibility gives $yA_i=yA$ for some $i$. The [Yoneda embedding](../../../../../yoneda-embedding.md) is full and faithful, since the coverage is subcanonical, and therefore reflects this isomorphism. Hence $A_i\hookrightarrow A$ is invertible in the syntactic category: $\phi$ entails $\psi_i$. Thus

$$
\boxed{\mathbb T\vdash\phi\Rightarrow\bigvee_{i=1}^{n}\psi_i
\quad\Longrightarrow\quad
\mathbb T\vdash\phi\Rightarrow\psi_i\text{ for some }i.}
$$

The disjunction is an outer coherent conclusion; the theory and all constituent formulas are regular. This [disjunction property of regular theories](../../../../../disjunction-property-of-regular-theories.md) follows from single-arrow descent, rather than from ordinary first-order compactness.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 74](../../paper-74-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
