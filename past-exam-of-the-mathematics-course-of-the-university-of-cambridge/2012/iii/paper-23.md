# Paper 23

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_23.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_23.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)

## 1

↑ **Parent:** [Paper 23](paper-23.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let $M\times X$ have the diagonal [right monoid action](../../../algebra.md#right-monoid-action) $(g,x)m=(gm,xm)$, and put $E=\operatorname{Hom}_M(M\times X,Y)$. Define the right action on this set of [equivariant maps of monoid sets](../../../algebra.md#equivariant-map-of-monoid-sets) by

$$
(ek)(g,x)=e(kg,x).
$$

It really stays in $E$: $(ek)(gm,xm)=e(kgm,xm)=e(kg,x)m$. Also $e1=e$ and $((ek)l)(g,x)=e(klg,x)=(e(kl))(g,x)$, so it satisfies the right-action law. Left multiplication in the first argument is intentional; no commutativity of $M$ has been assumed.

Define the [evaluation map of an exponential object](../../../category.md#evaluation-map-of-an-exponential-object)

$$
\operatorname{ev}:E\times X\to Y,\qquad \operatorname{ev}(e,x)=e(1,x).
$$

It is equivariant, because

$$
\operatorname{ev}(ek,xk)=e(k,xk)=e((1,x)k)=e(1,x)k.
$$

For any right $M$-set $Z$ and [equivariant map](../../../group-theory.md#equivariant-map) $h:Z\times X\to Y$, define its [currying](../../../category.md#currying) by

$$
\widehat h(z)(g,x)=h(zg,x).
$$

For fixed $z$, this is equivariant in the diagonal variables: $h(zgm,xm)=h(zg,x)m$. The map $z\mapsto\widehat h(z)$ is also equivariant, since

$$
\widehat h(zk)(g,x)=h(zkg,x)=(\widehat h(z)k)(g,x).
$$

It satisfies $\operatorname{ev}(\widehat h(z),x)=h(z,x)$.

Conversely, given an equivariant $u:Z\to E$, set $h(z,x)=u(z)(1,x)$. Evaluation makes this equivariant, and currying recovers $u$:

$$
\widehat h(z)(g,x)=u(zg)(1,x)=(u(z)g)(1,x)=u(z)(g,x).
$$

These constructions are inverse and natural in $Z$. Therefore they establish the [exponential object](../../../category.md#exponential-object) universal property

$$
\boxed{\operatorname{Hom}_M(Z,E)\cong\operatorname{Hom}_M(Z\times X,Y),\qquad
Y^X=E.}
$$

This is the [exponential of right monoid actions](../../../algebra.md#exponential-of-right-monoid-actions), not the set of ordinary maps $X\to Y$ with an arbitrarily guessed action.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

When $M=G$ is a [group](../../../group.md), evaluation at its identity gives a bijection from the previous equivariant-map set to all functions $X\to Y$. For an arbitrary function $f$, the inverse construction is

$$
e_f(g,x)=f(xg^{-1})g.
$$

Indeed,

$$
e_f(gk,xk)=f(xk(gk)^{-1})gk=f(xg^{-1})gk=e_f(g,x)k,
$$

so $e_f$ is an [equivariant map](../../../group-theory.md#equivariant-map). Conversely, if $e$ is equivariant, $(g,x)=(1,xg^{-1})g$ implies $e(g,x)=e(1,xg^{-1})g$, so $e=e_f$ for $f(x)=e(1,x)$.

Transport the right action from part (a) through this bijection. At $x$ its value is

$$
(ek)(1,x)=e(k,x)=f(xk^{-1})k.
$$

Thus the [exponential of right group actions](../../../algebra.md#exponential-of-right-group-actions) is

$$
\boxed{Y^X=\operatorname{Set}(X,Y),\qquad (fk)(x)=f(xk^{-1})k.}
$$

For clarity, the right-action law holds even in a nonabelian [group](../../../group.md):

$$
((fk)l)(x)=f(xl^{-1}k^{-1})kl=f(x(kl)^{-1})kl=(f(kl))(x).
$$

Evaluation is equivariant because $(fk)(xk)=f(x)k$. The underlying functions need not be equivariant; the fixed points of this exponential action are exactly the equivariant functions.

## 2

↑ **Parent:** [Paper 23](paper-23.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

At a point $x\in X$, all restrictions of the [constant presheaf of sets](../../../algebraic-geometry.md#constant-presheaf-of-sets) are identities. Two representatives $(U,t)$ and $(V,t')$ give the same [germ](../../../ringed-space.md#germ-of-a-sheaf-section) precisely when $t=t'$, so its [stalk](../../../ringed-space.md#stalk-of-a-sheaf) is canonically $T$. The disjoint union of the stalks is therefore the set $X\times T$.

The topology of the associated [étale space of a presheaf](../../../algebraic-geometry.md#etale-space-of-a-presheaf) has basic opens obtained from sections over open $U$. For the constant section $t$, that basic open is $U\times\{t\}$. These are exactly the basic opens of the product topology with $T$ discrete. Consequently the germ-space identification is a homeomorphism over $X$, and the projection

$$
\boxed{p:X\times T_{\mathrm{disc}}\longrightarrow X}
$$

is a local homeomorphism.

A continuous section over $V$ has the form $x\mapsto(x,f(x))$, where $f:V\to T_{\mathrm{disc}}$ is continuous, equivalently [locally constant](../../../calculus.md#locally-constant-function). Its sections form the [constant sheaf of sets](../../../algebraic-geometry.md#constant-sheaf-of-sets):

$$
\boxed{\Delta T(V)=\{f:V\to T:f\text{ is locally constant}\}.}
$$

The [sheaf gluing axiom](../../../algebraic-geometry.md#sheaf-gluing-axiom) follows by gluing the functions; continuity is local. This includes $\Delta T(\varnothing)$ being a singleton, even when the constant presheaf's value on the empty open set was $T$. The construction is its [sheafification](../../../ringed-space.md#sheafification).

A function $u:T\to T'$ acts by postcomposition on [locally constant](../../../calculus.md#locally-constant-function) functions, defining a [functor](../../../category.md#functor) $\Delta:\mathbf{Set}\to\mathbf{Sh}(X)$. It preserves identities and composition.

To prove the [adjunction](../../../category.md#adjoint-functors) with the [global sections functor](../../../category-theory.md#global-sections-functor), let $F$ be a sheaf. A sheaf morphism $\lambda:\Delta T\to F$ gives a function

$$
T\longrightarrow F(X),\qquad
t\longmapsto\lambda_X(\text{constant function }t).
$$

Conversely, suppose global sections $s_t\in F(X)$ are prescribed for every $t\in T$. For a [locally constant](../../../calculus.md#locally-constant-function) $f:V\to T$, its fibres $V_t=f^{-1}(t)$ are disjoint open sets covering $V$. Restrict $s_t$ to $V_t$ and glue these sections. They agree on intersections, which are empty, so unique gluing defines $\lambda_V(f)$. Restriction to smaller opens commutes with this construction, making $\lambda$ a sheaf morphism.

Applying the two constructions successively returns the original data: a [locally constant](../../../calculus.md#locally-constant-function) function is locally one of the constant functions, and sheaf morphisms respect those restrictions and unique gluing. Naturality in $T$ and $F$ follows from postcomposition and restriction. Hence

$$
\boxed{\operatorname{Hom}_{\mathbf{Sh}(X)}(\Delta T,F)
\cong\operatorname{Set}(T,\Gamma F),\qquad \Delta\dashv\Gamma.}
$$

For an empty space the same proof works: all global sections sets are singletons, and the sheaf category is degenerate. Constant sheaves are generally [locally constant](../../../calculus.md#locally-constant-function) rather than globally constant on disconnected opens.

## 3

↑ **Parent:** [Paper 23](paper-23.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Write $\widehat{\mathcal C}=[\mathcal C^{\mathrm{op}},\mathbf{Set}]$ and similarly for $\mathcal D$. The induced inverse-image [functor](../../../category.md#functor) is precomposition:

$$
u^*:\widehat{\mathcal D}\to\widehat{\mathcal C},
\qquad u^*(Q)=Q\circ f^{\mathrm{op}}.
$$

All [categorical limits](../../../category.md#categorical-limit) in a [presheaf category](../../../category.md#presheaf-category) are computed pointwise. Thus $u^*$ preserves every limit, in particular [finite limits](../../../category.md#finite-limit).

Because the indexing categories are small and $\mathbf{Set}$ is complete and cocomplete, both [Kan extensions](../../../category.md#kan-extension) along $f^{\mathrm{op}}$ exist. Their universal properties give

$$
\boxed{
u_!=\operatorname{Lan}_{f^{\mathrm{op}}}
\ \dashv\ u^*=(-)\circ f^{\mathrm{op}}
\ \dashv\ u_*=\operatorname{Ran}_{f^{\mathrm{op}}}.}
$$

For example their values are the comma-category formulas

$$
(u_!P)(d)=\operatorname*{colim}_{(f^{\mathrm{op}}\downarrow d)}P(c),
\qquad
(u_*P)(d)=\operatorname*{lim}_{(d\downarrow f^{\mathrm{op}})}P(c).
$$

The comma categories here are formed in $\mathcal D^{\mathrm{op}}$: an object of the first involves $f(c)\to d$ there, equivalently $d\to f(c)$ in $\mathcal D$. An object of the second involves $d\to f(c)$ there, equivalently $f(c)\to d$ in $\mathcal D$. Keeping the opposite category explicit prevents reversal of the two constructions.

The right-hand [adjunction](../../../category.md#adjoint-functors) and finite-limit preservation are exactly the axioms for a [geometric morphism](../../../category-theory.md#geometric-morphism) $u:\widehat{\mathcal C}\to\widehat{\mathcal D}$. The extra [left adjoint](../../../category.md#adjoint-functors) makes it an [essential geometric morphism](../../../category-theory.md#essential-geometric-morphism). On [representable presheaves](../../../category.md#representable-functor), its [left adjoint](../../../category.md#adjoint-functors) satisfies $u_!(y_{\mathcal C}c)\cong y_{\mathcal D}(fc)$, by the [Yoneda lemma](../../../category.md#yoneda-lemma) and the left [adjunction](../../../category.md#adjoint-functors). This identifies the induced morphism directly with the original [functor](../../../category.md#functor) $f$.

## 4

↑ **Parent:** [Paper 23](paper-23.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Present the [Grothendieck topos](../../../category-theory.md#grothendieck-topos) as $\mathcal E=\mathbf{Sh}(\mathcal C,J)$ for a small [site](../../../category.md#site-category-theory). Let $a:\widehat{\mathcal C}\to\mathcal E$ be [sheafification](../../../ringed-space.md#sheafification) and $i$ the inclusion. The standard [sheafification](../../../ringed-space.md#sheafification) construction supplies $a\dashv i$, with $a$ preserving [finite limits](../../../category.md#finite-limit). Concretely, matching-family constructions commute with [finite limits](../../../category.md#finite-limit), and their directed refinement over covering sieves does so as well. Limits of sheaves are computed in the [presheaf category](../../../category.md#presheaf-category), so $\mathcal E$ has [finite limits](../../../category.md#finite-limit); its [colimits](../../../category.md#colimit) are sheafifications of presheaf [colimits](../../../category.md#colimit).

For sheaves $A,B$, form the presheaf exponential

$$
E(c)=\operatorname{Nat}(y c\times A,B).
$$

It is a sheaf. Indeed, for a covering sieve $S\hookrightarrow y c$, one has $aS\cong a(y c)$. Exponential [adjunction](../../../category.md#adjoint-functors), [sheafification](../../../ringed-space.md#sheafification) [adjunction](../../../category.md#adjoint-functors) and left exactness give

$$
\operatorname{Nat}(S,E)
\cong\operatorname{Nat}(S\times A,B)
\cong\operatorname{Hom}_{\mathcal E}(aS\times A,B)
\cong\operatorname{Hom}_{\mathcal E}(a(y c)\times A,B)
\cong\operatorname{Nat}(y c,E).
$$

These are the restriction comparisons, proving the sheaf condition. Restricting the presheaf exponential [adjunction](../../../category.md#adjoint-functors) to sheaves now makes $E=B^A$ in $\mathcal E$.

The [subobject classifier](../../../category-theory.md#subobject-classifier) is the sheaf $\Omega_J$ of [J-closed sieves](../../../category.md#j-closed-sieve). A sieve $S$ on $c$ is J-closed when, for every $f:d\to c$, $f^*S\in J(d)$ implies $f\in S$. Pullback of sieves defines its restrictions, and the maximal sieve defines truth. Local sieve data glue by taking the J-closure of their compatible generated sieve; uniqueness follows because membership in a J-closed sieve is local. This proves that $\Omega_J$ is a sheaf.

For a subsheaf $A\hookrightarrow B$, the characteristic morphism sends $b\in B(c)$ to

$$
\chi_A(b)=\{f:d\to c:B(f)(b)\in A(d)\}.
$$

This sieve is J-closed because local membership in a subsheaf descends by its gluing axiom. Pulling truth back recovers exactly $A$. Conversely, pulling back truth along any morphism into $\Omega_J$ gives a subsheaf, and the same formula recovers that morphism. **[Finite limits](../../../category.md#finite-limit), exponentials and this classifier make every [Grothendieck topos](../../../category-theory.md#grothendieck-topos) an [elementary topos](../../../category-theory.md#elementary-topos).**

Here are the explicit [Heyting operations on subsheaves](../../../mathematical-logic.md#heyting-operations-on-subsheaves) of an object $B$. Intersections give meets:

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

Equivalently, $b$ locally lies in one of the $A_i$, with the index allowed to vary across the covering arrows. This is the J-closure of the pointwise union, or its [sheafification](../../../ringed-space.md#sheafification). It is the smallest subsheaf containing every $A_i$, since any such subsheaf must contain sections locally in it.

The bottom is the empty join, namely the initial [subobject](../../../category.md#subobject). Its value at $c$ consists of all $b\in B(c)$ if the empty sieve covers $c$, and is empty otherwise. This detail matters on [sites](../../../category.md#site-category-theory) with empty covers; it is not safe to use an always-empty presheaf as the initial sheaf.

Implication is described without any pointwise-complement assumption:

$$
\boxed{
(A\Rightarrow D)(c)=
\{b\in B(c):
\text{ for every }f:d\to c,\ B(f)b\in A(d)\Longrightarrow B(f)b\in D(d)\}.}
$$

Restrictions preserve this condition. It is also local: pull a covering sieve back along an arbitrary $f$, use membership in $A$ on those restrictions, then descend their membership in $D$. Thus it is a subsheaf. It satisfies the defining [Heyting algebra](../../../mathematical-logic.md#heyting-algebra) [adjunction](../../../category.md#adjoint-functors)

$$
C\leq(A\Rightarrow D)\quad\Longleftrightarrow\quad C\cap A\leq D.
$$

For the forward direction take the identity restriction. For the reverse direction every restriction of a section of $C$ remains in $C$, so membership in $A$ forces membership in $D$. Negation is $\neg A=A\Rightarrow0$. These formulas give the complete Heyting algebra structure on $\operatorname{Sub}_{\mathcal E}(B)$; in general negation is a pseudocomplement rather than a set-theoretic complement.

## 5

↑ **Parent:** [Paper 23](paper-23.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

In a [Grothendieck topos](../../../category-theory.md#grothendieck-topos) define

$$
\Delta S=\coprod_{s\in S}1,\qquad
\Gamma A=\operatorname{Hom}_{\mathcal E}(1,A).
$$

The [coproduct](../../../category.md#coproduct) universal property gives $\operatorname{Hom}_{\mathcal E}(\Delta S,A)\cong\operatorname{Set}(S,\Gamma A)$, naturally. Thus $\Delta\dashv\Gamma$. On any sheaf presentation, $\Delta$ is the composite of the constant-presheaf [functor](../../../category.md#functor) with [sheafification](../../../ringed-space.md#sheafification). The former preserves [finite limits](../../../category.md#finite-limit) pointwise, and the latter is left exact, so $\Delta$ preserves [finite limits](../../../category.md#finite-limit). Therefore these [functors](../../../category.md#functor) define a [geometric morphism](../../../category-theory.md#geometric-morphism) $\gamma:\mathcal E\to\mathbf{Set}$.

For uniqueness, let $v$ be any such [geometric morphism](../../../category-theory.md#geometric-morphism). Its inverse image is a [left adjoint](../../../category.md#adjoint-functors) and preserves the [terminal object](../../../category.md#terminal-object). Every set has the canonical [coproduct](../../../category.md#coproduct) decomposition $S=\coprod_{s\in S}\{*\}$, so

$$
v^*S\cong\coprod_{s\in S}v^*\{*\}
\cong\coprod_{s\in S}1=\Delta S.
$$

These isomorphisms respect all functions between sets, giving a [natural isomorphism](../../../category.md#natural-isomorphism) $v^*\cong\Delta$. The [right adjoint](../../../category.md#adjoint-functors) is then unique up to the corresponding [natural isomorphism](../../../category.md#natural-isomorphism), so $v_*\cong\Gamma$. **There is a unique [geometric morphism](../../../category-theory.md#geometric-morphism) to sets, up to isomorphism**, called the [global sections geometric morphism](../../../category-theory.md#global-sections-geometric-morphism). This also applies to the degenerate topos.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

For the covariant category in this part, put $\mathcal E=[\mathcal C,\mathbf{Set}]$ and $r_c=\mathcal C(c,-)$. Its global-sections [functor](../../../category.md#functor) is $\Gamma=\operatorname{Hom}(1,-)$, the limit of the diagram. If $\Gamma$ is also an inverse image, it is a [left adjoint](../../../category.md#adjoint-functors) and preserves all small [colimits](../../../category.md#colimit).

Consider the canonical pointwise-surjective map

$$
q:\coprod_{c\in\mathcal C}r_c\longrightarrow1.
$$

At $d$, the summand $r_d(d)$ contains $1_d$, so $q$ is an [epimorphism](../../../category.md#epimorphism). In a [presheaf topos](../../../category.md#presheaf-topos) [epimorphisms](../../../category.md#epimorphism) are regular, and a colimit-preserving [functor](../../../category.md#functor) preserves their coequalizer presentations. Thus $\Gamma q$ is surjective. Since $\Gamma$ preserves [coproducts](../../../category.md#coproduct), some summand has a global element, yielding a section $s:1\to r_c$ of its unique map $r_c\to1$. **The constant singleton [functor](../../../category.md#functor) is a retract of a covariant representable.**

Conversely, if $1$ is such a [retract in a category](../../../category.md#retract-in-a-category), $\operatorname{Hom}(1,-)$ is a retract of $\operatorname{Hom}(r_c,-)$, which is evaluation at $c$ by the [Yoneda lemma](../../../category.md#yoneda-lemma). Evaluation preserves [colimits](../../../category.md#colimit) pointwise. The [colimit](../../../category.md#colimit) comparison for a retract [functor](../../../category.md#functor) is a retract of the evaluation comparison; a retract of an isomorphism is an isomorphism, so $\Gamma$ preserves all small [colimits](../../../category.md#colimit). It also preserves [finite limits](../../../category.md#finite-limit) because it is representable. A [right adjoint](../../../category.md#adjoint-functors) can be constructed by

$$
R(S)(d)=\operatorname{Set}(\Gamma r_d,S).
$$

For $h:d\to d'$, precomposition gives $r_{d'}\to r_d$, and applying $\Gamma$ and then $\operatorname{Set}(-,S)$ gives $R(S)(d)\to R(S)(d')$. The presentation of every [functor](../../../category.md#functor) as a [colimit](../../../category.md#colimit) of representables gives $\operatorname{Hom}(F,R(S))\cong\operatorname{Set}(\Gamma F,S)$. Hence $\Gamma\dashv R$, so $\Gamma$ is an inverse image and the topos is local.

The retract condition has a precise interpretation as the [initial object criterion for a covariant local topos](../../../category-theory.md#initial-object-criterion-for-a-covariant-local-topos). Write the section as a natural family $u_d:c\to d$. Naturality says $h u_d=u_{d'}$ for every $h:d\to d'$. Put $e=u_c$. Then $e^2=e$ and every $f:c\to d$ satisfies $fe=u_d$. In the [idempotent completion](../../../category.md#karoubi-envelope) of $\mathcal C$, the object $(c,e)$ is initial: an arrow from it to $(d,k)$ must satisfy $v=kv e$, and the identities force $v=u_d$; this arrow exists because $k u_d=u_d$ and $u_d e=u_d$.

Conversely an [initial object](../../../category.md#initial-object) $(c,e)$ in the [idempotent completion](../../../category.md#karoubi-envelope) gives that natural family and the retract. Therefore

$$
\boxed{[\mathcal C,\mathbf{Set}]\text{ is local}
\ \Longleftrightarrow\
\operatorname{Kar}(\mathcal C)\text{ has an initial object}.}
$$

If $\mathcal C$ is already [idempotent-complete](../../../category.md#cauchy-complete-category), this is equivalent to an [initial object](../../../category.md#initial-object) in $\mathcal C$ itself, and $\Gamma$ is evaluation there. The word is initial, not terminal, because this question uses covariant [functors](../../../category.md#functor).

One cannot omit [idempotent completion](../../../category.md#karoubi-envelope) for a general small category. Take the one-object category of the [monoid](../../../algebra.md#monoid) $\{1,0\}$ with absorbing zero. It has no [initial object](../../../category.md#initial-object) because its endomorphism set has two elements, but the natural family $u=0$ satisfies $m0=0$ for every $m$. Its covariant [functor](../../../category.md#functor) category is local. Concretely, a [functor](../../../category.md#functor) is a set with an idempotent operator, and its global sections are the fixed points of that operator.

For a [topological space](../../../topology.md#topological-space) $X$, there is an equally explicit criterion. If $\mathbf{Sh}(X)$ is local, apply $\Gamma$ to the [epimorphism](../../../category.md#epimorphism) $\coprod_iU_i\to1$ associated with any open cover $X=\bigcup_iU_i$, regarding the opens as [subterminal sheaves](../../../category.md#subterminal-sheaf). Since $\Gamma U_i$ is a singleton exactly when $U_i=X$, and otherwise empty, [coproduct](../../../category.md#coproduct) and [epimorphism](../../../category.md#epimorphism) preservation force some $U_i=X$.

Thus every open cover of $X$ contains $X$ itself. Conversely this [open cover criterion for a local sheaf topos](../../../category-theory.md#open-cover-criterion-for-a-local-sheaf-topos) condition is equivalent to existence of a point $x$ whose only open neighborhood is $X$: the union of all proper open sets cannot be all of $X$, so choose $x$ outside it. Such a point plainly forces any cover to contain $X$. Empty spaces fail the condition.

At this point, the [stalk functor](../../../ringed-space.md#stalk-functor-for-presheaves-of-sets) $F\mapsto F_x$ is simply $F(X)=\Gamma F$, since there is only one open neighborhood. Its [right adjoint](../../../category.md#adjoint-functors) is the [skyscraper sheaf of sets](../../../algebraic-geometry.md#skyscraper-sheaf-of-sets)

$$
R(S)(V)=
\begin{cases}S,&x\in V,\\\{*\},&x\notin V.\end{cases}
$$

A morphism $F\to R(S)$ is determined exactly by its map $F(X)\to S$, because all proper opens omit $x$. Hence $\Gamma\dashv R$, and $\Gamma$ preserves [finite limits](../../../category.md#finite-limit), proving locality. Consequently

$$
\boxed{\mathbf{Sh}(X)\text{ is local}
\ \Longleftrightarrow\
\exists x\in X\text{ with no proper open neighborhood}.}
$$

In a $T_0$ space this distinguished point is unique and closed. In a $T_1$ space the condition forces $X$ to be a singleton. Indistinguishable points in a non-$T_0$ space can all have this property; uniqueness of an actual point is not part of the general criterion.

## 6

↑ **Parent:** [Paper 23](paper-23.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

A [geometric formula](../../../mathematical-logic.md#geometric-formula) is built from atomic formulas, including equality, using finite conjunctions, arbitrary set-indexed disjunctions and existential quantification in a finite variable context. Truth is the empty conjunction and falsity the empty disjunction. A [geometric theory](../../../mathematical-logic.md#geometric-theory) is a set of sequents $\phi\vdash_{\vec x}\psi$ between such formulas over a many-sorted signature. The context supplies the universal force of an axiom; unrestricted universal quantification, implication and negation are not formula constructors in this fragment.

These choices are exactly suited to [inverse image functors of geometric morphisms](../../../category-theory.md#inverse-image-functor-of-a-geometric-morphism). Finite-limit preservation handles equality and conjunction; [colimit](../../../category.md#colimit) and image preservation handle disjunction and existential quantification. Therefore an inverse image carries an internal model of a [geometric theory](../../../mathematical-logic.md#geometric-theory) to another model.

Construct the [geometric syntactic category](../../../mathematical-logic.md#geometric-syntactic-category) $\mathcal C_{\mathbb T}$ as follows. Objects are formulas in context $\{\vec x.\phi\}$, modulo provable renaming and equivalence. A morphism to $\{\vec y.\psi\}$ is an equivalence class of formulas $\theta(\vec x,\vec y)$ that are provably total and single-valued:

$$
\theta\vdash\phi\wedge\psi,\qquad
\phi\vdash_{\vec x}\exists\vec y\,\theta,\qquad
\theta(\vec x,\vec y)\wedge\theta(\vec x,\vec y')
\vdash_{\vec x,\vec y,\vec y'}\vec y=\vec y'.
$$

The last notation abbreviates componentwise equality. Identity is equality of the context variables; composition is existential conjunction over the intermediate tuple. The category has [finite limits](../../../category.md#finite-limit), formed through conjunction and equality.

Give it the [geometric syntactic topology](../../../mathematical-logic.md#geometric-syntactic-topology) $J_{\mathbb T}$. A family of arrows represented by $\theta_i(\vec y_i,\vec x)$ into $\{\vec x.\phi\}$ covers when

$$
\mathbb T\vdash_{\vec x}
\phi\ \Longrightarrow\ \bigvee_i\exists\vec y_i\,\theta_i(\vec y_i,\vec x).
$$

Pullback stability is substitution, and transitivity comes from distributing existential conjunction through the covering disjunctions. Thus the generated sieves define a [Grothendieck topology](../../../category.md#grothendieck-topology). Empty covers impose the interpretation of falsity as the [initial object](../../../category.md#initial-object).

The [classifying topos](../../../category-theory.md#classifying-topos) is

$$
\boxed{\mathbf{Set}[\mathbb T]=
\mathbf{Sh}(\mathcal C_{\mathbb T},J_{\mathbb T}).}
$$

Its universal model $U_{\mathbb T}$ assigns a sort $A$ the sheafified representable of $\{x^A.\top\}$, functions their definable graph morphisms and relations their definable [subobjects](../../../category.md#subobject). The syntactic covering conditions make the axioms valid in this model.

For the universal property, interpreting formulas in a model $M$ in a [Grothendieck topos](../../../category-theory.md#grothendieck-topos) $\mathcal F$ gives a finite-limit-preserving, $J_{\mathbb T}$-continuous [functor](../../../category.md#functor) $\mathcal C_{\mathbb T}\to\mathcal F$: covers go to jointly epimorphic families precisely because the relevant sequents hold. The [Diaconescu equivalence for geometric morphisms](../../../category-theory.md#diaconescu-equivalence-for-geometric-morphisms) associates to this [functor](../../../category.md#functor) a [geometric morphism](../../../category-theory.md#geometric-morphism) $\mathcal F\to\mathbf{Set}[\mathbb T]$. Conversely, pulling $U_{\mathbb T}$ back along a [geometric morphism](../../../category-theory.md#geometric-morphism) gives a model. The constructions on models and their homomorphisms are inverse up to [natural isomorphism](../../../category.md#natural-isomorphism), yielding

$$
\boxed{\operatorname{Geom}(\mathcal F,\mathbf{Set}[\mathbb T])
\simeq\mathbb T\operatorname{-Mod}(\mathcal F)}
$$

naturally in $\mathcal F$. This proves the required classifying property, not merely classification of set-valued models.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

**Yes, with the Horn/Cartesian-fragment convention.** A [Horn theory](../../../mathematical-logic.md#horn-theory) uses positive finite-conjunction sequents and has a [Cartesian syntactic category](../../../mathematical-logic.md#cartesian-syntactic-category) $\mathcal C_{\mathbb T}^{\mathrm{cart}}$ with [finite limits](../../../category.md#finite-limit). Provably uniquely witnessed existential formulas can also be admitted without changing the finite-limit nature of its semantics. Its internal models are precisely finite-limit-preserving [functors](../../../category.md#functor) from that category.

For a category with [finite limits](../../../category.md#finite-limit), [flat functors](../../../category.md#flat-functor) into a [Grothendieck topos](../../../category-theory.md#grothendieck-topos) are exactly finite-limit-preserving [functors](../../../category.md#functor). In sets, the reason is concrete: the [category of elements](../../../category.md#category-of-elements) of a covariant left-exact [functor](../../../category.md#functor) is cofiltered. Its [terminal object](../../../category.md#terminal-object) supplies nonemptiness, products supply cones over pairs of elements, and [equalizers](../../../category.md#equaliser) supply equalizing cones over parallel arrows. Conversely a cofiltered [category of elements](../../../category.md#category-of-elements) expresses the [functor](../../../category.md#functor) as a filtered [colimit](../../../category.md#colimit) of covariant representables; filtered [colimits](../../../category.md#colimit) of sets commute with [finite limits](../../../category.md#finite-limit). The internal version uses the same cone conditions locally.

The presheaf form of the [Diaconescu equivalence for geometric morphisms](../../../category-theory.md#diaconescu-equivalence-for-geometric-morphisms) therefore identifies [geometric morphisms](../../../category-theory.md#geometric-morphism) into

$$
\boxed{[(\mathcal C_{\mathbb T}^{\mathrm{cart}})^{\mathrm{op}},\mathbf{Set}]}
$$

with internal Horn models, naturally in the domain topos. This is the [presheaf classifier of a Horn theory](../../../mathematical-logic.md#presheaf-classifier-of-a-horn-theory).

Equivalently, using a small skeleton of the category $\mathcal A$ of finitely presented set-based Horn models, the classifier is $[\mathcal A,\mathbf{Set}]$, with covariant [functors](../../../category.md#functor). The duality $\mathcal A\simeq(\mathcal C_{\mathbb T}^{\mathrm{cart}})^{\mathrm{op}}$ sends a formula to the model generated by its tuple subject to its finite constraints. **The presheaf claim does not extend merely because a general geometric or regular theory has no written disjunctions**: arbitrary existential witnesses are not uniquely witnessed Horn data.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

[Morita equivalence of geometric theories](../../../category-theory.md#morita-equivalence-of-geometric-theories) means equivalence of their [classifying toposes](../../../category-theory.md#classifying-topos). Equivalently, their categories of models in every [Grothendieck topos](../../../category-theory.md#grothendieck-topos) are equivalent pseudonaturally with respect to inverse image. Agreement only of their set-based model categories, without this natural internal-model structure, is not the definition.

Suppose $\mathbf{Set}[\mathbb T]\simeq\mathbf{Set}[\mathbb S]=\mathcal E$. A property expressed intrinsically in terms of the topos is the same under either presentation. One can therefore translate a [site](../../../category.md#site-category-theory) or logical characterization of that property from $\mathbb T$ into one for $\mathbb S$. Examples include Booleanity, connectedness, atomicity and the structure of the [subtopos](../../../category-theory.md#subtopos) lattice. The bridge is the common invariant $\mathcal E$, rather than an assumed literal identification of the two signatures.

The [duality between geometric quotients and subtoposes](../../../category-theory.md#duality-between-geometric-quotients-and-subtoposes) makes this precise. A [geometric quotient theory](../../../mathematical-logic.md#geometric-quotient-theory) $\mathbb T'$ of $\mathbb T$ adds geometric axioms over the same signature. Quotients are identified when they prove the same geometric sequents. The theorem gives

$$
\boxed{\{\text{geometric quotients of }\mathbb T\}/\text{provable equivalence}
\ \longleftrightarrow\
\{\text{subtoposes of }\mathbf{Set}[\mathbb T]\}.}
$$

The [subtopos](../../../category-theory.md#subtopos) corresponding to $\mathbb T'$ is its [classifying topos](../../../category-theory.md#classifying-topos). Stronger axioms correspond to smaller [subtoposes](../../../category-theory.md#subtopos) under inclusion.

The [site](../../../category.md#site-category-theory) mechanism explains the correspondence. On $\mathcal C_{\mathbb T}$, an additional sequent requires the associated family of definable images to cover its antecedent. Adding these covering sieves produces a topology $J'\supseteq J_{\mathbb T}$ and a geometric embedding

$$
\mathbf{Sh}(\mathcal C_{\mathbb T},J')\hookrightarrow
\mathbf{Sh}(\mathcal C_{\mathbb T},J_{\mathbb T}).
$$

Conversely, [subtoposes](../../../category-theory.md#subtopos) correspond to such larger topologies; requiring their extra definable covers gives the corresponding deductively closed quotient theory. Pulling the universal model into the [subtopos](../../../category-theory.md#subtopos) supplies the universal model of the quotient.

Given a quotient $\mathbb T'$, transport its [subtopos](../../../category-theory.md#subtopos) along the chosen equivalence of [classifying toposes](../../../category-theory.md#classifying-topos). Apply the duality again to obtain a quotient $\mathbb S'$ of $\mathbb S$. Their [classifying toposes](../../../category-theory.md#classifying-topos) are equivalent, so

$$
\boxed{\mathbb T'\text{ and }\mathbb S'\text{ are Morita-equivalent}.}
$$

This is an explicit transfer principle for whole families of theory extensions and their order relations. Intrinsic constructions such as open, closed or Boolean [subtoposes](../../../category-theory.md#subtopos) can likewise be described in each syntax. Different descriptions may look unrelated, but their equality is explained by the common [subtopos](../../../category-theory.md#subtopos). No universal translation of individual formulas is asserted without choosing the relevant equivalence and interpretations.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2012](../../2012.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
