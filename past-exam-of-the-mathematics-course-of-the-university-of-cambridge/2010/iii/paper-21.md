# Paper 21

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper21.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper21.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [Solution](#6/solution)

## 1

↑ **Parent:** [Paper 21](paper-21.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

The [general adjoint functor theorem](../../../category.md#freyd-general-adjoint-functor-theorem) says that, for a [functor](../../../category.md#functor) $U:\mathcal A\to\mathcal B$ between [locally small categories](../../../category.md#locally-small-category), with $\mathcal A$ a [complete category](../../../category.md#complete-category), **$U$ has a left adjoint if and only if it preserves small limits and satisfies the solution-set condition**. The [solution-set condition](../../../category.md#solution-set-condition) means that for each $B\in\mathcal B$ there is a [set](../../../set.md) of arrows $b_i:B\to UA_i$ such that every $b:B\to UA$ factors as $U(a)b_i$ for some $i$ and some $a:A_i\to A$.

Here is the smallness argument behind the theorem. A [complete category](../../../category.md#complete-category) that is [locally small](../../../category.md#locally-small-category) and has a [weakly initial set](../../../category.md#weakly-initial-set) $(W_i)$ has an [initial object](../../../category.md#initial-object). Form the [product in a category](../../../category.md#product-category-theory) $W=\prod_iW_i$. It is weakly initial, since a projection $W\to W_i$ followed by a chosen arrow $W_i\to X$ gives an arrow $W\to X$. Take the simultaneous [equalizer](../../../category.md#equaliser) $e:E\to W$ of all [endomorphisms](../../../algebra.md#endomorphism) of $W$ with $1_W$; the family is a [set](../../../set.md) by local smallness. The object $E$ is also weakly initial. For parallel arrows $a,b:E\rightrightarrows X$, take their [equalizer](../../../category.md#equaliser) $j:Y\to E$ and a map $t:W\to Y$. Since $ejt$ is an [endomorphism](../../../algebra.md#endomorphism) of $W$, the defining property of $e$ gives $ejte=e$. Cancellation of the [monomorphism](../../../category.md#monomorphism) $e$ gives $jte=1_E$. Thus the [monomorphism](../../../category.md#monomorphism) $j$ has a right inverse and is an [isomorphism](../../../algebra.md#isomorphism), so $a=b$. Existence of arrows out of $E$ was already established, proving the [initial-object lemma for complete categories with a weakly initial set](../../../category.md#initial-object-lemma-for-complete-categories-with-a-weakly-initial-set).

If $U$ preserves small [categorical limits](../../../category.md#categorical-limit), the [comma category](../../../category.md#comma-category) $(B\downarrow U)$ is complete: take the limiting object in $\mathcal A$, and use preservation to assemble the arrows from $B$. It is [locally small](../../../category.md#locally-small-category), and the [solution-set condition](../../../category.md#solution-set-condition) provides a [weakly initial set](../../../category.md#weakly-initial-set). Its [initial object](../../../category.md#initial-object) is an arrow $\eta_B:B\to ULB$ with a natural bijection

$$
\mathcal A(LB,A)\cong\mathcal B(B,UA).
$$

For a [morphism](../../../algebra.md#morphism) $v:B\to B'$, define $Lv$ by $U(Lv)\eta_B=\eta_{B'}v$. Uniqueness proves functoriality and naturality, giving a [left adjoint](../../../category.md#adjoint-functors) $L\dashv U$. Conversely, a [right adjoint](../../../category.md#adjoint-functors) preserves [categorical limits](../../../category.md#categorical-limit), because applying the [adjunction](../../../category.md#adjoint-functors) converts a limiting [cone over a diagram](../../../category.md#cone-over-a-diagram) into the corresponding limiting cone of [hom-sets](../../../category.md#hom-set). Its [adjunction unit](../../../category.md#unit-of-an-adjunction) at $B$ is a singleton solution set. This proves both directions of the [general adjoint functor theorem](../../../category.md#freyd-general-adjoint-functor-theorem).

Apply it to the inclusion $J:\mathbf{KHaus}\hookrightarrow\mathbf{Top}$, where $\mathbf{KHaus}$ is the [full subcategory](../../../category.md#full-subcategory) of [compact Hausdorff spaces](../../../topology.md#compact-hausdorff-space). A small [product in a category](../../../category.md#product-category-theory) of [compact Hausdorff spaces](../../../topology.md#compact-hausdorff-space) is again compact Hausdorff by the [Tychonoff theorem](../../../geometry-and-topology.md#tychonoff-s-theorem). An [equalizer](../../../category.md#equaliser) of two [continuous functions](../../../calculus.md#continuous-function) into a [Hausdorff space](../../../topology.md#hausdorff-space) is closed, hence compact Hausdorff. Products and equalizers construct all small [categorical limits](../../../category.md#categorical-limit), and the inclusion preserves these constructions. Both [categories](../../../category.md) are [locally small](../../../category.md#locally-small-category).

Fix a [topological space](../../../topology.md#topological-space) $X$ and a [continuous function](../../../calculus.md#continuous-function) $f:X\to K$ into a [compact Hausdorff space](../../../topology.md#compact-hausdorff-space). The [closure](../../../topology.md#closure-topology) $K_f=\overline{f(X)}$ is compact Hausdorff and has a [dense subset](../../../topology.md#dense-set) of [cardinality](../../../set-theory.md#cardinality) at most $|X|$. The permitted cardinal estimate gives

$$
|K_f|\leq 2^{2^{|X|}}.
$$

For $X=\varnothing$, use $K_f=\varnothing$. Choose a [set](../../../set.md) of representatives of all compact Hausdorff topologies on underlying sets of cardinality at most this bound, and all [continuous functions](../../../calculus.md#continuous-function) from $X$ to those representatives. Every $f$ factors through one of them, using the inclusion $K_f\hookrightarrow K$. This is the [solution-set condition](../../../category.md#solution-set-condition). Consequently **the inclusion of compact Hausdorff spaces has a left adjoint**, the [compact Hausdorff reflection](../../../category.md#compact-hausdorff-reflection):

$$
\boxed{\mathbf{KHaus}(RX,K)\cong\mathbf{Top}(X,JK).}
$$

The universal arrow $X\to RX$ has [dense](../../../topology.md#dense-set) image: factoring it through its closed image and applying uniqueness supplies an inverse to that image inclusion. It need not be an embedding when $X$ is not sufficiently separated; the assertion is a [compact Hausdorff reflection](../../../category.md#compact-hausdorff-reflection), rather than a claim that every [topological space](../../../topology.md#topological-space) embeds in a compact Hausdorff space.

For completeness, the alternative [Special adjoint functor theorem](../../../category.md#special-adjoint-functor-theorem) can be proved from the same initial-object argument. Its limit form assumes that $\mathcal A$ is complete, locally small and [well-powered](../../../category.md#well-powered-category), with a [small cogenerating family](../../../category.md#cogenerating-set) $(Q_i)_{i\in I}$; then $U:\mathcal A\to\mathcal B$, with $\mathcal B$ locally small, has a [left adjoint](../../../category.md#adjoint-functors) precisely when it preserves small limits. To prove sufficiency, start with $b:B\to UA$ and intersect all [subobjects](../../../category.md#subobject) $M\hookrightarrow A$ through which $b$ factors after applying $U$. Well-poweredness makes this a small [intersection of subobjects](../../../category.md#intersection-of-subobjects), and preservation of limits gives a smallest supporting object $(M,b_M)$. For maps $s,t:M\rightrightarrows Q_i$, equality $U(s)b_M=U(t)b_M$ makes their [equalizer](../../../category.md#equaliser) another supporting subobject. Minimality forces that equalizer to be invertible, so $s=t$. Therefore

$$
\mathcal A(M,Q_i)\hookrightarrow\mathcal B(B,UQ_i),\qquad s\longmapsto U(s)b_M
$$

is an [injective function](../../../algebra.md#injective-function). The [evaluation embedding into cogenerator products](../../../category.md#evaluation-embedding-into-cogenerator-products) embeds $M$ in $\prod_iQ_i^{S_i}$, where $S_i$ is the realized subset of the fixed [set](../../../set.md) $\mathcal B(B,UQ_i)$. There are only a set of choices of these subsets, only a set of subobjects of each resulting product, and only a set of arrows from $B$ to each $U$-image. They give a solution set, so the already proved [general adjoint functor theorem](../../../category.md#freyd-general-adjoint-functor-theorem) applies. Necessity is again preservation of limits by a right adjoint. For $\mathbf{KHaus}$, [monomorphisms](../../../category.md#monomorphism) are embeddings onto closed subspaces, and $[0,1]$ is a [coseparator](../../../category.md#coseparator) because [continuous functions](../../../calculus.md#continuous-function) to it separate points. Thus the [Special adjoint functor theorem](../../../category.md#special-adjoint-functor-theorem) gives the same reflection directly.

## 2

↑ **Parent:** [Paper 21](paper-21.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

**The Yoneda embedding is an exact representation of a category, but does not by itself reduce the subject to the study of arbitrary functor categories.** There are both a size issue and a structure issue.

Let $\mathcal A$ be a [locally small category](../../../category.md#locally-small-category) and set $yA=\mathcal A(-,A)$. For a [categorical presheaf](../../../category.md#presheaf-category-theory) $P:\mathcal A^{\mathrm{op}}\to\mathbf{Set}$, a [natural transformation](../../../category.md#natural-transformation) $\theta:yA\to P$ is determined by $x=\theta_A(1_A)$. Indeed, naturality along $f:B\to A$ forces

$$
\theta_B(f)=P(f)(x).
$$

Conversely this formula defines a natural transformation for each $x\in P(A)$, since functoriality gives naturality along every $g:C\to B$. Taking $P=yA'$ gives

$$
\boxed{\operatorname{Nat}(yA,yA')\cong\mathcal A(A,A').}
$$

Thus the [Yoneda embedding](../../../category.md#yoneda-embedding) is [full and faithful](../../../category.md#full-and-faithful-functor), and $\mathcal A$ is equivalent to its [full subcategory](../../../category.md#full-subcategory) of [representable presheaves](../../../category.md#representable-functor). The indexing [category](../../../category.md) in the usual version is $\mathcal A^{\mathrm{op}}$, not necessarily a small category chosen independently of $\mathcal A$.

Local smallness makes the values $\mathcal A(B,A)$ [sets](../../../set.md); it does not make the collection of objects a set. For a large indexing category, the collection of [natural transformations](../../../category.md#natural-transformation) between arbitrary set-valued [functors](../../../category.md#functor) can itself be a proper class. For example, take the discrete category on the class of ordinals and the constant two-element functor. Its endomorphisms include an independently chosen function $\{0,1\}\to\{0,1\}$ at each ordinal. A small functor category cannot encode this collection without changing universes. The [Yoneda lemma](../../../category.md#yoneda-lemma) remains meaningful when the source is representable because the displayed bijection identifies its natural transformations with a set. It does not make the entire large functor category locally small.

Even for a [small category](../../../category.md#small-category), the representable image is usually a very special part of its [presheaf category](../../../category.md#presheaf-category). If $\mathcal A$ is the terminal category, its presheaf category is $\mathbf{Set}$, but its representable image consists only of a singleton. The presheaf category has all small [categorical limits](../../../category.md#categorical-limit) and [colimits](../../../category.md#colimit), whereas an arbitrary full subcategory need have almost none. The Yoneda embedding preserves existing limits because [representable functors](../../../category.md#representable-functor) preserve limits. It generally does not preserve colimits. For example, the coproduct of two singleton sets in [category of finite sets](../../../category.md#category-of-finite-sets) is a two-element set, but evaluating the proposed presheaf coproduct at a two-element set gives

$$
|(y1\amalg y1)(2)|=2,\qquad |y(1\amalg1)(2)|=4.
$$

The pointwise coproduct therefore leaves the representable image. Identifying which presheaves are representable, and which ambient constructions return to the original category, is precisely substantive [category theory](../../../category-theory.md).

The representation is nonetheless powerful. The [Yoneda lemma](../../../category.md#yoneda-lemma) replaces a morphism by all its probes, converts a [universal property](../../../category-theory.md#universal-property) into a [representation of a functor](../../../category.md#representation-of-a-functor), and makes the presheaf category a natural place to add formal [colimits](../../../category.md#colimit). A small presheaf category is the free [free cocompletion](../../../category.md#free-cocompletion) under small colimits: every presheaf is a colimit of representables indexed by its [category of elements](../../../category.md#category-of-elements). But this is a controlled enlargement of the category, not an identification of its original objects with all functors. The stronger conclusion in the proposed assertion therefore does not follow from the full-faithfulness statement.

## 3

↑ **Parent:** [Paper 21](paper-21.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

A [balanced category](../../../category.md#balanced-category) is one in which every [morphism](../../../algebra.md#morphism) that is both a [monomorphism](../../../category.md#monomorphism) and an [epimorphism](../../../category.md#epimorphism) is an [isomorphism](../../../algebra.md#isomorphism). A [strong monomorphism](../../../category.md#strong-monomorphism) $m:A\to B$ is a monomorphism right orthogonal to all epimorphisms: whenever $e:X\to Y$ is epic and $a:X\to A$, $b:Y\to B$ satisfy $ma=be$, there is a unique $d:Y\to A$ with $de=a$ and $md=b$. A [regular monomorphism](../../../category.md#regular-monomorphism) is an [equalizer](../../../category.md#equaliser) of some parallel pair of morphisms. Its equalizer property supplies the indicated lift after epic cancellation, so every regular monomorphism is strong.

If every monomorphism is strong and $m:A\to B$ is also epic, apply strongness to the square whose left and right sides are both $m$, with horizontal arrows $1_A$ and $1_B$. The lift $d:B\to A$ satisfies $dm=1_A$ and $md=1_B$. Thus $m$ is invertible and the [category](../../../category.md) is balanced.

Conversely, suppose the category is balanced and has [pullbacks in a category](../../../category.md#pullback-category-theory). Given the lifting square above, form $P=A\times_B Y$ with projections $p:P\to Y$, $q:P\to A$. The pair $(a,e)$ gives $h:X\to P$ with $ph=e$, $qh=a$. The pullback of the [monomorphism](../../../category.md#monomorphism) $m$ is monic, so $p$ is monic. It is also epic: $rp=sp$ implies $re=se$, hence $r=s$ because $e$ is epic. Balancedness makes $p$ invertible. Now $d=qp^{-1}$ satisfies both required equations, and monicity of $m$ proves uniqueness. Hence **in a balanced category with pullbacks, every monomorphism is strong**.

For the finite example, choose a strong monomorphism $m:A\to B$ that is not regular. It is not an isomorphism, since an isomorphism is the equalizer of an identical pair. It is not epic either, since an epic strong monomorphism is invertible by the first argument. Consequently there are distinct arrows $r,s:B\rightrightarrows D$ with $rm=sm$. Since $m$ is not the equalizer of this pair, there is a map $h:X\to B$ with $rh=sh$ that does not factor through $m$. Monicity rules out failure of uniqueness, so failure of existence is the only possible failure of its equalizer property.

Define $\mathcal C_0$ to have four formally distinct objects $a,b,x,d$ and exactly the following six nonidentity arrows:

$$
m_0:a\to b,\quad h_0:x\to b,\quad r_0,s_0:b\rightrightarrows d,\quad k_0:a\to d,\quad l_0:x\to d.
$$

Their only nontrivial composites are

$$
r_0m_0=s_0m_0=k_0,\qquad r_0h_0=s_0h_0=l_0.
$$

There are no longer composable strings of nonidentity arrows, so these rules define an associative [category](../../../category.md). Sending $a,b,x,d$ to $A,B,X,D$, respectively, and the six arrows to $m,h,r,s,rm,rh$, defines a [functor](../../../category.md#functor). It is a [faithful functor](../../../category.md#faithful-functor): every hom-set has at most one arrow except $\mathcal C_0(b,d)=\{r_0,s_0\}$, and their images are distinct. Faithfulness does not require the four image objects to be distinct.

The map $m_0$ is monic, by direct inspection of arrows into $a$. Neither $m_0$ nor $h_0$ is epic, since the distinct pair $r_0,s_0$ agrees after either. Every other nonidentity arrow has target $d$ and is epic, because there is only one arrow out of $d$. A lifting square against $m_0$ whose left side is one of these epimorphisms would require an arrow $d\to b$, which does not exist. Squares whose left side is an identity have the evident unique lift. Thus $m_0$ is a [strong monomorphism](../../../category.md#strong-monomorphism).

It is not a [regular monomorphism](../../../category.md#regular-monomorphism). The only distinct parallel pair out of $b$ is $r_0,s_0$, and $h_0$ equalizes it but has no factorization through $m_0$, since there is no arrow $x\to a$. An identical pair has $1_b$ as its equalizer and cannot have the noninvertible $m_0$ as its equalizer. Therefore

$$
\boxed{\mathcal C_0\text{ has four objects, six nonidentity arrows, and a strong nonregular monomorphism}.}
$$

## 4

↑ **Parent:** [Paper 21](paper-21.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Write $\eta:1_{\mathcal C}\to GF$ and $\varepsilon:FG\to1_{\mathcal D}$ for the [unit and counit of an adjunction](../../../category.md#unit-and-counit-of-an-adjunction). The induced [monad](../../../category-theory.md#monad) has

$$
T=GF,\qquad \mu=G\varepsilon F:T^2\to T.
$$

The [Eilenberg-Moore comparison functor](../../../category-theory.md#eilenberg-moore-comparison-functor) sends $D\in\mathcal D$ to the [algebra for a monad](../../../category-theory.md#algebra-for-a-monad)

$$
K(D)=(GD,G\varepsilon_D),
$$

and sends $v:D\to D'$ to $Gv$. The [triangle identities for an adjunction](../../../category.md#triangle-identities-for-an-adjunction) give the algebra unit law, and naturality of the counit gives the algebra multiplication law and the algebra-morphism equation for $Gv$.

If $\mathcal D$ has [coequalizers](../../../category.md#coequalizer), define the [Left adjoint to the Eilenberg-Moore comparison functor](../../../category-theory.md#left-adjoint-to-the-eilenberg-moore-comparison-functor) at an algebra $(A,a:TA\to A)$ by

$$
FTA\mathrel{\substack{\xrightarrow{Fa}\\[-2pt]\xrightarrow[\varepsilon_{FA}]{} }}FA\xrightarrow{q}L(A,a).
$$

The parallel pair is reflexive through $F\eta_A$. A [morphism](../../../algebra.md#morphism) $L(A,a)\to D$ is equivalently an arrow $b:FA\to D$ with $bFa=b\varepsilon_{FA}$. Under $F\dashv G$, its transpose is $\bar b=Gb\,\eta_A:A\to GD$. The transpose of $bFa$ is $\bar b\,a$, while the transpose of $b\varepsilon_{FA}$ is $G\varepsilon_D\,T\bar b$. Hence the coequalizer condition is exactly

$$
\bar b\,a=G\varepsilon_D\,T\bar b,
$$

the equation for a [morphism of algebras for a monad](../../../category-theory.md#morphism-of-algebras-for-a-monad) $(A,a)\to K(D)$. This supplies the natural bijection proving **$L\dashv K$**, and also defines $L$ on algebra morphisms by the coequalizer universal property.

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

Let $U_n:\mathcal C_{n+1}\to\mathcal C_n$ forget the last [partial unary operation](../../../function.md#partial-unary-operation). For an object $A$ of the [nested partial unary operation category](../../../category.md#nested-partial-unary-operation-category) $\mathcal C_n$, set

$$
S_n(A)=\{x\in A:\alpha_n(x)\text{ is defined and }\alpha_n(x)=x\}.
$$

The nesting rule implies that every earlier operation is defined and fixes such an $x$. To construct a [free extension of nested partial unary operations](../../../category.md#free-extension-of-nested-partial-unary-operations), adjoin a disjoint infinite chain for each $x\in S_n(A)$:

$$
L_nA=A\amalg\{(x,k):x\in S_n(A),\ k\in\mathbb N\}.
$$

Keep the old operations on $A$. On each new chain put $\alpha_1(x,k)=(x,k+1)$; every old operation $\alpha_i$ with $2\leq i\leq n$ is undefined there, because the first operation has no fixed points there. Define the new operation only on $S_n(A)$, by $\alpha_{n+1}(x)=(x,0)$. These are exactly the fixed points of the old top operation, so the required domain rule is satisfied. The inclusion $A\hookrightarrow U_nL_nA$ preserves all old defined operations.

For a [morphism](../../../algebra.md#morphism) $f:A\to U_nB$, preservation of the old operations makes $f(x)\in S_n(B)$ whenever $x\in S_n(A)$. Any extension to a morphism $\widehat f:L_nA\to B$ must have

$$
\widehat f(x,k)=\beta_1^k\bigl(\beta_{n+1}(f(x))\bigr),\qquad \widehat f|_A=f.
$$

The operation $\beta_{n+1}$ is defined at $f(x)$, and $\beta_1$ is total, so this formula exists. It preserves the new operation and the chain operation; there are no other defined operations on new points to check. It therefore gives the unique extension. Naturality and functoriality follow from uniqueness. Thus

$$
\boxed{\mathcal C_{n+1}(L_nA,B)\cong\mathcal C_n(A,U_nB),\qquad L_n\dashv U_n.}
$$

Notice the useful extra fact: the new top operation has no fixed points, since every value $(x,0)$ is new and every input $x$ is old. Hence freely adding any further operations adds no more points; those operations have empty domains.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Put $\mathcal C_0=\mathbf{Set}$. The initial free construction $L_0:\mathbf{Set}\to\mathcal C_1$ sends $A$ to $A\times\mathbb N$ with $\alpha_1(a,k)=(a,k+1)$. A [function](../../../function.md) $f:A\to UB$ extends uniquely by $(a,k)\mapsto\beta_1^k(f(a))$. Its induced [monad](../../../category-theory.md#monad) is $T_0A=A\times\mathbb N$, with unit $a\mapsto(a,0)$ and multiplication $(a,k,l)\mapsto(a,k+l)$. An [algebra for a monad](../../../category-theory.md#algebra-for-a-monad) is determined by the action of $1\in\mathbb N$, so its [Eilenberg-Moore category](../../../category-theory.md#eilenberg-moore-category) is $\mathcal C_1$. Thus this first free–forgetful adjunction is a [monadic adjunction](../../../category-theory.md#monadic-adjunction) without needing the given assumption for $n=0$.

The [monadic length](../../../category-theory.md#monadic-length) counts successive [Eilenberg-Moore comparison functor](../../../category-theory.md#eilenberg-moore-comparison-functor) steps until the comparison becomes an equivalence. Fix $0\leq m<n$. For $m\geq1$, the free construction in the preceding part adds the $(m+1)$st operation with no fixed points. For $m=0$, the free first operation also has no fixed points. Consequently the [left adjoint](../../../category.md#adjoint-functors) $F_{n,m}$ to the composite forgetful functor $U_{n,m}:\mathcal C_n\to\mathcal C_m$ is obtained by the one-step free construction, followed by empty higher operations. In particular, its underlying object of $\mathcal C_m$, unit and multiplication are exactly those of the one-step adjunction:

$$
U_{n,m}F_{n,m}=U_mL_m=T_m
$$

as [monads](../../../category-theory.md#monad), not merely as object functions. The multiplication agrees because both counits evaluate the same first new operation and the same chains; no later operation has a value on a free object.

By the assumed one-step [monadic adjunction](../../../category-theory.md#monadic-adjunction) property, or the explicit argument above when $m=0$, the [Eilenberg-Moore category](../../../category-theory.md#eilenberg-moore-category) $\mathcal C_m^{T_m}$ is equivalent to $\mathcal C_{m+1}$. Under this equivalence the comparison $\mathcal C_n\to\mathcal C_m^{T_m}$ is precisely $U_{n,m+1}$. Indeed, its algebra action evaluates each newly adjoined chain using $\alpha_1$, and evaluates the first new value using $\alpha_{m+1}$; it retains that operation and ignores all higher ones. The comparison has a left adjoint by the same explicit free extension. Thus the whole [monadic tower for nested partial unary operations](../../../category-theory.md#monadic-tower-for-nested-partial-unary-operations) is

$$
\mathbf{Set}=\mathcal C_0,\quad\mathcal C_1,\quad\ldots,\quad\mathcal C_n,
$$

with the remaining comparison at stage $m$ equal to $U_{n,m}$, and stage $n$ the identity.

It does not terminate earlier. If $m<n$, take the same underlying two-element [set](../../../set.md) in two objects of $\mathcal C_n$, making every operation up to $m$ the identity. In the first object make all remaining operations identities; in the second make $\alpha_{m+1}$ exchange the two elements, and leave all subsequent operations undefined. Both satisfy the nesting rule. The identity function is a morphism after forgetting to $\mathcal C_m$, but is not a morphism between the original objects. Thus $U_{n,m}$ is not a [full functor](../../../category.md#full-functor), and cannot be an equivalence. Therefore

$$
\boxed{\operatorname{monadic\ length}(\mathcal C_n\to\mathbf{Set})=n.}
$$

## 5

↑ **Parent:** [Paper 21](paper-21.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Let $F:\mathcal C\to\mathcal D$ be a [final functor](../../../category.md#final-functor), and let $\lambda_c:GFc\to V$ be a [cocone under a diagram](../../../category.md#cocone-under-a-diagram) $GF$. For $d\in\mathcal D$, choose an object $(c,a:d\to Fc)$ of the nonempty [comma category](../../../category.md#comma-category) $(d\downarrow F)$ and define

$$
\bar\lambda_d=\lambda_c\,G(a):Gd\to V.
$$

If $t:(c,a)\to(c',a')$ is a [morphism](../../../algebra.md#morphism) in that comma category, then $Ft\,a=a'$, so the cocone equation gives $\lambda_cG(a)=\lambda_{c'}G(Ft)G(a)=\lambda_{c'}G(a')$. Equality also holds along a reversed arrow, and hence along any zigzag. Connectedness makes the definition independent of the chosen object. For $v:d\to d'$, use $(c,a:d'\to Fc)$ and $(c,av:d\to Fc)$ to obtain $\bar\lambda_d=\bar\lambda_{d'}Gv$. Thus $\bar\lambda$ is a cocone under $G$. Taking $(c,1_{Fc})$ shows that it extends $\lambda$.

Every extension must satisfy $\bar\lambda_d=\lambda_cG(a)$ by its cocone equation, proving uniqueness. The construction commutes with postcomposition by a [morphism](../../../algebra.md#morphism) $V\to V'$. Hence restriction gives a natural bijection between the [sets](../../../set.md) of cocones of $G$ and $GF$ with any fixed vertex. A universal cocone for $GF$ therefore extends to a universal cocone for $G$. In particular,

$$
\boxed{\operatorname{colim}_{\mathcal D}G\cong\operatorname{colim}_{\mathcal C}GF,}
$$

whenever the latter exists, and existence of all [colimits](../../../category.md#colimit) of shape $\mathcal C$ implies existence of all colimits of shape $\mathcal D$.

For the factorization of an arbitrary [functor](../../../category.md#functor) $H:\mathcal C\to\mathcal E$, let

$$
P(e)=\pi_0(e\downarrow H),
$$

the [set](../../../set.md) of [connected components of a category](../../../category.md#connected-component-of-a-category), where components are defined by finite zigzags. Precomposition by $v:e\to e'$ gives a [functor](../../../category.md#functor) $(e'\downarrow H)\to(e\downarrow H)$ and therefore a map $P(v):P(e')\to P(e)$. Identity and composition laws make $P$ a [categorical presheaf](../../../category.md#presheaf-category-theory). This is a set-valued construction when the relevant comma categories are small or have only a set of components, as in the usual small-category convention for this factorization.

Take $\mathcal D$ to be the [category of elements](../../../category.md#category-of-elements) of this presheaf. Its objects are pairs $(e,S)$ with $S\in P(e)$; a morphism $(e,S)\to(e',S')$ is an arrow $v:e\to e'$ satisfying $P(v)(S')=S$. Define $G:\mathcal D\to\mathcal E$ by forgetting $S$. Given $v:e\to e'$ and an object $(e',S')$, the unique lift into that object has source $(e,P(v)(S'))$ and underlying arrow $v$. This proves that $G$ is a [discrete fibration](../../../category.md#discrete-fibration).

Define $F(c)=(Hc,[(c,1_{Hc})])$. For $t:c\to c'$, take $F(t)=Ht$. The arrow $t$ in $(Hc\downarrow H)$ joins $(c,1_{Hc})$ to $(c',Ht)$, so the required component equation holds. It follows that $F$ is a functor and $GF=H$.

Finally, an object of $((e,S)\downarrow F)$ is a pair $(c,v:e\to Hc)$ whose component in $(e\downarrow H)$ is $S$. Its morphisms are exactly the morphisms of that comma category between objects in $S$. Consequently $((e,S)\downarrow F)$ is precisely the full connected component $S$, and is nonempty and connected. Thus $F$ is final, and **every such functor factors as a final functor followed by a discrete fibration**.

## 6

↑ **Parent:** [Paper 21](paper-21.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

A [regular category](../../../category.md#regular-category) has [finite limits](../../../category.md#finite-limit), [coequalizers](../../../category.md#coequalizer) of [kernel pairs](../../../category.md#kernel-pair), and [regular epimorphisms](../../../category.md#regular-epimorphism) stable under pullback. Equivalently, every morphism factors as a regular epimorphism followed by a monomorphism, and these factorizations are stable under pullback. A [regular functor](../../../category.md#regular-functor) preserves finite limits and regular epimorphisms, hence also preserves these [image factorizations](../../../category.md#image-factorization).

For this question, the [capital regular category](../../../category.md#capital-regular-category) convention is the one in which every [well-supported object](../../../category.md#well-supported-object) is a [well-pointed object in a category](../../../category.md#well-pointed-object-in-a-category). Here an object $A$ is well-supported if $A\to1$ is a regular epimorphism. It is well-pointed if a [subobject](../../../category.md#subobject) $m:B\hookrightarrow A$ through which every point $1\to A$ factors must be the whole object. This convention is documented in [Definitions 1.1–1.3](https://www2.math.ethz.ch/EMIS/journals/TAC/volumes/16/31/16-31.pdf). It imposes no such point-detection requirement on objects whose support is a proper subobject of $1$. In particular, it should not be replaced here by the stronger assertion that $\mathcal A(1,-)$ reflects every isomorphism.

First prove two facts about a capital regular category $\mathcal A$. Every well-supported object $A$ has a point. Otherwise $A\times A$ is well-supported and has no points, so its diagonal $A\hookrightarrow A\times A$ contains all points and is invertible. That makes $A$ a [subterminal object](../../../category.md#subterminal-object); the regular epimorphism $A\to1$ is then also monic and hence invertible, contradicting the absence of a point. If $e:X\to Y$ is a regular epimorphism and $y:1\to Y$ is a point, its [pullback in a category](../../../category.md#pullback-category-theory) is a well-supported object over $1$, so it has a point lifting $y$. Thus the [representable functor](../../../category.md#representable-functor)

$$
\Gamma=\mathcal A(1,-):\mathcal A\to\mathbf{Set}
$$

preserves regular epimorphisms; it already preserves all existing limits. Hence **$\Gamma$ is a regular functor**. Second, if $\Gamma X$ is a singleton, its unique point $x:1\to X$ is a monomorphism, $X$ is well-supported, and $x$ contains all points of $X$. Well-pointedness makes $x$ invertible. Thus $\Gamma$ reflects terminal objects, even though it need not reflect arbitrary isomorphisms.

Now let $\mathcal C$ be a [small category](../../../category.md#small-category) that is a [regular category](../../../category.md#regular-category). For each object $B$, its [slice category](../../../category.md#slice-category) $\mathcal C/B$ is small and regular: finite limits, images and the stability of regular epimorphisms are computed using the corresponding constructions in $\mathcal C$. By the permitted capitalization result choose a [conservative functor](../../../category.md#conservative-functor) that is regular,

$$
J_B:\mathcal C/B\to\mathcal A_B,
$$

with $\mathcal A_B$ a small capital regular category. The base-change functor $B^*:\mathcal C\to\mathcal C/B$, given by $X\mapsto(X\times B\to B)$, preserves finite limits and regular epimorphisms. So does

$$
R_B=\Gamma_BJ_BB^*:\mathcal C\to\mathbf{Set}.
$$

Taking these as the coordinates defines a regular functor

$$
R:\mathcal C\to\mathbf{Set}^{\operatorname{ob}\mathcal C}.
$$

The exponent is a [set](../../../set.md) of indices, so this is a power of the [Category of sets](../../../category.md#category-of-sets), with finite limits and regular epimorphisms computed coordinatewise.

To prove reflection of isomorphisms, suppose $R(f)$ is invertible for $f:A\to B$. In $\mathcal C/B$, the object $(A,f)$ is the pullback of $B^*f:(A\times B\to B)\to(B\times B\to B)$ along the point given by the diagonal $B\to B\times B$. Applying $\Gamma_BJ_B$ shows that $\Gamma_BJ_B(A,f)$ is the fibre of the bijection $R_B(f)$ over this diagonal point, and is a singleton. The preceding lemma gives $J_B(A,f)\cong1$ through its canonical arrow to $1$. Since $J_B$ reflects isomorphisms, $(A,f)\to(B,1_B)$ is invertible. Its underlying morphism is $f$. Therefore

$$
\boxed{R:\mathcal C\to\mathbf{Set}^{\operatorname{ob}\mathcal C}\text{ is regular and reflects isomorphisms}.}
$$

In the small-category setting of this representation result, the elementary condition for replacing the power by one copy of $\mathbf{Set}$ is:

$$
\boxed{\text{Every object is either well-supported or a strict initial object}.}
$$

This is [almost total support for a regular category](../../../category.md#almost-total-support-for-a-regular-category). “Strict initial” means initial and every arrow into it is invertible; the condition allows the case in which all objects are well-supported and no initial object exists.

For necessity, let $V:\mathcal C\to\mathbf{Set}$ be regular and conservative. If $VA\ne\varnothing$, factor $A\to1$ through its [support of an object in a regular category](../../../category.md#support-of-an-object-in-a-regular-category) $S\hookrightarrow1$. Preservation of images gives $VS=1$. Conservativity makes $S\to1$ invertible, so $A$ is well-supported. If $VA=\varnothing$, then for every $X$ the projection $A\times X\to A$ is sent to the bijection $\varnothing\to\varnothing$, hence is invertible. Its inverse followed by the other projection supplies an arrow $A\to X$. For any two such arrows, their equalizer is sent to a bijection onto $VA$, hence is invertible, proving uniqueness. Thus $A$ is initial. If $X\to A$ exists, then $VX\to\varnothing$ exists, so $VX=\varnothing$ and that arrow is sent to a bijection. Conservativity makes it invertible. Hence $A$ is strict initial.

For sufficiency, choose the permitted conservative regular functor $J:\mathcal C\to\mathcal A$ into a small capital regular category, and put $V=\Gamma J$. This is regular. A well-supported object of $\mathcal C$ is sent to a well-supported object of $\mathcal A$, which has a point. A non-well-supported object is strict initial by the condition, and is consequently a proper subterminal object. The functor $J$ preserves subterminality and reflects the noninvertibility of its arrow to $1$; its image is a proper subterminal object and has no points. Thus $VA$ is empty exactly on the non-well-supported objects.

Suppose $Vf$ is a bijection for $f:A\to B$. If both sets are empty, $A$ and $B$ are strict initial objects and $f$ is invertible. Otherwise $A,B$ are well-supported. Factor $Jf$ as a regular epimorphism followed by a monomorphism $m:I\hookrightarrow JB$. Surjectivity of $Vf$ makes every point of $JB$ factor through $m$; capitality of $\mathcal A$ makes $m$ invertible. Hence $Jf$ is a regular epimorphism. Its kernel pair $P=JA\times_{JB}JA$ is well-supported, because $P\to JA$ and $JA\to1$ are regular epimorphisms. Injectivity of $Vf$ implies that every point of $P$ has equal coordinates, and therefore factors through the diagonal $JA\hookrightarrow P$. Since $P$ is well-pointed, this diagonal is invertible. Thus $Jf$ is also monic, hence an isomorphism, and conservativity of $J$ makes $f$ invertible. This proves sufficiency with actual point and image arguments, rather than asserting that global sections of every capital regular category is conservative.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2010](../../2010.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
