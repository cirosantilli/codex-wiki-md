<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

The [Freyd general adjoint functor theorem](../../../../../freyd-general-adjoint-functor-theorem.md) is as follows. Let $G:\mathcal D\to\mathcal C$, with $\mathcal D$ a [complete category](../../../../../complete-category.md) which is [locally small](../../../../../locally-small-category.md). Then $G$ has a [left adjoint](../../../../../adjoint-functors.md) if and only if it preserves all small [categorical limits](../../../../../categorical-limit.md) and satisfies the [solution-set condition](../../../../../solution-set-condition.md): for each $c\in\mathcal C$, there is a set-indexed family

$$
u_i:c\to Gd_i
$$

such that every $u:c\to Gd$ can be written $u=G(h)u_i$ for some $i$ and some $h:d_i\to d$. The target [category](../../../../../category-split.md) need not be complete. We prove all the existence steps.

First establish the [initial-object lemma for complete categories with a weakly initial set](../../../../../initial-object-lemma-for-complete-categories-with-a-weakly-initial-set.md). Let $\mathcal E$ be [locally small](../../../../../locally-small-category.md) and complete, with a [weakly initial set](../../../../../weakly-initial-set.md) $\{w_i\}$, meaning every object receives a map from at least one $w_i$. Its [categorical product](../../../../../product-category-theory.md) $w=\prod_iw_i$ is weakly initial: compose a [categorical product](../../../../../product-category-theory.md) projection with the map from the appropriate $w_i$. Local smallness makes $\mathcal E(w,w)$ a [set](../../../../../set-split.md). Let $e:v\to w$ be the simultaneous [equaliser](../../../../../equaliser.md) of every [endomorphism](../../../../../endomorphism.md) of $w$ and the identity. Explicitly it is the [equaliser](../../../../../equaliser.md) of the two arrows

$$
w\rightrightarrows\prod_{k\in\mathcal E(w,w)}w
$$

with components $k$ and $1_w$. Thus $ke=e$ for every [endomorphism](../../../../../endomorphism.md) $k$, and $e$ is monic.

Every object $x$ receives a [morphism](../../../../../morphism.md) from $v$, by composing $e$ with a map $w\to x$. To prove uniqueness, take parallel maps $a,b:v\to x$ and their [equaliser](../../../../../equaliser.md) $m:y\to v$. Weak initiality of $w$ gives $t:w\to y$. The composite $emt$ is an [endomorphism](../../../../../endomorphism.md) of $w$, so $(emt)e=e$. Cancelling the [monomorphism](../../../../../monomorphism.md) $e$ gives $mte=1_v$. Hence $m$ is both monic and a [split epimorphism](../../../../../split-epimorphism.md), and is therefore invertible. Since $am=bm$, this forces $a=b$. We have proved $v$ is initial, without using a class-sized [categorical product](../../../../../product-category-theory.md) or [equaliser](../../../../../equaliser.md).

For sufficiency in the theorem, fix $c$ and consider the [comma category](../../../../../comma-category.md) $(c\downarrow G)$. Its objects are pairs $(d,u:c\to Gd)$; a [morphism](../../../../../morphism.md) $h:(d,u)\to(d',u')$ satisfies $G(h)u=u'$. This [category](../../../../../category-split.md) is [locally small](../../../../../locally-small-category.md) because each [hom-set](../../../../../hom-set.md) is a subset of $\mathcal D(d,d')$. It is complete: for a small diagram of such pairs, take the underlying [categorical limit](../../../../../categorical-limit.md) $d$ in $\mathcal D$. The arrows from $c$ form a cone to its image under $G$, and preservation of the [categorical limit](../../../../../categorical-limit.md) gives a unique $u:c\to Gd$ inducing them. The same [universal property](../../../../../universal-property.md) gives all mediators in the [comma category](../../../../../comma-category.md). The solution-set family is a [weakly initial set](../../../../../weakly-initial-set.md) in this [comma category](../../../../../comma-category.md), so the lemma supplies an initial pair

$$
(Fc,\eta_c:c\to GFc).
$$

For $f:c\to c'$, initiality defines a unique $Ff:Fc\to Fc'$ satisfying $G(Ff)\eta_c=\eta_{c'}f$. Uniqueness proves the identity and composition laws, making $F$ a [functor](../../../../../functor.md). Initiality also gives [bijections](../../../../../bijection.md)

$$
\boxed{\mathcal D(Fc,d)\cong\mathcal C(c,Gd),\qquad h\longmapsto G(h)\eta_c.}
$$

The definition of $Ff$ proves [naturality](../../../../../naturality.md) in $c$, and postcomposition proves [naturality](../../../../../naturality.md) in $d$. These [bijections](../../../../../bijection.md) are the required [adjunction](../../../../../adjoint-functors.md) $F\dashv G$.

For necessity, if $F\dashv G$, the single arrow $\eta_c:c\to GFc$ is a solution [set](../../../../../set-split.md): the transpose of any $u:c\to Gd$ gives its factorization through $\eta_c$. If $d$ is a limiting cone vertex of a small diagram $D_j$ in $\mathcal D$, then, naturally in $c$,

$$
\mathcal C(c,Gd)\cong\mathcal D(Fc,d)
\cong\lim_j\mathcal D(Fc,D_j)
\cong\lim_j\mathcal C(c,GD_j).
$$

These are the canonical cone-factorization [bijections](../../../../../bijection.md), so $Gd$ with its image projections is a [categorical limit](../../../../../categorical-limit.md) of $GD_j$. Thus $G$ preserves all small [categorical limits](../../../../../categorical-limit.md), completing both directions of the theorem.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 23](../../paper-23-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
