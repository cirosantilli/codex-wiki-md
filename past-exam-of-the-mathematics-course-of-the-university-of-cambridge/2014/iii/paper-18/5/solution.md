<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For $A\in\mathcal C$, the [comma category](../../../../../comma-category.md) $(A\downarrow G)$ has objects $(D,u)$ with $D\in\mathcal D$ and $u:A\to GD$. A morphism $(D,u)\to(D',u')$ is $h:D\to D'$ satisfying $Gh\,u=u'$. Identities and composition are those of $\mathcal D$, and functoriality of $G$ verifies the condition under composition.

The [Freyd general adjoint functor theorem](../../../../../freyd-general-adjoint-functor-theorem.md) states: if $\mathcal D$ is a [locally small category](../../../../../locally-small-category.md) with all small [categorical limits](../../../../../categorical-limit.md), and $\mathcal C$ is locally small, then $G:\mathcal D\to\mathcal C$ has a [left adjoint](../../../../../adjoint-functors.md) if and only if it preserves small limits and satisfies the [solution-set condition](../../../../../solution-set-condition.md). The latter means that for each $A$ there is a set-indexed family $u_i:A\to GD_i$ such that every $u:A\to GD$ equals $Gh\,u_i$ for some $i$ and some $h:D_i\to D$.

For necessity, use the standard result that a [right adjoint](../../../../../adjoint-functors.md) preserves [categorical limits](../../../../../categorical-limit.md). If $F\dashv G$, the singleton family containing the [unit of an adjunction](../../../../../unit-of-an-adjunction.md) $\eta_A:A\to GFA$ is a solution set, since transposition gives $u=Gh\,\eta_A$ for a unique $h:FA\to D$.

For sufficiency, use the following standard limit fact: if $\mathcal D$ is complete and $G$ preserves limits, the projection $(A\downarrow G)\to\mathcal D$ creates small limits. Indeed, a compatible family $A\to GD_j$ induces a unique arrow into $G(\lim D_j)$, and this makes the underlying limit a limit in the comma category. The [comma category](../../../../../comma-category.md) is locally small because each of its hom-sets is a subset of a hom-set of $\mathcal D$. Its solution family is a [weakly initial set](../../../../../weakly-initial-set.md).

We prove the remaining [initial-object lemma for complete categories with a weakly initial set](../../../../../initial-object-lemma-for-complete-categories-with-a-weakly-initial-set.md). In any [locally small category](../../../../../locally-small-category.md) $\mathcal K$ with all small limits and a weakly initial set $(K_i)$, form $W=\prod_iK_i$. It is weakly initial: for any $X$, some $K_i\to X$ exists and may be composed with the projection $W\to K_i$. The empty family cannot be weakly initial in a nonempty complete category, which has a terminal object.

The set $\operatorname{End}(W)$ is small. Form a simultaneous [equalizer](../../../../../equaliser.md) $e:E\to W$ of every endomorphism of $W$ and $1_W$; thus

$$
u e=e\quad\text{for every }u:W\to W.
$$

This equalizer exists by completeness, for example as the equalizer of two maps $W\rightrightarrows W^{\operatorname{End}(W)}$. The object $E$ is still weakly initial, since it maps to $W$.

Given $a,b:E\to X$, take their [equalizer](../../../../../equaliser.md) $j:Y\to E$. Weak initiality of $W$ gives $t:W\to Y$. Since $ejt$ is an endomorphism of $W$, we have $ejte=e$, and cancellation of the [monomorphism](../../../../../monomorphism.md) $e$ gives $jte=1_E$. Thus $j$ is a [split epimorphism](../../../../../split-epimorphism.md) as well as a [monomorphism](../../../../../monomorphism.md), so it is an [isomorphism](../../../../../isomorphism.md). From $aj=bj$ follows $a=b$. There is at least one map $E\to X$ by weak initiality, so **$E$ is initial**.

Apply this lemma to every $(A\downarrow G)$ and choose its [initial object](../../../../../initial-object.md) $(FA,\eta_A)$. For $v:A\to A'$, initiality gives the unique $Fv:FA\to FA'$ satisfying $GFv\,\eta_A=\eta_{A'}v$. Uniqueness proves the functor laws. The same initiality gives natural [bijections](../../../../../bijection.md)

$$
\mathcal D(FA,D)\cong\mathcal C(A,GD),\qquad h\longmapsto Gh\,\eta_A.
$$

Hence **$F\dashv G$**, completing the theorem without invoking another adjoint functor theorem.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 18](../../paper-18-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
