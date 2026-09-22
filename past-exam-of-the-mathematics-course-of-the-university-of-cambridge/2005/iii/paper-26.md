# Paper 26

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper26.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper26.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [Solution](#6/solution)

## 1

↑ **Parent:** [Paper 26](paper-26.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

A [monad](../../../category-theory.md#monad) on a [category](../../../category.md) $\mathcal C$ consists of an [endofunctor](../../../category.md#endofunctor) $T$, a unit [natural transformation](../../../category.md#natural-transformation) $\eta:1_{\mathcal C}\Rightarrow T$, and a multiplication $\mu:T^2\Rightarrow T$, satisfying

$$
\mu\,T\mu=\mu\,\mu T,\qquad \mu\,T\eta=1_T=\mu\,\eta T.
$$

An [algebra for a monad](../../../category-theory.md#algebra-for-a-monad) is $(A,a:TA\to A)$ with $a\eta_A=1_A$ and $aTa=a\mu_A$. A [morphism of algebras for a monad](../../../category-theory.md#morphism-of-algebras-for-a-monad) $h:(A,a)\to(B,b)$ satisfies $ha=bTh$. These objects and arrows form the [Eilenberg-Moore category](../../../category-theory.md#eilenberg-moore-category) $\mathcal C^T$.

For an [adjunction](../../../category.md#adjoint-functors) $F:\mathcal C\rightleftarrows\mathcal D:U$ with $F\dashv U$, the [monad induced by an adjunction](../../../category-theory.md#monad-induced-by-an-adjunction) is $T=UF$, with $\mu=U\varepsilon F$. The [Eilenberg-Moore comparison functor](../../../category-theory.md#eilenberg-moore-comparison-functor) is $K(D)=(UD,U\varepsilon_D)$ and $K(h)=Uh$. The [functor](../../../category.md#functor) $U$ is monadic when this comparison is an [equivalence of categories](../../../category.md#equivalence-of-categories); this is a [monadic adjunction](../../../category-theory.md#monadic-adjunction).

The [precise monadicity theorem](../../../category-theory.md#beck-s-monadicity-theorem) says that $U:\mathcal D\to\mathcal C$ is monadic exactly when it has a [left adjoint](../../../category.md#adjoint-functors), reflects [isomorphisms](../../../algebra.md#isomorphism), and satisfies the following condition: whenever the image of a parallel pair in $\mathcal D$ admits a [split coequalizer](../../../category.md#split-coequalizer) in $\mathcal C$, the pair has a [coequalizer](../../../category.md#coequalizer) in $\mathcal D$ and $U$ preserves that [coequalizer](../../../category.md#coequalizer). Equivalently, these [coequalizers](../../../category.md#coequalizer) are created up to the canonical [isomorphism](../../../algebra.md#isomorphism) identifying their underlying [coequalizer](../../../category.md#coequalizer) objects. Here a [split coequalizer](../../../category.md#split-coequalizer) of $f,g:A\rightrightarrows B$ consists of $q:B\to Q$, $s:Q\to B$, and $t:B\to A$ with

$$
qf=qg,\qquad qs=1_Q,\qquad ft=1_B,\qquad gt=sq.
$$

These equations prove its [universal property](../../../category-theory.md#universal-property): if $hf=hg$, then $h=hft=hgt=hsq$, and $hs$ is the unique factor through $q$. Every [functor](../../../category.md#functor) preserves these equations, so every [functor](../../../category.md#functor) preserves [split coequalizers](../../../category.md#split-coequalizer).

First consider the forgetful [functor](../../../category.md#functor) $U^T:\mathcal C^T\to\mathcal C$. It has the [free algebra functor](../../../category-theory.md#free-algebra-functor) $A\mapsto(TA,\mu_A)$ as a [left adjoint](../../../category.md#adjoint-functors): the inverse transposition formulas are $h\mapsto h\eta_A$ and $v\mapsto bTv$. An [monad algebra morphism](../../../category-theory.md#morphism-of-algebras-for-a-monad) whose underlying arrow is invertible has an algebra-morphism inverse, by rearranging its structure equation. Thus $U^T$ reflects [isomorphisms](../../../algebra.md#isomorphism).

Suppose $f,g:(A,a)\rightrightarrows(B,b)$ have an underlying [split coequalizer](../../../category.md#split-coequalizer) $q:B\to Q$. Applying $T$ gives a [coequalizer](../../../category.md#coequalizer) of $Tf,Tg$. The equation $qbTf=qfa=qga=qbTg$ therefore gives a unique $c:TQ\to Q$ with $cTq=qb$. The [monad algebra](../../../category-theory.md#algebra-for-a-monad) laws follow by cancellation: composing $c\eta_Q=1_Q$ with the [epimorphism](../../../category.md#epimorphism) $q$ reduces it to $b\eta_B=1_B$, and composing $cTc=c\mu_Q$ with $T^2q$ reduces it to $bTb=b\mu_B$. Both $Tq$ and $T^2q$ are [epimorphisms](../../../category.md#epimorphism) because they remain split [coequalizers](../../../category.md#coequalizer). Thus $(Q,c)$ is an [algebra for a monad](../../../category-theory.md#algebra-for-a-monad) and $q$ is an [monad algebra morphism](../../../category-theory.md#morphism-of-algebras-for-a-monad). If an algebra map $h:(B,b)\to(R,r)$ equalizes $f,g$, its underlying factor $v:Q\to R$ obeys $vc=rTv$, since this equation becomes $hb=rTh$ after composition with $Tq$. This proves that $U^T$ creates the required [coequalizers](../../../category.md#coequalizer). An [equivalence of categories](../../../category.md#equivalence-of-categories) transfers these properties to any monadic $U$, proving necessity.

Conversely assume the three conditions and write $T=UF$. Given $(A,a)\in\mathcal C^T$, take the pair

$$
FTA\mathrel{\substack{\xrightarrow{\varepsilon_{FA}}\\[-2pt]\xrightarrow[Fa]{}}}FA.
$$

Its image is $\mu_A,Ta:T^2A\rightrightarrows TA$, with [split coequalizer](../../../category.md#split-coequalizer) $a:TA\to A$: the splittings are $s=\eta_A$ and $t=\eta_{TA}$, because

$$
a\eta_A=1_A,\qquad \mu_A\eta_{TA}=1_{TA},\qquad Ta\,\eta_{TA}=\eta_Aa.
$$

Let $q:FA\to D_a$ be its [coequalizer](../../../category.md#coequalizer) in $\mathcal D$. Preservation gives a canonical [isomorphism](../../../algebra.md#isomorphism) $UD_a\cong A$ under which $Uq=a$. Transporting the algebra action of $K(D_a)$ along this [isomorphism](../../../algebra.md#isomorphism) gives $\alpha:TA\to A$. Naturality of the [adjunction counit](../../../category.md#counit-of-an-adjunction) says that $K(q)$ is an [monad algebra morphism](../../../category-theory.md#morphism-of-algebras-for-a-monad), hence $\alpha Ta=a\mu_A$. But $aTa=a\mu_A$ too, and $Ta$ is a [split epimorphism](../../../category.md#split-epimorphism), with section $T\eta_A$. Therefore $\alpha=a$. Every algebra is consequently isomorphic to some $K(D_a)$.

It remains to establish full faithfulness, rather than merely construct objects. For $B\in\mathcal D$, put $b=U\varepsilon_B$. The [adjunction counit](../../../category.md#counit-of-an-adjunction) $\varepsilon_B:FUB\to B$ coequalizes $\varepsilon_{FUB},Fb$. The [coequalizer](../../../category.md#coequalizer) supplied by the hypothesis has underlying [coequalizer](../../../category.md#coequalizer) $b:TUB\to UB$. The induced arrow from that [coequalizer](../../../category.md#coequalizer) object to $B$ is therefore sent by $U$ to an [isomorphism](../../../algebra.md#isomorphism); reflection of [isomorphisms](../../../algebra.md#isomorphism) makes it invertible. Thus $\varepsilon_B$ itself is this [coequalizer](../../../category.md#coequalizer).

Now let $h:K(B)\to K(C)$ be an [monad algebra morphism](../../../category-theory.md#morphism-of-algebras-for-a-monad), and put $c=U\varepsilon_C$. The arrow $v=\varepsilon_CFh:FUB\to C$ coequalizes the two arrows in the preceding presentation. To check this directly, use transposition along $F\dashv U$: the transposes of $vFb$ and $v\varepsilon_{FUB}$ are respectively $hb$ and $cTh$, which agree by the algebra-morphism equation. Hence a unique $\bar h:B\to C$ satisfies $\bar h\varepsilon_B=v$. Applying $U$ gives $(U\bar h)b=cTh=hb$; cancellation of the [split epimorphism](../../../category.md#split-epimorphism) $b$ yields $U\bar h=h$. Finally, any arrow $r:B\to C$ satisfies $r\varepsilon_B=\varepsilon_CFU r$ by naturality, so two arrows with equal image under $U$ are equal by the [coequalizer](../../../category.md#coequalizer) property. The comparison is [full and faithful](../../../category.md#full-and-faithful-functor) and essentially surjective, hence an [equivalence of categories](../../../category.md#equivalence-of-categories). This proves the theorem.

For the application, the free [compact Hausdorff space](../../../topology.md#compact-hausdorff-space) on a [set](../../../set.md) $S$ is the [Stone-Čech compactification](../../../physics.md#stone-cech-compactification) $\beta(S_{\mathrm{disc}})$ of the corresponding [discrete space](../../../topology.md#discrete-space). Its standard extension property says that every set map $S\to UX$, for compact Hausdorff $X$, extends uniquely to a [continuous map](../../../topology.md#continuous-map) $\beta S\to X$. This constructs the required [left adjoint](../../../category.md#adjoint-functors). Also a continuous bijection from a compact space to a Hausdorff space is a [homeomorphism](../../../topology.md#homeomorphism), so $U$ reflects [isomorphisms](../../../algebra.md#isomorphism).

Take [continuous maps](../../../topology.md#continuous-map) $f,g:X\rightrightarrows Y$ whose underlying functions have a [split coequalizer](../../../category.md#split-coequalizer) $q:Y\to Q$ with splittings $s,t$. The splittings need not be continuous. Let

$$
E=\{(f(x),g(x)):x\in X\}\subseteq Y\times Y,\qquad R=\{(y,z):q(y)=q(z)\}.
$$

The set $E$ is compact and hence closed. Since $qf=qg$, it is contained in $R$. Conversely $(y,sq(y))=(ft(y),gt(y))\in E$. Thus

$$
R=\{(y,z):\exists w\in Y,\ (y,w)\in E,\ (z,w)\in E\}.
$$

The set of triples on the right is closed in the [compact Hausdorff space](../../../topology.md#compact-hausdorff-space) $Y^3$, so its projection onto the first two coordinates is compact and closed. This proves that the [equivalence relation](../../../set-theory.md#equivalence-relation) $R$ is closed, without assuming continuity of either splitting.

Give $Q\cong Y/R$ the [quotient topology](../../../topology.md#quotient-topology). The allowed closed-relation criterion makes it a [compact Hausdorff space](../../../topology.md#compact-hausdorff-space). If a [continuous map](../../../topology.md#continuous-map) $h:Y\to Z$ equalizes $f,g$, the split-coequalizer property makes it constant on the fibres of $q$; its unique factor $Q\to Z$ is continuous by the quotient [topology](../../../topology.md). Hence this is a [coequalizer](../../../category.md#coequalizer) in [compact Hausdorff spaces](../../../topology.md#compact-hausdorff-space), preserved by $U$. Its [topology](../../../topology.md) is forced uniquely, since any continuous surjection from a compact space to a Hausdorff space is a quotient map. All three conditions hold, and therefore **the forgetful functor from compact Hausdorff spaces to sets is monadic**.

## 2

↑ **Parent:** [Paper 26](paper-26.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

**An essay arguing against the claim.** A good [definition](../../../mathematical-logic.md#definition-mathematics) can change which mathematical questions are visible. Nevertheless, I would argue that [category theory](../../../category-theory.md) derives its explanatory force from the interaction between definitions and theorems; there is no sound general ordering in which definitions contribute more than theorems.

The strongest case for the contrary view comes from [universal properties](../../../category-theory.md#universal-property). A [product in a category](../../../category.md#product-category-theory) is characterized by maps into it, rather than by a particular construction of ordered pairs. The same definition applies to [sets](../../../set.md), [groups](../../../group.md), and [topological spaces](../../../topology.md#topological-space). An [adjunction](../../../category.md#adjoint-functors) goes further: its natural correspondence of arrows puts free constructions, quotient constructions, and several kinds of completion into a common language. Such definitions remove irrelevant choices and expose relationships that would be difficult to recognize from separate constructions.

But a universal-property definition does not supply an object. The [definition](../../../mathematical-logic.md#definition-mathematics) of a [product in a category](../../../category.md#product-category-theory) says what a product would accomplish; an existence theorem says whether the category actually has one. Even uniqueness up to unique [isomorphism](../../../algebra.md#isomorphism) is a short proof, not an extra clause to be silently supplied by the word “universal”. Given two products, their [universal properties](../../../category-theory.md#universal-property) produce maps in both directions, and uniqueness forces the two composites to be identities. This elementary theorem makes the definition usable independently of a chosen construction.

The [Yoneda lemma](../../../category.md#yoneda-lemma) illustrates the distinction especially clearly. A [representable functor](../../../category.md#representable-functor) is a definition, but the lemma proves that its [natural transformations](../../../category.md#natural-transformation) into any set-valued [functor](../../../category.md#functor) are determined by one element. Its proof evaluates at the identity and reconstructs the whole transformation by functoriality. Consequently the [Yoneda embedding](../../../category.md#yoneda-embedding) is [full and faithful](../../../category.md#full-and-faithful-functor): an object's pattern of incoming arrows recovers its morphisms without loss. That is a substantive explanation of why the chosen definition is powerful. Merely calling a [functor](../../../category.md#functor) representable would not establish it.

Similarly, defining a [monadic adjunction](../../../category-theory.md#monadic-adjunction) gives a precise meaning to recovering structured objects as [algebras for a monad](../../../category-theory.md#algebra-for-a-monad). It does not decide whether a given [forgetful functor](../../../category.md#forgetful-functor) is monadic. The [precise monadicity theorem](../../../category-theory.md#beck-s-monadicity-theorem) translates that difficult classification into a usable test involving [adjoint functors](../../../category.md#adjoint-functors), reflected [isomorphisms](../../../algebra.md#isomorphism), and specific [coequalizers](../../../category.md#coequalizer). For [compact Hausdorff spaces](../../../topology.md#compact-hausdorff-space), the crucial step is proving that a set-split relation is closed. The definition of a [monad](../../../category-theory.md#monad) alone does not contain this topological argument. The theorem connects the algebraic language to an independently meaningful class of spaces.

There is also a danger in praising definitions without hypotheses. A [Cartesian closed category](../../../category.md#cartesian-closed-category) has [exponential objects](../../../category.md#exponential-object), but a category of structured objects need not be cartesian closed merely because underlying sets have function sets. The correct exponential in a [functor category](../../../category.md#functor-category) generally involves [natural transformations](../../../category.md#natural-transformation) out of [representable functors](../../../category.md#representable-functor), not pointwise function sets. Its existence and [universal property](../../../category-theory.md#universal-property) require an argument. Theorems also reveal when tempting definitions cannot support the intended construction.

Definitions provide the vocabulary and select the structures worth studying; proofs establish existence, consequences, and limitations. Category theory makes this partnership unusually explicit because its definitions are often expressed through [universal properties](../../../category-theory.md#universal-property). **Its distinctive achievement is to turn well-chosen definitions into reusable theorems, rather than to make theorems secondary.**

**An alternative essay arguing for the claim.** In [category theory](../../../category-theory.md), theorems are indispensable, but a carefully chosen [definition](../../../mathematical-logic.md#definition-mathematics) often performs the greater act of organization. It identifies what many apparently unrelated constructions have in common and makes whole families of proofs possible. In that explanatory sense, definitions can be the subject's most influential contributions.

Consider a [universal property](../../../category-theory.md#universal-property). Describing a [product in a category](../../../category.md#product-category-theory) as an object representing pairs of incoming arrows replaces several different concrete constructions by one invariant pattern. The corresponding uniqueness proof is important but short; the lasting insight is that the same pattern is the right question in every category. Once the definition is available, it becomes meaningful to ask which [functors](../../../category.md#functor) preserve products, whether the products exist in a new category, and how they interact with other universal constructions.

An [adjunction](../../../category.md#adjoint-functors) is an even more striking example. The existence of free [groups](../../../group.md), free [modules](../../../module-theory.md#module-mathematics), and a [Stone-Čech compactification](../../../physics.md#stone-cech-compactification) can be proved separately. The definition of an [adjunction](../../../category.md#adjoint-functors) recognizes their common relation to [forgetful functors](../../../category.md#forgetful-functor) and explains why arrows out of a free object are determined by arrows out of its generators. It also packages the relation as a [monad](../../../category-theory.md#monad). A large collection of isolated existence results becomes an instance of a shared structure, with reusable consequences about composition and [categorical limits](../../../category.md#categorical-limit).

A valuable definition also has to distinguish structures rather than merely rename them. An [abelian category](../../../category-theory.md#abelian-category) is not just an [additive category](../../../category-theory.md#additive-category) with [categorical kernels](../../../category.md#kernel-in-a-category) and [categorical cokernels](../../../category.md#cokernel-in-a-category): normality of [monomorphisms](../../../category.md#monomorphism) and [epimorphisms](../../../category.md#epimorphism) matters. The additive example with truncated primary torsion shows why those clauses belong in the definition. The definition therefore preserves exactly the structure on which theorems about images and exact sequences depend.

This view does not make proofs dispensable. The [Yoneda lemma](../../../category.md#yoneda-lemma) justifies the use of [representable functors](../../../category.md#representable-functor), and the [precise monadicity theorem](../../../category-theory.md#beck-s-monadicity-theorem) tests when a proposed algebraic description is valid. Rather, it argues that the best categorical definitions have unusually broad explanatory reach: they select the invariant structures to which those proofs apply. **If “matter more” means providing the reusable framework in which many theorems become instances of one idea, category-theoretic definitions have a strong claim to that role.**

## 3

↑ **Parent:** [Paper 26](paper-26.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For a locally small [category](../../../category.md) $\mathcal C$, an object $A$, and a [functor](../../../category.md#functor) $F:\mathcal C\to\mathbf{Set}$, the covariant form of the [Yoneda lemma](../../../category.md#yoneda-lemma) is the natural [bijection](../../../function.md#bijection)

$$
\operatorname{Nat}(\mathcal C(A,-),F)\cong F(A),\qquad \alpha\longmapsto\alpha_A(1_A).
$$

For $x\in F(A)$ define $\alpha^x_B(f)=F(f)(x)$, where $f:A\to B$. For $u:B\to D$, functoriality gives $F(u)\alpha^x_B(f)=F(uf)(x)=\alpha^x_D(uf)$, so this is a [natural transformation](../../../category.md#natural-transformation). Conversely, naturality of $\alpha$ at $f:A\to B$ gives $\alpha_B(f)=F(f)\alpha_A(1_A)$. The two constructions are inverse. They are natural in $F$, because a [natural transformation](../../../category.md#natural-transformation) $F\Rightarrow G$ commutes with evaluation. They are also natural in $A$: an arrow $v:A'\to A$ induces $\mathcal C(A,-)\to\mathcal C(A',-)$ by precomposition, and the resulting map $\operatorname{Nat}(\mathcal C(A',-),F)\to\operatorname{Nat}(\mathcal C(A,-),F)$ corresponds to $F(v):F(A')\to F(A)$. Applying the result to the [opposite category](../../../category.md#opposite-category) gives $\operatorname{Nat}(\mathcal C(-,A),H)\cong H(A)$ for $H:\mathcal C^{\mathrm{op}}\to\mathbf{Set}$.

Now let $\mathcal C$ be a [small category](../../../category.md#small-category), and let $F,G:\mathcal C\to\mathbf{Set}$. Finite [products in a category](../../../category.md#product-category-theory) in $[\mathcal C,\mathbf{Set}]$ exist pointwise; the terminal [functor](../../../category.md#functor) is the constant singleton [functor](../../../category.md#functor). Define the [exponential of covariant set-valued functors](../../../category.md#exponential-of-covariant-set-valued-functors) by

$$
(G^F)(C)=\operatorname{Nat}(\mathcal C(C,-)\times F,G).
$$

Smallness ensures that these [natural transformations](../../../category.md#natural-transformation) form a set. For $u:C\to D$, define $(G^F)(u)(\alpha)$ at $E$ by

$$
\bigl((G^F)(u)(\alpha)\bigr)_E(v,x)=\alpha_E(vu,x),\qquad v:D\to E.
$$

Precomposition respects identities and composition, so this defines a [functor](../../../category.md#functor). Its [evaluation map of an exponential object](../../../category.md#evaluation-map-of-an-exponential-object) is

$$
\mathrm{ev}_C:(G^F)(C)\times F(C)\to G(C),\qquad (\alpha,x)\mapsto\alpha_C(1_C,x).
$$

To check naturality, for $u:C\to D$ both sides give $\alpha_D(u,F(u)x)$: one side uses naturality of $\alpha$, and the other uses the defining action of $G^F$.

Here is the full [universal property](../../../category-theory.md#universal-property). Given $\theta:H\times F\Rightarrow G$, define $\widehat\theta:H\Rightarrow G^F$ by

$$
\bigl(\widehat\theta_C(h)\bigr)_D(v,x)=\theta_D(H(v)h,x),\qquad v:C\to D.
$$

For $w:D\to E$, naturality of $\theta$ makes this commute with $G(w)$, so $\widehat\theta_C(h)$ is a [natural transformation](../../../category.md#natural-transformation). Replacing $h$ by $H(u)h$ is the same as precomposing $v$ by $u$, proving naturality in $C$. Conversely, $\beta:H\Rightarrow G^F$ gives $\theta_C(h,x)=\beta_C(h)_C(1_C,x)$. Starting with $\theta$ recovers it immediately. Starting with $\beta$, its naturality at $v:C\to D$ yields

$$
\beta_D(H(v)h)_D(1_D,x)=\beta_C(h)_D(v,x),
$$

so it too is recovered. The formulas are natural in $H$ and $G$, giving the required [adjunction](../../../category.md#adjoint-functors) $(-)\times F\dashv(-)^F$. Therefore **the covariant functor category is cartesian closed**. This proof supplies the actual exponential and does not need a colimit presentation of its arguments.

Finally suppose $\mathcal C$ itself is a [small category](../../../category.md#small-category) which is a [Cartesian closed category](../../../category.md#cartesian-closed-category). In its [presheaf category](../../../category.md#presheaf-category), the same construction, applied to $\mathcal C^{\mathrm{op}}$, gives

$$
\begin{aligned}
((YB)^{YA})(C)
&=\operatorname{Nat}(YC\times YA,YB)\\
&\cong\operatorname{Nat}(Y(C\times A),YB)\\
&\cong\mathcal C(C\times A,B)\\
&\cong\mathcal C(C,B^A)\\
&=Y(B^A)(C).
\end{aligned}
$$

The first [isomorphism](../../../algebra.md#isomorphism) uses the product's [universal property](../../../category-theory.md#universal-property): a map into $C\times A$ is precisely a pair of maps into $C$ and $A$. The next is the [Yoneda lemma](../../../category.md#yoneda-lemma), and the last is the exponential [adjunction](../../../category.md#adjoint-functors) in $\mathcal C$. Each step is natural in $C$, $A$, and $B$. Under these identifications, evaluation corresponds to $Y$ of the evaluation $B^A\times A\to B$. Hence **the Yoneda embedding preserves exponentials**, with the natural identification $\boxed{Y(B^A)\cong(YB)^{YA}}$.

## 4

↑ **Parent:** [Paper 26](paper-26.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

For an [adjunction](../../../category.md#adjoint-functors) $L:\mathcal C\rightleftarrows\mathcal D:R$, write its [adjunction unit](../../../category.md#unit-of-an-adjunction) as $\eta$ and its [adjunction counit](../../../category.md#counit-of-an-adjunction) as $\varepsilon$. It is an [idempotent adjunction](../../../category.md#idempotent-adjunction) when the induced [monad](../../../category-theory.md#monad) has invertible multiplication $\mu=R\varepsilon L:RLRL\Rightarrow RL$. The dual condition is invertibility of the induced [comonad](../../../category.md#comonad) comultiplication $\delta=L\eta R:LR\Rightarrow LRLR$.

To prove equivalence of these conditions, suppose $\mu$ is invertible. The two unit identities imply $T\eta=\eta T=\mu^{-1}$, where $T=RL$. For any [algebra for a monad](../../../category-theory.md#algebra-for-a-monad) $a:TA\to A$, naturality gives

$$
\eta_Aa=Ta\,\eta_{TA}=Ta\,T\eta_A=T(a\eta_A)=1_{TA},
$$

while $a\eta_A=1_A$. Thus $\eta_A$ is invertible. For each $D\in\mathcal D$, the arrow $R\varepsilon_D:T(RD)\to RD$ is a [monad algebra](../../../category-theory.md#algebra-for-a-monad) action, so $\eta_{RD}$ is invertible. Applying $L$ proves $\delta_D=L\eta_{RD}$ invertible. Apply this implication to the opposite [adjunction](../../../category.md#adjoint-functors), interchanging the roles of the [monad](../../../category-theory.md#monad) and comonad, to obtain the converse. Therefore **idempotence is self-dual**.

The [open-set frame](../../../category-theory.md#open-set-frame) $O(X)$ is ordered by inclusion. Its arbitrary [joins](../../../set.md#least-upper-bound-in-a-partially-ordered-set) are unions; arbitrary [meets](../../../set.md#greatest-lower-bound-in-a-partially-ordered-set) are interiors of intersections. Finite intersections are already open, so finite [meets](../../../set.md#greatest-lower-bound-in-a-partially-ordered-set) are ordinary intersections, including the empty [meet](../../../set.md#greatest-lower-bound-in-a-partially-ordered-set) $X$. Distributivity of intersection over arbitrary unions proves the [frame](../../../category-theory.md#complete-heyting-algebra) law. If $f:X\to Y$ is a [continuous map](../../../topology.md#continuous-map), inverse image

$$
f^{-1}:O(Y)\to O(X)
$$

preserves arbitrary unions and finite intersections, including $\varnothing$ and the entire space. It is therefore a [frame homomorphism](../../../category-theory.md#frame-homomorphism). Since $(gf)^{-1}=f^{-1}g^{-1}$ and $1_X^{-1}=1_{O(X)}$, this defines $O:\mathbf{Top}\to\mathbf{Frm}^{\mathrm{op}}$.

Let $\mathbf2=\{0<1\}$ and let $P(A)$ be the set of [points of a frame](../../../category-theory.md#point-of-a-frame) $A$, namely [frame homomorphisms](../../../category-theory.md#frame-homomorphism) $A\to\mathbf2$. For $a\in A$, put $U_a=\{p:p(a)=1\}$. Preservation of [joins](../../../set.md#least-upper-bound-in-a-partially-ordered-set) and finite [meets](../../../set.md#greatest-lower-bound-in-a-partially-ordered-set) gives

$$
U_0=\varnothing,\qquad U_1=P(A),\qquad U_{a\wedge b}=U_a\cap U_b,\qquad U_{\bigvee_i a_i}=\bigcup_iU_{a_i}.
$$

In the last equality, a [join](../../../set.md#least-upper-bound-in-a-partially-ordered-set) in $\mathbf2$ is $1$ precisely when at least one summand is $1$, also covering the empty family. Thus the sets $U_a$ are all the opens of a [topology](../../../topology.md), rather than merely a proposed basis.

For a [frame homomorphism](../../../category-theory.md#frame-homomorphism) $h:A\to B$, define $P(h):P(B)\to P(A)$ by $p\mapsto p\circ h$. Since $P(h)^{-1}(U_a)=U_{h(a)}$, it is continuous. Composition and identities follow from composition of functions, giving $P:\mathbf{Frm}^{\mathrm{op}}\to\mathbf{Top}$.

The [frame-point adjunction](../../../category-theory.md#frame-point-adjunction) is the natural [bijection](../../../function.md#bijection)

$$
\mathbf{Top}(X,P(A))\cong\mathbf{Frm}(A,O(X))
=\mathbf{Frm}^{\mathrm{op}}(O(X),A).
$$

A [continuous map](../../../topology.md#continuous-map) $f:X\to P(A)$ determines $h_f(a)=f^{-1}(U_a)$; the displayed identities for $U_a$ show that $h_f$ is a [frame homomorphism](../../../category-theory.md#frame-homomorphism). Conversely a [frame homomorphism](../../../category-theory.md#frame-homomorphism) $h:A\to O(X)$ determines $f_h(x)(a)=1$ exactly when $x\in h(a)$. Membership in unions and finite intersections proves that $f_h(x)$ is a [frame homomorphism](../../../category-theory.md#frame-homomorphism) to $\mathbf2$, and $f_h^{-1}(U_a)=h(a)$ proves continuity. These constructions are inverse. Precomposing in $X$ becomes inverse image of open sets; precomposing a [frame homomorphism](../../../category-theory.md#frame-homomorphism) becomes composition of [frame](../../../category-theory.md#complete-heyting-algebra) points. Hence the bijection is natural in both arguments and proves $O\dashv P$.

The [adjunction unit](../../../category.md#unit-of-an-adjunction) is

$$
\eta_X:X\to P(O(X)),\qquad \eta_X(x)(V)=1\ \Longleftrightarrow\ x\in V.
$$

The [adjunction counit](../../../category.md#counit-of-an-adjunction) at $A$, regarded as an arrow of $\mathbf{Frm}^{\mathrm{op}}$, is represented by the [frame homomorphism](../../../category-theory.md#frame-homomorphism) $e_A:A\to O(P(A))$, $a\mapsto U_a$. It is surjective because every open of $P(A)$ is of this form. We can compute $P(e_A):P(O(P(A)))\to P(A)$ explicitly: it sends $q$ to $p=q\circ e_A$. For every open $U_a$ of $P(A)$,

$$
\eta_{P(A)}(p)(U_a)=p(a)=q(U_a).
$$

Thus $\eta_{P(A)}P(e_A)=1$. Conversely, evaluation at $p$ sends $U_a$ to $p(a)$, so $P(e_A)\eta_{P(A)}=1$. Both maps are continuous by their definitions. Therefore $P(e_A)$ is a [homeomorphism](../../../topology.md#homeomorphism). The multiplication of the induced [monad](../../../category-theory.md#monad) $PO$ at $X$ is $P(e_{O(X)})$, which is invertible by this calculation. Consequently **the frame-point adjunction is idempotent**. This does not assert that every $\eta_X$ is a [homeomorphism](../../../topology.md#homeomorphism): it says that applying the point-space construction a second time makes no further change.

## 5

↑ **Parent:** [Paper 26](paper-26.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

A [filtered category](../../../category.md#filtered-category) is nonempty, any two objects have arrows to a common object, and any parallel pair $u,v:A\rightrightarrows B$ is equalized by some arrow $B\to C$. Equivalently, every finite diagram has a [cocone](../../../category.md#cocone-under-a-diagram): first choose a common target for its finitely many objects, then successively equalize the finitely many discrepancies along its arrows. A [weakly filtered category](../../../category.md#weakly-filtered-category) requires a [cocone](../../../category.md#cocone-under-a-diagram) only for finite nonempty connected diagrams. Equivalently, each [connected component of a category](../../../category.md#connected-component-of-a-category) is filtered. To see this, two objects in one component are joined by a finite zigzag; a [cocone](../../../category.md#cocone-under-a-diagram) on that zigzag gives a common target, and a parallel-pair diagram gives the equalization condition. Conversely a connected diagram lies in one filtered component. An empty category is weakly filtered, since it has no such diagrams.

The unique outgoing-arrow lifting property is precisely that of a [discrete opfibration](../../../category.md#discrete-opfibration). Let $F:\mathcal C\to\mathcal D$ have this property, with $\mathcal D$ weakly filtered. Take a diagram $H:J\to\mathcal C$ with $J$ finite, nonempty and connected, and choose a [cocone](../../../category.md#cocone-under-a-diagram) $\alpha_j:FH(j)\to D$ in $\mathcal D$. Lift each $\alpha_j$ uniquely from $H(j)$, obtaining $\widetilde\alpha_j:H(j)\to C_j$. For an arrow $u:j\to k$, the arrow $\widetilde\alpha_kH(u)$ and the lift $\widetilde\alpha_j$ have the same source and the same image $\alpha_kFH(u)=\alpha_j$. Unique lifting gives equality of the arrows and, importantly, $C_j=C_k$. Connectedness of $J$ makes all targets a single object $C_0$. The lifts are a [cocone](../../../category.md#cocone-under-a-diagram) in $\mathcal C$, so **the domain of a discrete opfibration over a weakly filtered category is weakly filtered**.

Consider [discrete opfibrations](../../../category.md#discrete-opfibration) $F:A\to D$ and $G:B\to D$ and their [pullback in a category](../../../category.md#pullback-category-theory) $E=A\times_D B$. The assumed creation of pullbacks describes its objects as pairs $(a,b)$ with $Fa=Gb$, and its arrows as pairs $(u,v)$ with $Fu=Gv$. There is a canonical map

$$
\Phi:\pi_0(E)\to\pi_0(A)\times_{\pi_0(D)}\pi_0(B),\qquad [(a,b)]\mapsto([a],[b]),
$$

where $\pi_0$ denotes [connected components of a category](../../../category.md#connected-component-of-a-category). Assume the vertices are [weakly filtered categories](../../../category.md#weakly-filtered-category).

For surjectivity, choose components $[a]$ and $[b]$ whose images belong to the same component of $D$. That component is filtered, so there are arrows $Fa\to d$ and $Gb\to d$. Lifting them from $a$ and $b$ gives $a\to a_1$ and $b\to b_1$ with $Fa_1=Gb_1=d$. Thus $(a_1,b_1)\in E$ maps to the chosen component pair.

For injectivity, suppose $(a,b)$ and $(a',b')$ have the same images under $\Phi$. Filteredness of the relevant components upstairs gives arrows

$$
a\xrightarrow{u}a_0\xleftarrow{u'}a',\qquad
b\xrightarrow{v}b_0\xleftarrow{v'}b'.
$$

Write $d=Fa=Gb$ and $d'=Fa'=Gb'$. In $D$ the four arrows $Fu,Gv,Fu',Gv'$ make a finite connected diagram with objects $d,d',Fa_0,Gb_0$. It has a [cocone](../../../category.md#cocone-under-a-diagram), so there are $r:Fa_0\to z$ and $s:Gb_0\to z$ with

$$
rFu=sGv,\qquad rFu'=sGv'.
$$

Lift $r$ from $a_0$ and $s$ from $b_0$, obtaining arrows to $a_1,b_1$ with $Fa_1=Gb_1=z$. Their composites with $(u,v)$ form an arrow $(a,b)\to(a_1,b_1)$ of $E$, and their composites with $(u',v')$ form an arrow $(a',b')\to(a_1,b_1)$. Hence the two representatives lie in the same component. This proves the [connected components of discrete-opfibration pullbacks](../../../category.md#connected-components-of-discrete-opfibration-pullbacks) formula

$$
\boxed{\pi_0(A\times_D B)\cong\pi_0(A)\times_{\pi_0(D)}\pi_0(B)}.
$$

The map is the canonical comparison, so this is preservation of the pullback, not just an accidental bijection of its objects.

Now fix a small [filtered category](../../../category.md#filtered-category) $C$. Every object $D\to C$ of $\mathrm{Disc}/C$ has weakly filtered domain by the lifting argument, and every arrow of this slice is a [discrete opfibration](../../../category.md#discrete-opfibration). Pullbacks in the slice are the created pullbacks above; their resulting domains are weakly filtered as well, since a pullback projection is a [discrete opfibration](../../../category.md#discrete-opfibration) onto a weakly filtered domain. The terminal slice object is $1_C:C\to C$. Because $C$ is nonempty and filtered, it is connected, so $\pi_0(C)$ is a singleton. Thus the component [functor](../../../category.md#functor) preserves the [terminal object](../../../category.md#terminal-object) and pullbacks. These construct every finite [categorical limit](../../../category.md#categorical-limit): binary products are pullbacks over the [terminal object](../../../category.md#terminal-object), and [equalizers](../../../category.md#equaliser) are pullbacks along a diagonal into a binary product. Therefore **the functor from this slice to sets preserves all finite limits**.

## 6

↑ **Parent:** [Paper 26](paper-26.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

A [preadditive category](../../../category.md#preadditive-category) has an [abelian group](../../../group.md#abelian-group) of [morphisms](../../../algebra.md#morphism) between each pair of objects, and composition is additive in both variables. An [additive category](../../../category-theory.md#additive-category) is a [preadditive category](../../../category.md#preadditive-category) with a [zero object](../../../category.md#zero-object) and finite [products in a category](../../../category.md#product-category-theory); equivalently one may require finite coproducts. The equivalence, and the stronger assertion that these constructions agree canonically, follow from the argument below. An [abelian category](../../../category-theory.md#abelian-category) is an [additive category](../../../category-theory.md#additive-category) with [kernels in a category](../../../category.md#kernel-in-a-category) and [cokernels in a category](../../../category.md#cokernel-in-a-category), in which every [monomorphism](../../../category.md#monomorphism) is a [categorical kernel](../../../category.md#kernel-in-a-category) and every [epimorphism](../../../category.md#epimorphism) is a [categorical cokernel](../../../category.md#cokernel-in-a-category). A [monomorphism](../../../category.md#monomorphism) with the first property is a [normal monomorphism](../../../category.md#normal-monomorphism); an [epimorphism](../../../category.md#epimorphism) with the second is a [conormal epimorphism](../../../category.md#conormal-epimorphism).

Let $P=\prod_{i=1}^n A_i$, with projections $p_i$. There is a unique $i_j:A_j\to P$ with $p_ii_j=\delta_{ij}1_{A_j}$, interpreting the other components as zero. Since every $p_j$ sends $\sum_i i_ip_i$ to $p_j$, the product's [universal property](../../../category-theory.md#universal-property) gives

$$
p_ii_j=\delta_{ij}1_{A_j},\qquad \sum_i i_ip_i=1_P.
$$

Given arrows $f_i:A_i\to B$, put $f=\sum_i f_ip_i$. Then $fi_j=f_j$. Conversely any arrow with these restrictions equals $f1_P=\sum_i fi_ip_i$, so it is uniquely this sum. Thus $(P,i_i)$ is a [coproduct in a category](../../../category.md#coproduct). The empty product is the [zero object](../../../category.md#zero-object) and also the empty coproduct. The dual argument starts from coproducts and constructs projections; it proves the equivalent definition. Hence **finite products and coproducts are the same biproducts**, with the displayed identities giving the canonical identification.

For the [image factorization in an abelian category](../../../category.md#image-factorization-in-an-abelian-category), let $h:A\to B$, let $c:B\to Q$ be its [cokernel](../../../linear-algebra.md#cokernel), and let $i:I\to B$ be the [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) of $c$. Since $ch=0$, write $h=ie$. We prove that $e:A\to I$ is epic. Suppose $t:I\to Z$ satisfies $te=0$ and let $l:L\to I$ be its [categorical kernel](../../../category.md#kernel-in-a-category). Then $e=lr$ for some $r:A\to L$. The composite $il$ is monic and hence is a [normal monomorphism](../../../category.md#normal-monomorphism), say $il=\ker z$ for $z:B\to W$. Since $zh=zilr=0$, the [categorical cokernel](../../../category.md#cokernel-in-a-category) property makes $z$ factor through $c$, and therefore $zi=0$. The [categorical kernel](../../../category.md#kernel-in-a-category) property of $il$ gives $s:I\to L$ with $ils=i$. Cancellation of $i$ yields $ls=1_I$; since $l$ is monic this also gives $sl=1_L$. Thus $l$ is invertible and $t=0$. In a [preadditive category](../../../category.md#preadditive-category), $ue=ve$ now implies $(u-v)e=0$, hence $u=v$. This proves $e$ is an [epimorphism](../../../category.md#epimorphism) and supplies the required factorization.

For uniqueness, an [epimorphism](../../../category.md#epimorphism) that is a [categorical cokernel](../../../category.md#cokernel-in-a-category) is the [categorical cokernel](../../../category.md#cokernel-in-a-category) of its own [categorical kernel](../../../category.md#kernel-in-a-category). Indeed, if $e=\operatorname{coker}r$ and $k=\ker e$, then $r$ factors through $k$; an arrow killing $k$ therefore kills $r$ and factors uniquely through $e$. Dually, a [normal monomorphism](../../../category.md#normal-monomorphism) is the [categorical kernel](../../../category.md#kernel-in-a-category) of its own [categorical cokernel](../../../category.md#cokernel-in-a-category). If $h=mp$ is any epi–mono factorization, monicity of $m$ gives $\ker p=\ker h$. Both $p$ and $e$ are consequently [categorical cokernels](../../../category.md#cokernel-in-a-category) of this same [categorical kernel](../../../category.md#kernel-in-a-category). Their [universal properties](../../../category-theory.md#universal-property) give a unique [isomorphism](../../../algebra.md#isomorphism) $\theta$ between the intermediate objects with $\theta p=e$, and cancellation of $p$ gives $i\theta=m$. Therefore **the epi–mono factorization is unique up to the unique compatible isomorphism**.

Here is an [additive category with truncated primary torsion](../../../category-theory.md#additive-category-with-truncated-primary-torsion), with the prime fixed as $2$. Its objects are [finitely generated abelian groups](../../../group.md#finitely-generated-abelian-group) having no element of order $4$, and its morphisms are all [group homomorphisms](../../../group-theory.md#group-homomorphism). Equivalently their $2$-primary torsion [subgroup](../../../group.md#subgroup) has exponent at most $2$. It is a full [subcategory](../../../category.md#subcategory) of [abelian groups](../../../group.md#abelian-group), closed under finite [direct sums](../../../vector-space.md#direct-sum) and [subgroups](../../../group.md#subgroup). Its hom groups and bilinear composition are inherited, and the zero group and finite [direct sums](../../../vector-space.md#direct-sum) belong to it, so it is additive. [Categorical kernels](../../../category.md#kernel-in-a-category) are ordinary [subgroup](../../../group.md#subgroup) [categorical kernels](../../../category.md#kernel-in-a-category), which are still finitely generated and have no element of order $4$.

To construct [categorical cokernels](../../../category.md#cokernel-in-a-category), for an arbitrary finitely generated [abelian group](../../../group.md#abelian-group) $G$ let $t_2(G)$ be its $2$-primary [torsion subgroup](../../../group-theory.md#torsion-subgroup), and define

$$
R(G)=G/(2t_2(G)).
$$

The [Fundamental theorem of finitely generated abelian groups](../../../group.md#fundamental-theorem-of-finitely-generated-abelian-groups) shows that this quotient lies in the subcategory: it leaves the free and odd-primary parts unchanged and replaces each cyclic $2$-primary summand by either $0$ or $\mathbb Z/2\mathbb Z$. Every homomorphism $G\to H$ to an allowed group kills $2t_2(G)$, because it sends $2$-primary torsion into a [subgroup](../../../group.md#subgroup) killed by $2$. Thus $G\to R(G)$ has the [universal property](../../../category-theory.md#universal-property) of a reflection. For $f:A\to B$, its [categorical cokernel](../../../category.md#cokernel-in-a-category) in the subcategory is

$$
B\longrightarrow R(B/f(A)).
$$

This has exactly the [categorical cokernel](../../../category.md#cokernel-in-a-category) [universal property](../../../category-theory.md#universal-property) by the preceding factorization. Finite [categorical limits](../../../category.md#categorical-limit) exist because [equalizers](../../../category.md#equaliser) are [categorical kernels](../../../category.md#kernel-in-a-category) of differences and finite products exist. Finite [colimits](../../../category.md#colimit) exist dually because [coequalizers](../../../category.md#coequalizer) are [categorical cokernels](../../../category.md#cokernel-in-a-category) of differences and finite coproducts exist.

The [epimorphisms](../../../category.md#epimorphism) in this example are precisely the surjective homomorphisms. A surjection is epic already in [abelian groups](../../../group.md#abelian-group). Conversely, if $f$ is epic in the subcategory, its [categorical cokernel](../../../category.md#cokernel-in-a-category) is zero, so $R(B/f(A))=0$. A nonzero finitely generated [abelian group](../../../group.md#abelian-group) has nonzero reflection: a nonzero free or odd-primary summand survives, and a nonzero finite $2$-primary summand has a nonzero quotient modulo twice itself. Hence $B/f(A)=0$ and $f$ is surjective. Its ordinary [categorical kernel](../../../category.md#kernel-in-a-category) belongs to the subcategory, and its quotient by that [categorical kernel](../../../category.md#kernel-in-a-category) is its codomain, which also belongs to the subcategory. It is therefore the [categorical cokernel](../../../category.md#cokernel-in-a-category) of its [categorical kernel](../../../category.md#kernel-in-a-category). This proves that every [epimorphism](../../../category.md#epimorphism) is conormal.

The [monomorphism](../../../category.md#monomorphism)

$$
m:\mathbb Z\to\mathbb Z,\qquad m(n)=4n
$$

is not normal. Its [categorical cokernel](../../../category.md#cokernel-in-a-category) in this category is reduction modulo $2$, since $R(\mathbb Z/4\mathbb Z)=\mathbb Z/2\mathbb Z$. The [categorical kernel](../../../category.md#kernel-in-a-category) of that [categorical cokernel](../../../category.md#cokernel-in-a-category) is the inclusion $2\mathbb Z\hookrightarrow\mathbb Z$, whereas the image of $m$ is $4\mathbb Z$. A [normal monomorphism](../../../category.md#normal-monomorphism) is the [categorical kernel](../../../category.md#kernel-in-a-category) of its own [categorical cokernel](../../../category.md#cokernel-in-a-category), as proved above, so $m$ cannot be normal. In fact multiplication by $2$ is itself the [categorical kernel](../../../category.md#kernel-in-a-category) of reduction modulo $2$, up to the identification $\mathbb Z\cong2\mathbb Z$. Its composite with itself is multiplication by $4$. Thus this example already exhibits two [normal monomorphisms](../../../category.md#normal-monomorphism) whose composite is not normal.

For the general assertion, let $m:A\to B$ be a nonnormal [monomorphism](../../../category.md#monomorphism) in any [additive category](../../../category-theory.md#additive-category) of the specified kind. Put $c=\operatorname{coker}m$ and $k:K\to B$ be its [categorical kernel](../../../category.md#kernel-in-a-category), and factor $m=kg$. Both $m$ and $k$ are monic, so $g$ is monic. Set $d=\operatorname{coker}g$ and $l:L\to K$ be its [categorical kernel](../../../category.md#kernel-in-a-category). Then $k,l$ are normal, and $g=lr$ for some $r$.

Suppose their composite were normal, say $kl=\ker t$. Since $tm=tklr=0$, $t$ factors through $c$, whence $tk=0$. The [categorical kernel](../../../category.md#kernel-in-a-category) property of $kl$ supplies $s:K\to L$ with $kls=k$; cancellation shows $ls=1_K$, and monicity makes $l$ an [isomorphism](../../../algebra.md#isomorphism). Because $dl=0$, this forces $d=0$. In a [preadditive category](../../../category.md#preadditive-category), vanishing of the [categorical cokernel](../../../category.md#cokernel-in-a-category) of $g$ implies that $g$ is epic: any $u,v$ with $ug=vg$ have $u-v$ factor through the zero [categorical cokernel](../../../category.md#cokernel-in-a-category). By hypothesis $g$ is therefore a [categorical cokernel](../../../category.md#cokernel-in-a-category), and it is also monic. If $g=\operatorname{coker}a$, monicity and $ga=0$ force $a=0$; a [categorical cokernel](../../../category.md#cokernel-in-a-category) of a zero arrow is an [isomorphism](../../../algebra.md#isomorphism). Thus $g$ is invertible, making $m=kg$ normal, a contradiction. Consequently **normal monomorphisms cannot be closed under composition in any such category**; the explicit pair $k,l$ witnesses the failure.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2005](../../2005.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
