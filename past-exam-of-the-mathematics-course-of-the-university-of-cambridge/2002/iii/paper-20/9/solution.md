<h1 id="9/solution">Solution</h1>

↑ **Parent:** [9](../9.md)

For the general alternative, let $G:\mathcal D\to\mathcal C$ be a [functor](../../../../../functor.md) between [locally small categories](../../../../../locally-small-category.md), with $\mathcal D$ a [complete category](../../../../../complete-category.md). The [Freyd general adjoint functor theorem](../../../../../freyd-general-adjoint-functor-theorem.md) says that $G$ has a [left adjoint](../../../../../adjoint-functors.md) if and only if it preserves small [categorical limits](../../../../../categorical-limit.md) and satisfies the [solution-set condition](../../../../../solution-set-condition.md). Explicitly, for every $c\in\mathcal C$, there must be a [set](../../../../../set-split.md) of [morphisms](../../../../../morphism.md) $x_j:c\to Gd_j$ such that every $x:c\to Gd$ has the form $G(h)x_j$ for some $j$ and $h:d_j\to d$. Equivalently, each [comma category](../../../../../comma-category.md) $(c\downarrow G)$ has a [weakly initial set](../../../../../weakly-initial-set.md).

We prove the [initial-object lemma for complete categories with a weakly initial set](../../../../../initial-object-lemma-for-complete-categories-with-a-weakly-initial-set.md). Let $\mathcal E$ be a [locally small category](../../../../../locally-small-category.md) which is complete and has a [weakly initial set](../../../../../weakly-initial-set.md) $(w_j)_{j\in J}$. Its [product in a category](../../../../../product-category-theory.md) $p=\prod_jw_j$ is weakly initial: for each $z$, choose a [morphism](../../../../../morphism.md) $w_j\to z$ and compose with the projection $p\to w_j$. The [hom-set](../../../../../hom-set.md) $\mathcal E(p,p)$ is a [set](../../../../../set-split.md). Form $e:i\to p$ equalizing every [endomorphism](../../../../../endomorphism.md) of $p$ with $1_p$, by taking the [equalizer](../../../../../equaliser.md) of the two [morphisms](../../../../../morphism.md)

$$
p\rightrightarrows\prod_{v\in\mathcal E(p,p)}p,
$$

whose $v$-coordinates are $v$ and $1_p$. Then $ve=e$ for every [endomorphism](../../../../../endomorphism.md) $v$, and $e$ is monic. There is a [morphism](../../../../../morphism.md) $i\to z$ for every $z$, by composing $e$ with a weakly initial [morphism](../../../../../morphism.md) out of $p$.

To prove uniqueness, let $u,v:i\rightrightarrows z$ and take their [equalizer](../../../../../equaliser.md) $q:w\to i$. Weak initiality of $p$ gives $a:p\to w$. The composite $eqa:p\to p$ is an [endomorphism](../../../../../endomorphism.md), so $eqa e=e$. Cancel the [monomorphism](../../../../../monomorphism.md) $e$ to obtain $qa e=1_i$. Thus $q$ is both monic and split epic, hence an [isomorphism](../../../../../isomorphism.md): if $qk=1$, cancellation from $qkq=q$ gives $kq=1$. Since $uq=vq$, it follows that $u=v$. Therefore $i$ is an [initial object](../../../../../initial-object.md), proving the lemma fully.

Now assume [categorical limit](../../../../../categorical-limit.md) preservation and the [solution-set condition](../../../../../solution-set-condition.md). The [comma category](../../../../../comma-category.md) $(c\downarrow G)$ is locally small. It is complete: for a small [diagram in a category](../../../../../diagram-category-theory.md) $(d_j,x_j)$, take its underlying [categorical limit](../../../../../categorical-limit.md) $l$ in $\mathcal D$. Since $G$ preserves this [categorical limit](../../../../../categorical-limit.md), the compatible $x_j:c\to Gd_j$ give a unique $x:c\to Gl$. The same [universal property](../../../../../universal-property.md) shows that $(l,x)$ is the [categorical limit](../../../../../categorical-limit.md) in the [comma category](../../../../../comma-category.md). Its [weakly initial set](../../../../../weakly-initial-set.md) and the proved lemma therefore supply an [initial object](../../../../../initial-object.md) $(Fc,\eta_c)$. For $t:c\to c'$, its [universal property](../../../../../universal-property.md) defines a unique $Ft:Fc\to Fc'$ with $G(Ft)\eta_c=\eta_{c'}t$. Uniqueness proves the [identity morphism](../../../../../identity-morphism.md) and [composition in a category](../../../../../composition-in-a-category.md) laws and the [naturality](../../../../../naturality.md) of $\eta$. The same [universal property](../../../../../universal-property.md) gives the [natural bijection](../../../../../natural-bijection.md) $\mathcal D(Fc,d)\cong\mathcal C(c,Gd)$, so $F\dashv G$.

For necessity, an [adjunction](../../../../../adjoint-functors.md) $F\dashv G$ supplies the singleton [weakly initial set](../../../../../weakly-initial-set.md) $(Fc,\eta_c)$ at $c$. It also proves that $G$ preserves [categorical limits](../../../../../categorical-limit.md): maps $c\to Gd$ correspond to maps $Fc\to d$, and compatible families of the latter factor uniquely through any [categorical limit](../../../../../categorical-limit.md) in $\mathcal D$. Hence the image [categorical cone](../../../../../cone-over-a-diagram.md) under $G$ has the required [universal property](../../../../../universal-property.md). This proves both directions of the general alternative.

For the special alternative, the [limit form of the special adjoint functor theorem](../../../../../limit-form-of-the-special-adjoint-functor-theorem.md) says: if $\mathcal D$ is complete, locally small and [well-powered](../../../../../well-powered-category.md), with a [small cogenerating family](../../../../../cogenerating-set.md) $(Q_i)_{i\in I}$, and $\mathcal C$ is locally small, then $G:\mathcal D\to\mathcal C$ has a [left adjoint](../../../../../adjoint-functors.md) exactly when it preserves small [categorical limits](../../../../../categorical-limit.md). A [cogenerating set](../../../../../cogenerating-set.md) means that unequal parallel [morphisms](../../../../../morphism.md) $u,v:X\rightrightarrows Y$ are distinguished by some [morphism](../../../../../morphism.md) $Y\to Q_i$. We prove the needed [solution-set condition](../../../../../solution-set-condition.md), so that the general theorem applies.

Fix $x:c\to Gd$. A supporting [subobject](../../../../../subobject.md) of $d$ is a [monomorphism](../../../../../monomorphism.md) $m:d'\to d$ through whose image under $G$ the [morphism](../../../../../morphism.md) $x$ factors. There is at least one, namely $1_d$. Because $\mathcal D$ is [well-powered](../../../../../well-powered-category.md), choose a [set](../../../../../set-split.md) of representatives of all these supporting [subobjects](../../../../../subobject.md). A limit-preserving [functor](../../../../../functor.md) preserves [monomorphisms](../../../../../monomorphism.md): a map is monic exactly when its diagonal into its self-[pullback in a category](../../../../../pullback-category-theory.md) is an [isomorphism](../../../../../isomorphism.md), and both the [pullback in a category](../../../../../pullback-category-theory.md) and this [isomorphism](../../../../../isomorphism.md) are preserved. Consequently each factorization of $x$ through $Gm$ is unique. Form the [intersection of subobjects](../../../../../intersection-of-subobjects.md) of the supporting representatives, as a wide [pullback in a category](../../../../../pullback-category-theory.md) over $d$. The unique lifts of $x$ are compatible and, since $G$ preserves that [categorical limit](../../../../../categorical-limit.md), they give a factorization

$$
x=G(m_0)x_0,\qquad m_0:d_0\hookrightarrow d,\quad x_0:c\to Gd_0.
$$

This is a [minimal supported subobject](../../../../../minimal-supported-subobject.md). More explicitly, if $q:e\hookrightarrow d_0$ also supports $x_0$, then $m_0q$ is one of the supporting [subobjects](../../../../../subobject.md) of $d$. The intersection therefore factors through $m_0q$, giving $r:d_0\to e$ with $m_0qr=m_0$. Monicity of $m_0$ gives $qr=1_{d_0}$; monicity of $q$ then makes $q$ invertible.

For any $u,v:d_0\to Q_i$, if $G(u)x_0=G(v)x_0$, the [equalizer](../../../../../equaliser.md) of $u,v$ supports $x_0$, because $G$ preserves that [equalizer](../../../../../equaliser.md). Minimality makes it invertible, so $u=v$. We have therefore obtained [injective functions](../../../../../injective-function.md)

$$
\mathcal D(d_0,Q_i)\longrightarrow\mathcal C(c,GQ_i),\qquad u\longmapsto G(u)x_0.
$$

Let $S_i$ be the realized image [subset](../../../../../subset.md) of the fixed [set](../../../../../set-split.md) $\mathcal C(c,GQ_i)$. Use the unique [morphism](../../../../../morphism.md) corresponding to each $s\in S_i$ to form the [evaluation embedding into cogenerator products](../../../../../evaluation-embedding-into-cogenerator-products.md)

$$
d_0\longrightarrow P_S=\prod_{i\in I}\prod_{s\in S_i}Q_i.
$$

This [morphism](../../../../../morphism.md) is monic: if two [morphisms](../../../../../morphism.md) into $d_0$ have identical product composites, every [morphism](../../../../../morphism.md) from $d_0$ to every $Q_i$ gives identical composites, and the cogenerating property makes the two [morphisms](../../../../../morphism.md) equal. There is only a [set](../../../../../set-split.md) of possible families of [subsets](../../../../../subset.md) $(S_i)$, and hence a [set](../../../../../set-split.md) of possible products $P_S$. Each has only a [set](../../../../../set-split.md) of [subobjects](../../../../../subobject.md) by well-poweredness, and each chosen [subobject](../../../../../subobject.md) $a$ has only a [set](../../../../../set-split.md) of [morphisms](../../../../../morphism.md) $c\to Ga$ by local smallness. Take all these pairs $(a,z:c\to Ga)$ as a [weakly initial set](../../../../../weakly-initial-set.md). Every original $(d,x)$ receives a [morphism](../../../../../morphism.md) from a pair representing its $(d_0,x_0)$, through $m_0$. Thus the [set](../../../../../set-split.md) is weakly initial in $(c\downarrow G)$.

The general theorem now supplies a [left adjoint](../../../../../adjoint-functors.md). Necessity again follows from preservation of [categorical limits](../../../../../categorical-limit.md) by a [right adjoint](../../../../../adjoint-functors.md). This proves the special alternative, including its size argument. Using only the realized [subsets](../../../../../subset.md) $S_i$ avoids assuming that an arbitrary object admits a [morphism](../../../../../morphism.md) into every cogenerator. **Both adjoint [functor](../../../../../functor.md) theorem alternatives are proved.**

## ↑ Ancestors (10)

1. [9](../9.md)
2. [Paper 20](../../paper-20-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
