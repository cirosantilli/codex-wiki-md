<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the covariant category in this part, put $\mathcal E=[\mathcal C,\mathbf{Set}]$ and $r_c=\mathcal C(c,-)$. Its global-sections [functor](../../../../../../functor.md) is $\Gamma=\operatorname{Hom}(1,-)$, the limit of the diagram. If $\Gamma$ is also an inverse image, it is a [left adjoint](../../../../../../adjoint-functors.md) and preserves all small [colimits](../../../../../../colimit.md).

Consider the canonical pointwise-surjective map

$$
q:\coprod_{c\in\mathcal C}r_c\longrightarrow1.
$$

At $d$, the summand $r_d(d)$ contains $1_d$, so $q$ is an [epimorphism](../../../../../../epimorphism.md). In a [presheaf topos](../../../../../../presheaf-topos.md) [epimorphisms](../../../../../../epimorphism.md) are regular, and a colimit-preserving [functor](../../../../../../functor.md) preserves their coequalizer presentations. Thus $\Gamma q$ is surjective. Since $\Gamma$ preserves [coproducts](../../../../../../coproduct.md), some summand has a global element, yielding a section $s:1\to r_c$ of its unique map $r_c\to1$. **The constant singleton [functor](../../../../../../functor.md) is a retract of a covariant representable.**

Conversely, if $1$ is such a [retract in a category](../../../../../../retract-in-a-category.md), $\operatorname{Hom}(1,-)$ is a retract of $\operatorname{Hom}(r_c,-)$, which is evaluation at $c$ by the [Yoneda lemma](../../../../../../yoneda-lemma.md). Evaluation preserves [colimits](../../../../../../colimit.md) pointwise. The [colimit](../../../../../../colimit.md) comparison for a retract [functor](../../../../../../functor.md) is a retract of the evaluation comparison; a retract of an isomorphism is an isomorphism, so $\Gamma$ preserves all small [colimits](../../../../../../colimit.md). It also preserves [finite limits](../../../../../../finite-limit.md) because it is representable. A [right adjoint](../../../../../../adjoint-functors.md) can be constructed by

$$
R(S)(d)=\operatorname{Set}(\Gamma r_d,S).
$$

For $h:d\to d'$, precomposition gives $r_{d'}\to r_d$, and applying $\Gamma$ and then $\operatorname{Set}(-,S)$ gives $R(S)(d)\to R(S)(d')$. The presentation of every [functor](../../../../../../functor.md) as a [colimit](../../../../../../colimit.md) of representables gives $\operatorname{Hom}(F,R(S))\cong\operatorname{Set}(\Gamma F,S)$. Hence $\Gamma\dashv R$, so $\Gamma$ is an inverse image and the topos is local.

The retract condition has a precise interpretation as the [initial object criterion for a covariant local topos](../../../../../../initial-object-criterion-for-a-covariant-local-topos.md). Write the section as a natural family $u_d:c\to d$. Naturality says $h u_d=u_{d'}$ for every $h:d\to d'$. Put $e=u_c$. Then $e^2=e$ and every $f:c\to d$ satisfies $fe=u_d$. In the [idempotent completion](../../../../../../karoubi-envelope.md) of $\mathcal C$, the object $(c,e)$ is initial: an arrow from it to $(d,k)$ must satisfy $v=kv e$, and the identities force $v=u_d$; this arrow exists because $k u_d=u_d$ and $u_d e=u_d$.

Conversely an [initial object](../../../../../../initial-object.md) $(c,e)$ in the [idempotent completion](../../../../../../karoubi-envelope.md) gives that natural family and the retract. Therefore

$$
\boxed{[\mathcal C,\mathbf{Set}]\text{ is local}
\ \Longleftrightarrow\
\operatorname{Kar}(\mathcal C)\text{ has an initial object}.}
$$

If $\mathcal C$ is already [idempotent-complete](../../../../../../cauchy-complete-category.md), this is equivalent to an [initial object](../../../../../../initial-object.md) in $\mathcal C$ itself, and $\Gamma$ is evaluation there. The word is initial, not terminal, because this question uses covariant [functors](../../../../../../functor.md).

One cannot omit [idempotent completion](../../../../../../karoubi-envelope.md) for a general small category. Take the one-object category of the [monoid](../../../../../../monoid.md) $\{1,0\}$ with absorbing zero. It has no [initial object](../../../../../../initial-object.md) because its endomorphism set has two elements, but the natural family $u=0$ satisfies $m0=0$ for every $m$. Its covariant [functor](../../../../../../functor.md) category is local. Concretely, a [functor](../../../../../../functor.md) is a set with an idempotent operator, and its global sections are the fixed points of that operator.

For a [topological space](../../../../../../topological-space.md) $X$, there is an equally explicit criterion. If $\mathbf{Sh}(X)$ is local, apply $\Gamma$ to the [epimorphism](../../../../../../epimorphism.md) $\coprod_iU_i\to1$ associated with any open cover $X=\bigcup_iU_i$, regarding the opens as [subterminal sheaves](../../../../../../subterminal-sheaf.md). Since $\Gamma U_i$ is a singleton exactly when $U_i=X$, and otherwise empty, [coproduct](../../../../../../coproduct.md) and [epimorphism](../../../../../../epimorphism.md) preservation force some $U_i=X$.

Thus every open cover of $X$ contains $X$ itself. Conversely this [open cover criterion for a local sheaf topos](../../../../../../open-cover-criterion-for-a-local-sheaf-topos.md) condition is equivalent to existence of a point $x$ whose only open neighborhood is $X$: the union of all proper open sets cannot be all of $X$, so choose $x$ outside it. Such a point plainly forces any cover to contain $X$. Empty spaces fail the condition.

At this point, the [stalk functor](../../../../../../stalk-functor-for-presheaves-of-sets.md) $F\mapsto F_x$ is simply $F(X)=\Gamma F$, since there is only one open neighborhood. Its [right adjoint](../../../../../../adjoint-functors.md) is the [skyscraper sheaf of sets](../../../../../../skyscraper-sheaf-of-sets.md)

$$
R(S)(V)=
\begin{cases}S,&x\in V,\\\{*\},&x\notin V.\end{cases}
$$

A morphism $F\to R(S)$ is determined exactly by its map $F(X)\to S$, because all proper opens omit $x$. Hence $\Gamma\dashv R$, and $\Gamma$ preserves [finite limits](../../../../../../finite-limit.md), proving locality. Consequently

$$
\boxed{\mathbf{Sh}(X)\text{ is local}
\ \Longleftrightarrow\
\exists x\in X\text{ with no proper open neighborhood}.}
$$

In a $T_0$ space this distinguished point is unique and closed. In a $T_1$ space the condition forces $X$ to be a singleton. Indistinguishable points in a non-$T_0$ space can all have this property; uniqueness of an actual point is not part of the general criterion.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
