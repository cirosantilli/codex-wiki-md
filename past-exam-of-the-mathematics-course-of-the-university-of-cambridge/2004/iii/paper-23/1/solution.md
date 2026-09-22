<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the [Freyd general adjoint functor theorem](../../../../../freyd-general-adjoint-functor-theorem.md): a [functor](../../../../../functor.md) $U:\mathcal A\to\mathcal B$, with $\mathcal A$ [complete](../../../../../completeness.md) and both categories [locally small](../../../../../locally-small-category.md), has a [left adjoint](../../../../../adjoint-functors.md) precisely when it preserves small [categorical limits](../../../../../categorical-limit.md) and satisfies the [solution-set condition](../../../../../solution-set-condition.md). The latter means that every [comma category](../../../../../comma-category.md) $(b\downarrow U)$ has a small [weakly initial set](../../../../../weakly-initial-set.md).

Here is the proof. First prove the [initial-object lemma for complete categories with a weakly initial set](../../../../../initial-object-lemma-for-complete-categories-with-a-weakly-initial-set.md). In a complete locally small [category](../../../../../category-split.md) $\mathcal E$, take the [product in a category](../../../../../product-category-theory.md) $W$ of a small weakly initial family. It is weakly initial: project to whichever member admits a [morphism](../../../../../morphism.md) into the required object. Form the simultaneous [equalizer](../../../../../equaliser.md) $i:I\to W$ of every [endomorphism](../../../../../endomorphism.md) of $W$ and $1_W$; local smallness makes this a small limit.

For parallel $f,g:I\to X$, let $j:Y\to I$ be their [equalizer](../../../../../equaliser.md). Weak initiality supplies $t:W\to Y$. Since $ijt$ is an endomorphism of $W$, the defining equalities give $ijti=i$. Cancel the [monomorphism](../../../../../monomorphism.md) $i$ to get $jti=1_I$. Thus $j$ is a split epimorphism as well as a monomorphism, hence invertible, and $f=g$. Existence of a [morphism](../../../../../morphism.md) $I\to X$ follows by composing $i$ with a map $W\to X$. Therefore $I$ is an [initial object](../../../../../initial-object.md).

Now, if $U$ preserves small [categorical limits](../../../../../categorical-limit.md), each $(b\downarrow U)$ has them: take the limit of the underlying $\mathcal A$-diagram and use preservation to assemble its maps out of $b$. It is locally small and has a weakly initial solution set, so the lemma produces an [initial object](../../../../../initial-object.md) $(Lb,\eta_b)$. Its [universal property](../../../../../universal-property.md) gives natural [bijections](../../../../../bijection.md)

$$
\mathcal A(Lb,a)\cong\mathcal B(b,Ua).
$$

The universal arrows define $L$ on [morphisms](../../../../../morphism.md), proving $L\dashv U$. Conversely, a [right adjoint](../../../../../adjoint-functors.md) preserves [categorical limits](../../../../../categorical-limit.md), and its unit supplies a singleton solution set in each comma category.

Apply this to $U=F^*$. The [functor category](../../../../../functor-category.md) $[\mathcal D,\mathbf{Set}]$ is complete and locally small because $\mathcal D$ is small; [pointwise limits in a functor category](../../../../../pointwise-limits-in-a-functor-category.md) show $F^*$ preserves all small limits. For $Q:\mathcal C\to\mathbf{Set}$, verify the [bounded subfunctor solution set for precomposition](../../../../../bounded-subfunctor-solution-set-for-precomposition.md). Choose an infinite [cardinal number](../../../../../cardinal-number.md) $\kappa$ at least as large as the number of $\mathcal D$-[morphisms](../../../../../morphism.md) and $\sum_{c\in\mathcal C}|Q(c)|$. Given $\eta:Q\to GF$, set

$$
G'(d)=\{G(u)\eta_c(x):c\in\mathcal C,\ x\in Q(c),\ u:Fc\to d\}.
$$

Postcomposition makes $G'$ a subfunctor, each value has cardinality at most $\kappa$, and $\eta$ factors through $G'F$. After labelling its values by subsets of $\kappa$, only a set of possibilities for $G'$ and $Q\to G'F$ exists. Their maps into $G$ give the required weakly initial set. Thus **$F^*$ has a left adjoint**.

It is the [left Kan extension](../../../../../left-kan-extension.md). The [left Kan extension as a comma-category colimit](../../../../../left-kan-extension-as-a-comma-category-colimit.md) makes it concrete:

$$
\boxed{(\operatorname{Lan}_FQ)(d)=\operatorname{colim}_{(c,u:Fc\to d)\in(F\downarrow d)}Q(c).}
$$

Every representative $(c,u,x)$ maps under $\eta:Q\to GF$ to $G(u)\eta_c(x)$. The colimit identifications and naturality make this well-defined, giving exactly $\operatorname{Nat}(\operatorname{Lan}_FQ,G)\cong\operatorname{Nat}(Q,GF)$.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [Section A](../section-a.md)
3. [Paper 23](../../paper-23-split.md)
4. [Iii](../../split.md)
5. [2004](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
