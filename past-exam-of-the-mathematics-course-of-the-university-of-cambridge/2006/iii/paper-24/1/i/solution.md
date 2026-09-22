<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

We use the [general adjoint functor theorem](../../../../../../freyd-general-adjoint-functor-theorem.md) in its solution-set form. Let $G:\mathcal D\to\mathcal C$ be a [functor](../../../../../../functor.md) between [locally small categories](../../../../../../locally-small-category.md), with $\mathcal D$ a [complete category](../../../../../../complete-category.md). Then $G$ has a [left adjoint](../../../../../../adjoint-functors.md) exactly when it preserves all small [categorical limits](../../../../../../categorical-limit.md) and, for each $C\in\mathcal C$, there is a set-indexed family

$$
u_i:C\to GD_i\qquad(i\in I_C)
$$

such that every $u:C\to GD$ factors as $Gf\,u_i$ for some $i$ and some $f:D_i\to D$. This is the [solution-set condition](../../../../../../solution-set-condition.md). The indexing family is a set, whereas the entire [comma category](../../../../../../comma-category.md) $(C\downarrow G)$ can be large.

We first prove the [initial-object lemma for complete categories with a weakly initial set](../../../../../../initial-object-lemma-for-complete-categories-with-a-weakly-initial-set.md). Let $\mathcal E$ be locally small and complete, with a [weakly initial set](../../../../../../weakly-initial-set.md) $(E_i)_{i\in I}$. Its [product in a category](../../../../../../product-category-theory.md) $W=\prod_iE_i$ is weakly initial: follow a projection by a map from the corresponding $E_i$ to any desired object. The [hom-set](../../../../../../hom-set.md) $\mathcal E(W,W)$ is a set, so we can form the simultaneous [equalizer](../../../../../../equaliser.md)

$$
e:E\longrightarrow W,\qquad he=e\quad\text{for every }h:W\to W.
$$

This is a small limit; equivalently, equalize the family of endomorphisms with the family of identity maps into a product of copies of $W$. Every object receives a map from $E$, since it receives one from $W$.

To prove uniqueness, let $a,b:E\rightrightarrows B$, and take their equalizer $j:V\to E$. Weak initiality of $W$ gives $t:W\to V$. Since $ejt$ is an endomorphism of $W$, the defining property of $e$ gives

$$
ejte=e.
$$

The [monomorphism](../../../../../../monomorphism.md) $e$ cancels, yielding $jte=1_E$. Thus $j$ is both a monomorphism and a [split epimorphism](../../../../../../split-epimorphism.md), hence an [isomorphism](../../../../../../isomorphism.md). Its equalizer property now implies $a=b$. Therefore **$E$ is initial**.

Fix $C$. Small [categorical limits](../../../../../../categorical-limit.md) in $(C\downarrow G)$ are obtained from the limits in $\mathcal D$: preservation by $G$ supplies the unique map from $C$ to the image of the limiting object. The [comma category](../../../../../../comma-category.md) is locally small, and the solution family is a [weakly initial set](../../../../../../weakly-initial-set.md) in it. The lemma supplies an [initial object](../../../../../../initial-object.md) $(LC,\eta_C:C\to GLC)$.

For $k:C\to C'$, initiality gives a unique arrow $Lk:LC\to LC'$ satisfying $G(Lk)\eta_C=\eta_{C'}k$. Uniqueness proves preservation of identities and composition, so $L$ is a [functor](../../../../../../functor.md). Initiality also gives [natural bijections](../../../../../../natural-bijection.md)

$$
\boxed{\mathcal D(LC,D)\cong\mathcal C(C,GD),\qquad f\longmapsto Gf\,\eta_C,}
$$

which prove $L\dashv G$.

Conversely, if $L\dashv G$, the singleton $\eta_C:C\to GLC$ is a solution set by the [adjunction](../../../../../../adjoint-functors.md) bijection. To see that $G$ preserves a small limit $D=\lim_jD_j$, use the adjunction and the limit property to obtain, naturally in $C$,

$$
\mathcal C(C,GD)\cong\mathcal D(LC,D)\cong\lim_j\mathcal D(LC,D_j)\cong\lim_j\mathcal C(C,GD_j).
$$

This is precisely the [universal property](../../../../../../universal-property.md) of the image limit cone. It proves the necessity of both hypotheses.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
