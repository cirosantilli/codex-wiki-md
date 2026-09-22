# Paper 119

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_119.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_119.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [Solution](#6/solution)

## 1

↑ **Parent:** [Paper 119](paper-119.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

An [equivalence of categories](../../../category.md#equivalence-of-categories) consists of [functors](../../../category.md#functor) $F:\mathcal C\to\mathcal D$ and $G:\mathcal D\to\mathcal C$ together with invertible [natural transformations](../../../category.md#natural-transformation) $GF\cong1_{\mathcal C}$ and $FG\cong1_{\mathcal D}$. A strict [isomorphism of categories](../../../category.md#isomorphism-of-categories) instead requires a [functor](../../../category.md#functor) with an inverse whose composites are literally identity [functors](../../../category.md#functor).

First suppose $F$ belongs to an [equivalence of categories](../../../category.md#equivalence-of-categories). The isomorphisms $FGD\cong D$ give [essential surjectivity](../../../category.md#essential-surjectivity). If $Ff=Fg$, apply $G$ and conjugate by $GF\cong1_{\mathcal C}$ to obtain $f=g$, so $F$ is a [faithful functor](../../../category.md#faithful-functor). Similarly $G$ is a [faithful functor](../../../category.md#faithful-functor). Writing $\alpha:GF\xrightarrow{\sim}1_{\mathcal C}$, any $h:FA\to FB$ has a preimage

$$
f=\alpha_B\,G(h)\,\alpha_A^{-1}.
$$

Indeed [naturality](../../../category.md#naturality) of $\alpha$ gives $GF(f)=G(h)$, and faithfulness of $G$ gives $F(f)=h$. Thus $F$ is a [full and faithful functor](../../../category.md#full-and-faithful-functor).

Conversely, assume $F$ is a [full and faithful functor](../../../category.md#full-and-faithful-functor) and has [essential surjectivity](../../../category.md#essential-surjectivity). Using the [axiom of choice](../../../set-theory.md#axiom-of-choice), for each $D$ choose an object $GD$ and an isomorphism $\theta_D:F(GD)\to D$. Define $G$ on a [morphism](../../../algebra.md#morphism) $h:D\to E$ by the unique lift

$$
F(Gh)=\theta_E^{-1}h\theta_D.
$$

The [full and faithful functor](../../../category.md#full-and-faithful-functor) property makes $G$ preserve identities and composition, and makes $\theta:FG\cong1_{\mathcal D}$ a [natural transformation](../../../category.md#natural-transformation). For $A\in\mathcal C$, lift $\theta_{FA}:FGFA\to FA$ uniquely to $\alpha_A:GFA\to A$. Lifting its inverse shows that $\alpha_A$ is invertible. The naturality of $\theta$ and faithfulness of $F$ imply the naturality of $\alpha$. This proves

$$
\boxed{F\text{ is an equivalence}\iff F\text{ is full, faithful and essentially surjective}.}
$$

For large [categories](../../../category.md), this choice argument is understood in a fixed universe, or with the corresponding class-choice convention; ordinary set-sized [axiom of choice](../../../set-theory.md#axiom-of-choice) suffices for [small categories](../../../category.md#small-category).

For the [category of partial functions](../../../category.md#category-of-partial-functions), let $X_+=X\amalg\{*\}$, with a tagged new element as basepoint. Send a [partial function](../../../function.md#partial-function) $f:X\rightharpoonup Y$ to the basepoint-preserving total [function](../../../function.md)

$$
f_+(x)=\begin{cases}f(x),&x\in\operatorname{dom}f,\\ *,&x\notin\operatorname{dom}f,\end{cases}
\qquad f_+(*)=*.
$$

Undefined composition is sent to the basepoint, so this is a [functor](../../../category.md#functor) $(-)_+:\mathbf{Part}\to\mathbf{Set}_*$. Restriction away from the basepoint recovers each [partial function](../../../function.md#partial-function) uniquely; hence it is a [full and faithful functor](../../../category.md#full-and-faithful-functor). Every [pointed set](../../../set.md#pointed-set) $(Y,y_0)$ is isomorphic to $(Y\setminus\{y_0\})_+$, so there is an [equivalence of categories](../../../category.md#equivalence-of-categories). This particular equivalence can also be constructed explicitly, without choice, by deleting and adjoining the basepoint.

These actual [categories](../../../category.md) are **equivalent but not isomorphic**. In $\mathbf{Part}$ the empty [set](../../../set.md) is the only [zero object](../../../category.md#zero-object): if $X$ is nonempty, its identity differs from its nowhere-defined endomorphism, so it cannot be initial or terminal. In $\mathbf{Set}_*$ every singleton [pointed set](../../../set.md#pointed-set) is a [zero object](../../../category.md#zero-object), and distinct singleton underlying [sets](../../../set.md) give distinct objects. An [isomorphism of categories](../../../category.md#isomorphism-of-categories) is a bijection on objects preserving [zero objects](../../../category.md#zero-object); it cannot take one such object onto several. This uses the categories of all actual [sets](../../../set.md), as in the paper, rather than chosen [skeletal categories](../../../category.md#skeletal-category) of representatives.

A [skeletal category](../../../category.md#skeletal-category) has no distinct isomorphic objects. If an equivalence $F:\mathcal C\to\mathcal D$ joins two [skeletal categories](../../../category.md#skeletal-category), [essential surjectivity](../../../category.md#essential-surjectivity) becomes surjectivity on objects. If $FA=FB$, lift the identity of that object and its inverse using [full and faithful](../../../category.md#full-and-faithful-functor) to obtain $A\cong B$, so $A=B$. Thus $F$ is bijective on objects and on every hom-set. Its inverse on objects and [morphisms](../../../algebra.md#morphism) is a strictly inverse [functor](../../../category.md#functor), proving that it is an [isomorphism of categories](../../../category.md#isomorphism-of-categories).

Under the [axiom of choice](../../../set-theory.md#axiom-of-choice), choose one object from each isomorphism class of a [small category](../../../category.md#small-category). The full [subcategory](../../../category.md#subcategory) on those objects is a [skeleton of a category](../../../category.md#skeleton-of-a-category), and its inclusion is a [full and faithful functor](../../../category.md#full-and-faithful-functor) with [essential surjectivity](../../../category.md#essential-surjectivity), hence an [equivalence of categories](../../../category.md#equivalence-of-categories).

For the converse, form the [small category](../../../category.md#small-category) which is a [groupoid](../../../category.md#groupoid) with objects $(i,a)$ for $a\in A_i$, and exactly one [morphism](../../../algebra.md#morphism) $(i,a)\to(j,b)$ when $i=j$, with no [morphisms](../../../algebra.md#morphism) when $i\ne j$. Suppose it is equivalent to a [skeletal category](../../../category.md#skeletal-category) $\mathcal S$, with quasi-inverse [functors](../../../category.md#functor) $H:\mathcal C\to\mathcal S$ and $K:\mathcal S\to\mathcal C$. For each $i$, the objects $H(i,a)$ for $a\in A_i$ are isomorphic, hence all equal to a uniquely determined $s_i$. The isomorphism $KH(i,a)\cong(i,a)$ ensures that $K(s_i)=(i,a_i)$ for some $a_i\in A_i$. The rule $i\mapsto a_i$ is a choice function. In particular, no representative in $A_i$ had to be chosen to define $s_i$, since it is unique. Consequently

$$
\boxed{\text{Every small category has a skeletal equivalent}\iff\text{the axiom of choice}.}
$$

## 2

↑ **Parent:** [Paper 119](paper-119.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

A [balanced category](../../../category.md#balanced-category) is one in which every [morphism](../../../algebra.md#morphism) that is both a [monomorphism](../../../category.md#monomorphism) and an [epimorphism](../../../category.md#epimorphism) is an [isomorphism](../../../algebra.md#isomorphism). A [faithful functor](../../../category.md#faithful-functor) reflects both of these cancellation properties: for instance, $fu=fv$ implies $Ff\,Fu=Ff\,Fv$, so monicity of $Ff$ and faithfulness imply $u=v$; the dual argument applies to [epimorphisms](../../../category.md#epimorphism). If $Ff$ is invertible, it is both monic and epic. Thus a [faithful functor](../../../category.md#faithful-functor) from a [balanced category](../../../category.md#balanced-category) reflects [isomorphisms](../../../algebra.md#isomorphism).

For the [adjunction](../../../category.md#adjoint-functors) $F\dashv G$, the [unit and counit of an adjunction](../../../category.md#unit-and-counit-of-an-adjunction) satisfy

$$
\varepsilon_{FA}F\eta_A=1_{FA},\qquad G\varepsilon_B\eta_{GB}=1_{GB}.
$$

If $F$ is a [faithful functor](../../../category.md#faithful-functor) and $\eta_Au=\eta_Av$, applying $F$ and composing with $\varepsilon_{FA}$ gives $Fu=Fv$, hence $u=v$. Thus each $\eta_A$ is a [monomorphism](../../../category.md#monomorphism). Conversely, if every $\eta_A$ is monic and $Fu=Fv$ for $u,v:X\to A$, [naturality](../../../category.md#naturality) gives

$$
\eta_Au=GFu\,\eta_X=GFv\,\eta_X=\eta_Av,
$$

so $u=v$. This proves the [faithful left adjoint criterion](../../../category.md#faithful-left-adjoint-criterion).

Now assume both $\eta$ and $\varepsilon$ are pointwise monic. The first triangle identity makes $\varepsilon_{FA}$ a [split epimorphism](../../../category.md#split-epimorphism); since it is also a [monomorphism](../../../category.md#monomorphism), it is invertible and $F\eta_A$ is its inverse. The [faithful left adjoint criterion](../../../category.md#faithful-left-adjoint-criterion) says that $F$ is faithful, and the [balanced category](../../../category.md#balanced-category) argument above then reflects the invertibility of $F\eta_A$ to that of $\eta_A$.

For completeness, an invertible unit makes $F$ a [full and faithful functor](../../../category.md#full-and-faithful-functor). For $h:FA\to FA'$, set $k=\eta_{A'}^{-1}G(h)\eta_A$. The triangle identity gives $F\eta_A=\varepsilon_{FA}^{-1}$, so [naturality](../../../category.md#naturality) of $\varepsilon$ yields

$$
F(k)=\varepsilon_{FA'}FG(h)\varepsilon_{FA}^{-1}=h.
$$

Faithfulness was already proved.

Let $q:FA\to B$ be a [strong epimorphism](../../../category.md#strong-epimorphism), and put

$$
t=FG(q)\varepsilon_{FA}^{-1}:FA\to FGB.
$$

Then [naturality](../../../category.md#naturality) gives $\varepsilon_Bt=q$. The square with left edge $q$, right edge the [monomorphism](../../../category.md#monomorphism) $\varepsilon_B$, top edge $t$, and bottom edge $1_B$ has a diagonal $s:B\to FGB$ by the defining lifting property of a [strong epimorphism](../../../category.md#strong-epimorphism). Thus $\varepsilon_Bs=1_B$. A monic [split epimorphism](../../../category.md#split-epimorphism) is invertible, so $B\cong FGB$. The essential image of $F$ is therefore closed under [strong quotients](../../../category.md#strong-quotient).

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Assume $F$ is a [full and faithful functor](../../../category.md#full-and-faithful-functor) and its essential image is closed under [strong quotients](../../../category.md#strong-quotient). First its unit is invertible. To prove this directly, fullness gives $k:GFA\to A$ with $Fk=\varepsilon_{FA}$. The triangle identity and faithfulness give $k\eta_A=1_A$. [Naturality](../../../category.md#naturality) of $\eta$ at $k$ and the other triangle identity give

$$
\eta_Ak=GFk\,\eta_{GFA}=G\varepsilon_{FA}\,\eta_{GFA}=1_{GFA}.
$$

Thus $\eta_A$ is an [isomorphism](../../../algebra.md#isomorphism), and $\varepsilon_{FA}=(F\eta_A)^{-1}$ is also an [isomorphism](../../../algebra.md#isomorphism).

Factor $\varepsilon_B$ as a [strong epimorphism](../../../category.md#strong-epimorphism) followed by a [monomorphism](../../../category.md#monomorphism). By closure under [strong quotients](../../../category.md#strong-quotient), the intermediate object can, after transport along an [isomorphism](../../../algebra.md#isomorphism), be written as $FA$:

$$
FGB\xrightarrow{e}FA\xrightarrow{m}B,\qquad \varepsilon_B=me.
$$

Fullness gives $e=Fk$ for $k:GB\to A$. Taking the transpose of $\varepsilon_B=mFk$ under the [adjunction](../../../category.md#adjoint-functors), whose transpose is $1_{GB}$, gives

$$
1_{GB}=Gm\,GFk\,\eta_{GB}=Gm\,\eta_A\,k.
$$

Hence $k$ is a [split monomorphism](../../../category.md#split-monomorphism), so $e=Fk$ is a [monomorphism](../../../category.md#monomorphism). A [strong epimorphism](../../../category.md#strong-epimorphism) which is monic is invertible: apply its lifting property to the square with that same map on both sides and identity top and bottom edges. Thus $e$ is invertible and $\varepsilon_B=me$ is monic. We have proved the [pointwise-monic unit-and-counit criterion](../../../category.md#pointwise-monic-unit-and-counit-criterion):

$$
\boxed{\eta,\varepsilon\text{ monic}\iff F\text{ fully faithful with image closed under strong quotients}.}
$$

For a counterexample without the balanced hypothesis, use the [pointwise-monic adjunction over a non-balanced poset](../../../category.md#pointwise-monic-adjunction-over-a-non-balanced-poset). Let $\mathcal C=\{0<1\}$ and let $\mathcal D$ have one object and only its identity. The unique $F:\mathcal C\to\mathcal D$ is left adjoint to $G$ selecting $1$, since both $\mathcal D(Fc,*)$ and $\mathcal C(c,1)$ are singletons. All [morphisms](../../../algebra.md#morphism) in a [poset](../../../set.md#partially-ordered-set) viewed as a [category](../../../category.md) are [monomorphisms](../../../category.md#monomorphism), so the unit and counit are monic. However $F$ is not full: the identity $F1\to F0$ has no preimage $1\to0$. The arrow $0\to1$ is both monic and epic but not invertible, so $\mathcal C$ is not a [balanced category](../../../category.md#balanced-category). **The balanced hypothesis cannot be dropped.**

## 3

↑ **Parent:** [Paper 119](paper-119.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

A [diagram in a category](../../../category.md#diagram-category-theory) of shape $J$ is a [functor](../../../category.md#functor) $D:J\to\mathcal C$. A [categorical cone](../../../category.md#cone-over-a-diagram) with vertex $X$ is a family $\gamma_j:X\to Dj$ satisfying $D(a)\gamma_j=\gamma_k$ for every $a:j\to k$. A [morphism](../../../algebra.md#morphism) between [categorical cones](../../../category.md#cone-over-a-diagram) from $(X,\gamma)$ to $(Y,\delta)$ is a [morphism](../../../algebra.md#morphism) $u:X\to Y$ with $\delta_ju=\gamma_j$ for all $j$. A [categorical limit](../../../category.md#categorical-limit) is a [terminal object](../../../category.md#terminal-object) in this [category](../../../category.md) of cones: each cone has a unique such [morphism](../../../algebra.md#morphism) to the limiting cone.

For a finite $J$, form the [products in a category](../../../category.md#product-category-theory)

$$
P=\prod_{j\in\operatorname{ob}J}Dj,\qquad Q=\prod_{a:j\to k}Dk.
$$

Define $s,t:P\rightrightarrows Q$ with $a$-coordinates $D(a)\pi_j$ and $\pi_k$. The [equalizer](../../../category.md#equaliser) $e:L\to P$ imposes exactly the cone equations. Therefore $\pi_je$ gives a [categorical limit](../../../category.md#categorical-limit) of $D$, since maps into $P$ encode families of legs and factoring through $e$ encodes their compatibility. The empty [product in a category](../../../category.md#product-category-theory) is the [terminal object](../../../category.md#terminal-object), covering the empty diagram. This is the [construction of small limits from products and equalizers](../../../category.md#construction-of-small-limits-from-products-and-equalizers), restricted to finite shapes.

Now take an [initial functor](../../../category.md#initial-functor) $F:I\to J$ and a [categorical cone](../../../category.md#cone-over-a-diagram) $\delta_i:X\to DFi$ over $DF$. For each $j$ and each object $(i,u:Fi\to j)$ of the [comma category](../../../category.md#comma-category) $(F\downarrow j)$, consider $D(u)\delta_i$. A [morphism](../../../algebra.md#morphism) $a:(i,u)\to(i',u')$ there satisfies $u'F(a)=u$, so

$$
D(u')\delta_{i'}=D(u')D(Fa)\delta_i=D(u)\delta_i.
$$

Since $(F\downarrow j)$ is a nonempty [connected category](../../../category.md#connected-category), this common value is independent of the object. Define it to be $\gamma_j$. This does not require choosing representatives: the value is uniquely determined.

For $b:j\to k$, replacing $(i,u)$ by $(i,bu)$ proves $D(b)\gamma_j=\gamma_k$. Taking $(i,1_{Fi})$ proves $\gamma_{Fi}=\delta_i$. Conversely, extending a restricted cone recovers its original legs, since $\gamma_j=D(u)\gamma_{Fi}$. A vertex [morphism](../../../algebra.md#morphism) commuting with every $\delta_i$ also commutes with each $\gamma_j=D(u)\delta_i$, and the converse follows by restriction. Thus extension and restriction are strictly inverse [functors](../../../category.md#functor), not merely an [equivalence of categories](../../../category.md#equivalence-of-categories). This proves [cone restriction along an initial functor](../../../category.md#cone-restriction-along-an-initial-functor).

If $\mathcal C$ has all [categorical limits](../../../category.md#categorical-limit) of shape $I$, transport a [terminal object](../../../category.md#terminal-object) in the cone category of $DF$ across this isomorphism to obtain a [categorical limit](../../../category.md#categorical-limit) of $D$. Uniqueness of the induced comparison, and its compatibility with [natural transformations](../../../category.md#natural-transformation) of diagrams, gives

$$
\boxed{\lim_J\cong\lim_I\circ F^*.}
$$

For the converse use the [representable test for initial functors](../../../category.md#representable-test-for-initial-functors). For $j\in J$, the [representable presheaf](../../../category.md#representable-functor) $J(-,j):J^{\mathrm{op}}\to\mathbf{Set}$ is equivalently a [diagram in a category](../../../category.md#diagram-category-theory) $D_j:J\to\mathbf{Set}^{\mathrm{op}}$. Its [categorical limit](../../../category.md#categorical-limit) in the [opposite category](../../../category.md#opposite-category) is the [colimit](../../../category.md#colimit) of $J(-,j)$ in [sets](../../../set.md). Elements of that [colimit](../../../category.md#colimit) are connected components of the [category of elements](../../../category.md#category-of-elements), equivalently of the [opposite category](../../../category.md#opposite-category) of the slice $J\downarrow j$. This slice has [terminal object](../../../category.md#terminal-object) $(j,1_j)$, so that [colimit](../../../category.md#colimit) is a singleton.

For the restricted presheaf $J(F(-),j)$, the same description identifies its [colimit](../../../category.md#colimit) with the connected-component [set](../../../set.md) of $(F\downarrow j)$. Indeed a relation identifying $u':Fi'\to j$ with $u'F(a):Fi\to j$ is exactly a generating edge of the zigzag relation in this [comma category](../../../category.md#comma-category). The assumed isomorphism of limit [functors](../../../category.md#functor) forces this [set](../../../set.md) to be a singleton. Therefore $(F\downarrow j)$ is nonempty and connected for every $j$, proving

$$
\boxed{F\text{ is initial}.}
$$

## 4

↑ **Parent:** [Paper 119](paper-119.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

A [monad](../../../category-theory.md#monad) on $\mathcal C$ is an endofunctor $T$ with [natural transformations](../../../category.md#natural-transformation) $\eta:1\to T$ and $\mu:T^2\to T$ satisfying

$$
\mu\,T\mu=\mu\,\mu T,\qquad \mu\,T\eta=1_T=\mu\,\eta T.
$$

An [algebra for a monad](../../../category-theory.md#algebra-for-a-monad) is $(A,\alpha:TA\to A)$ with $\alpha\eta_A=1_A$ and $\alpha T\alpha=\alpha\mu_A$. A [morphism of algebras for a monad](../../../category-theory.md#morphism-of-algebras-for-a-monad) $f:(A,\alpha)\to(B,\beta)$ satisfies $f\alpha=\beta Tf$. These form the [Eilenberg-Moore category](../../../category-theory.md#eilenberg-moore-category) $\mathcal C^T$. Its [free algebra functor](../../../category-theory.md#free-algebra-functor) is $FX=(TX,\mu_X)$, and its [adjunction](../../../category.md#adjoint-functors) to the forgetful [functor](../../../category.md#functor) $U$ has the explicit bijection

$$
\mathcal C^T(FX,(C,\gamma))\cong\mathcal C(X,C),\qquad
h\longmapsto h\eta_X,\qquad u\longmapsto\gamma Tu.
$$

Write $S=A+B$, $V=TA+TB$, and let $\nu_1,\nu_2$ be the [coproduct in a category](../../../category.md#coproduct) injections. Set

$$
r=F(\alpha+\beta),\qquad s=\mu_SF\kappa: FV\rightrightarrows FS,
\qquad \kappa=[T\nu_1,T\nu_2].
$$

Here $\mu_S:FTS\to FS$ is an algebra [morphism](../../../algebra.md#morphism), with underlying multiplication $T^2S\to TS$. For an algebra $(C,\gamma)$, an algebra [morphism](../../../algebra.md#morphism) $h:FS\to(C,\gamma)$ corresponds to $u:S\to C$, and the transposes of $hr,hs$ are respectively

$$
u(\alpha+\beta),\qquad h\kappa=\gamma Tu\,\kappa.
$$

For the second formula, $(\mu_ST\kappa)\eta_V=\kappa$ by [naturality](../../../category.md#naturality) of $\eta$ and the [monad](../../../category-theory.md#monad) unit law. Thus $hr=hs$ exactly when, writing $u=[a,b]$,

$$
a\alpha=\gamma Ta,\qquad b\beta=\gamma Tb.
$$

These say precisely that $a$ and $b$ are [morphisms of algebras for a monad](../../../category-theory.md#morphism-of-algebras-for-a-monad). Consequently any [coequalizer](../../../category.md#coequalizer) $q:FS\to Q$ of $r,s$ represents pairs of algebra [morphisms](../../../algebra.md#morphism) out of $(A,\alpha)$ and $(B,\beta)$, proving the [coproduct presentation for monad algebras](../../../category-theory.md#coproduct-presentation-for-monad-algebras):

$$
\boxed{Q\cong(A,\alpha)+(B,\beta)\quad\text{in }\mathcal C^T.}
$$

Its two algebra injections have underlying [morphisms](../../../algebra.md#morphism) $q\eta_S\nu_1$ and $q\eta_S\nu_2$; the equivalence just proved verifies both the algebra equations and their universal property.

The displayed pair is a [reflexive pair](../../../category-theory.md#reflexive-pair), with common section

$$
t=F(\eta_A+\eta_B):FS\to FV.
$$

Indeed $rt=1_{FS}$ by the algebra unit laws, while

$$
\kappa(\eta_A+\eta_B)=\eta_S,\qquad st=\mu_SF\eta_S=1_{FS}.
$$

Now suppose $\mathcal C$ has all finite [colimits](../../../category.md#colimit) and $T$ preserves [reflexive coequalizers](../../../category-theory.md#reflexive-coequalizer). The permitted creation theorem gives [reflexive coequalizers](../../../category-theory.md#reflexive-coequalizer) in $\mathcal C^T$: the underlying pair is reflexive and its [coequalizer](../../../category.md#coequalizer) exists and is preserved by $T$. The preceding construction therefore gives binary algebra [coproducts in a category](../../../category.md#coproduct). The [initial object](../../../category.md#initial-object) is $F0$, since the [free algebra functor](../../../category-theory.md#free-algebra-functor) is a [left adjoint](../../../category.md#adjoint-functors) and $0$ is initial in $\mathcal C$.

For any algebra pair $a,b:X\rightrightarrows Y$, the augmented pair

$$
[a,1_Y],[b,1_Y]:X+Y\rightrightarrows Y
$$

is a [reflexive pair](../../../category-theory.md#reflexive-pair), with common section the injection of $Y$, and has exactly the same coequalizing [morphisms](../../../algebra.md#morphism) as $a,b$. Hence all [coequalizers](../../../category.md#coequalizer) exist in $\mathcal C^T$. The [construction of finite colimits from coproducts and reflexive coequalizers](../../../category.md#construction-of-finite-colimits-from-coproducts-and-reflexive-coequalizers) now gives

$$
\boxed{\mathcal C^T\text{ has all finite colimits}.}
$$

## 5

↑ **Parent:** [Paper 119](paper-119.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

A [regular category](../../../category.md#regular-category) has finite [categorical limits](../../../category.md#categorical-limit), [coequalizers](../../../category.md#coequalizer) of [kernel pairs](../../../category.md#kernel-pair), and [regular epimorphism](../../../category.md#regular-epimorphism)–[monomorphism](../../../category.md#monomorphism) image factorizations whose [regular epimorphisms](../../../category.md#regular-epimorphism) are stable under every [pullback in a category](../../../category.md#pullback-category-theory). Equivalently, finite limits, pullback-stable [regular epimorphism](../../../category.md#regular-epimorphism)–[monomorphism](../../../category.md#monomorphism) factorizations suffice. In particular, every [strong epimorphism](../../../category.md#strong-epimorphism) in a [regular category](../../../category.md#regular-category) is regular.

For the weaker hypotheses here, interpret an [image factorization](../../../category.md#image-factorization) as $f=me$ with $m:I\hookrightarrow B$ the least [subobject](../../../category.md#subobject) through which $f$ factors, and $e:A\to I$ a [strong epimorphism](../../../category.md#strong-epimorphism). With [pullback in a category](../../../category.md#pullback-category-theory) constructions, the least-subobject characterization itself implies that $e$ is strong: in a lifting square against a [monomorphism](../../../category.md#monomorphism), pull that monomorphism back to $I$; since $e$ factors through this pullback, image minimality forces its mono into $I$ to be invertible, giving the required diagonal. Thus the two descriptions of images agree under the stated hypotheses.

For $a:A'\hookrightarrow A$, define $\exists_f(A')$ as the [image factorization](../../../category.md#image-factorization) subobject of $fa:A'\to B$. For $b:B'\hookrightarrow B$, the [pullback in a category](../../../category.md#pullback-category-theory) universal property and image minimality give

$$
\exists_f(A')\le B'\iff fa\text{ factors through }b
\iff A'\le f^*(B').
$$

Hence

$$
\boxed{\exists_f\dashv f^*.}
$$

This is an [adjunction](../../../category.md#adjoint-functors) between the [posets](../../../set.md#partially-ordered-set) of [subobjects](../../../category.md#subobject).

For [Frobenius reciprocity for subobjects](../../../category.md#frobenius-reciprocity-for-subobjects), factor $fa=me$ through its image $m:I\hookrightarrow B$, and put $P=I\times_BB'$. Its mono into $B$ represents $\exists_f(A')\cap B'$. The [pullback in a category](../../../category.md#pullback-category-theory) of $e$ along the [monomorphism](../../../category.md#monomorphism) $P\to I$ has domain canonically $A'\times_BB'$, which represents $A'\cap f^*(B')$. If [strong epimorphisms](../../../category.md#strong-epimorphism) are stable under pullback along [monomorphisms](../../../category.md#monomorphism), that pulled-back arrow is strong, so its composite with $P\hookrightarrow B$ is an [image factorization](../../../category.md#image-factorization). This gives

$$
\boxed{\exists_f(A'\cap f^*B')=\exists_f(A')\cap B'.}
$$

Equality here is equality of [subobjects](../../../category.md#subobject), hence an isomorphism of their representatives.

Conversely, let $e:X\to Y$ be a [strong epimorphism](../../../category.md#strong-epimorphism) and $b:B'\hookrightarrow Y$ be monic. Its image is all of $Y$: in any [image factorization](../../../category.md#image-factorization) of $e$, the lifting property makes the mono invertible. Apply [Frobenius reciprocity for subobjects](../../../category.md#frobenius-reciprocity-for-subobjects) to $f=e$ and $A'=X$. The induced [morphism](../../../algebra.md#morphism) $p:X\times_YB'\to B'$ has image all of $B'$, because the image of $bp$ in $Y$ is $B'$. Its [image factorization](../../../category.md#image-factorization) therefore has invertible mono, so $p$ is a [strong epimorphism](../../../category.md#strong-epimorphism). This proves the converse.

We now use the [glued ring categories counterexample to regularity](../../../category.md#glued-ring-categories-counterexample-to-regularity). All [rings](../../../commutative-algebra.md#ring) and [ring homomorphisms](../../../commutative-algebra.md#ring-homomorphism) are unital; the zero [ring](../../../commutative-algebra.md#ring), where $0=1$, is allowed. It is the [terminal object](../../../category.md#terminal-object) of $\mathbf{Rng}$, and there is no unital [ring homomorphism](../../../commutative-algebra.md#ring-homomorphism) from it to a nonzero [ring](../../../commutative-algebra.md#ring). Denote the common zero [ring](../../../commutative-algebra.md#ring) by $Z$, and the newly adjoined [strict initial object](../../../category.md#strict-initial-object) by $\bot$. Nonzero objects in different copies have no [morphisms](../../../algebra.md#morphism) between them. There is one [morphism](../../../algebra.md#morphism) from every object to $Z$ and from $\bot$ to every object, and no [morphism](../../../algebra.md#morphism) into $\bot$ except its identity.

Finite [products in a category](../../../category.md#product-category-theory) and [equalizers](../../../category.md#equaliser) can be described explicitly. The [terminal object](../../../category.md#terminal-object) is $Z$. The [product in a category](../../../category.md#product-category-theory) of two nonzero objects in one copy is their ordinary [ring](../../../commutative-algebra.md#ring) product; the [product in a category](../../../category.md#product-category-theory) of nonzero objects in different copies is $\bot$, since only $\bot$ can map to both. A product with $Z$ is the other factor, and one with $\bot$ is $\bot$. For parallel [morphisms](../../../algebra.md#morphism) between nonzero objects in the same copy, the ordinary ring [equalizer](../../../category.md#equaliser) works; it is nonzero because its subring contains distinct $0$ and $1$. All other parallel pairs are equal, and their [equalizer](../../../category.md#equaliser) is the identity of the domain. Thus the [construction of small limits from products and equalizers](../../../category.md#construction-of-small-limits-from-products-and-equalizers) gives all finite [categorical limits](../../../category.md#categorical-limit).

Within either ring copy, [monomorphisms](../../../category.md#monomorphism) are precisely injective [ring homomorphisms](../../../commutative-algebra.md#ring-homomorphism): maps from $\mathbb Z[x]$ detect unequal elements. The only monos from outside a copy are the maps $\bot\to X$, and the only [subobjects](../../../category.md#subobject) of $Z$ are $\bot$ and $Z$. Indeed a nonzero [ring](../../../commutative-algebra.md#ring) $R$ is not subterminal, since $\mathbb Z[x]\to R$ can send $x$ to $0$ or to $1$.

Ordinary ring-image factorizations remain [image factorizations](../../../category.md#image-factorization) in the glued [category](../../../category.md). Their surjective parts remain [strong epimorphisms](../../../category.md#strong-epimorphism): a lifting square into a nonzero ring stays in one copy; a square into $Z$ with mono $\bot\to Z$ would require a nonexistent map from a noninitial domain to $\bot$. Maps with domain $\bot$ are already monic and have identity strong part. Conversely, a [strong epimorphism](../../../category.md#strong-epimorphism) within a ring copy has surjective ring image, since its mono image part must be invertible. A map $\bot\to X$ with $X\ne\bot$ is monic but noninvertible, and therefore cannot be strong. This classifies the [strong epimorphisms](../../../category.md#strong-epimorphism) as the identities of $\bot$ and the surjective homomorphisms in the copies, including maps to $Z$.

Pullback along a [monomorphism](../../../category.md#monomorphism) within a copy preserves those surjections, using the given regularity of $\mathbf{Rng}$. Pullback along $\bot\to X$ gives $1_\bot$, and these exhaust the additional monos, including those into $Z$. Thus [strong epimorphisms](../../../category.md#strong-epimorphism) are stable under pullback along monos, so [Frobenius reciprocity for subobjects](../../../category.md#frobenius-reciprocity-for-subobjects) holds.

However, let $e:\mathbb Z_{\mathcal D}\to Z$ be the surjective [ring homomorphism](../../../commutative-algebra.md#ring-homomorphism) in the first copy, and pull it back along $\mathbb Z[x]_{\mathcal E}\to Z$ in the other copy. The resulting arrow is

$$
\bot\longrightarrow\mathbb Z[x]_{\mathcal E}.
$$

It is not even an [epimorphism](../../../category.md#epimorphism), since the distinct evaluation [ring homomorphisms](../../../commutative-algebra.md#ring-homomorphism) $x\mapsto0$ and $x\mapsto1$ to $\mathbb Z_{\mathcal E}$ agree after composing with $\bot\to\mathbb Z[x]_{\mathcal E}$. Since $e$ is strong, it would be a [regular epimorphism](../../../category.md#regular-epimorphism) in a [regular category](../../../category.md#regular-category), whose pullbacks must be regular, in particular epic. Therefore **the glued category has finite limits and images and satisfies Frobenius reciprocity, but is not regular**.

## 6

↑ **Parent:** [Paper 119](paper-119.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

A [pointed category](../../../category.md#pointed-category) has a [zero object](../../../category.md#zero-object), both initial and terminal. Factoring through that object gives a [zero morphism](../../../category.md#zero-morphism) $0_{A,B}$ between any two objects. In this paper a [semi-additive structure](../../../category-theory.md#commutative-monoid-enrichment) means [commutative-monoid enrichment](../../../category-theory.md#commutative-monoid-enrichment): every hom-set is a [commutative monoid](../../../algebra.md#commutative-monoid) with additive zero, and composition distributes over addition in both variables. No existence of finite [products in a category](../../../category.md#product-category-theory) is included in this last definition. This convention matters for the final one-object example; under the stronger convention requiring finite [biproducts](../../../category-theory.md#biproduct), that example would not be a [semi-additive category](../../../category-theory.md#semi-additive-category).

Let $c_{A,B}:A+B\to A\times B$ be the given canonical isomorphism. Transfer the coproduct injections across $c_{A,B}$, so $A\times B$ is also a [coproduct in a category](../../../category.md#coproduct), with injections

$$
i_1=\langle1_A,0\rangle,\qquad i_2=\langle0,1_B\rangle.
$$

Write $\nabla_B:B\times B\to B$ for the [morphism](../../../algebra.md#morphism) whose composites with $i_1,i_2$ are both $1_B$. For $f,g:A\to B$, define the [biproduct-induced addition of morphisms](../../../category-theory.md#biproduct-induced-addition-of-morphisms) by

$$
\boxed{f+g=\nabla_B\langle f,g\rangle=[1_B,1_B]c_{B,B}^{-1}\langle f,g\rangle.}
$$

The zero is the existing [zero morphism](../../../category.md#zero-morphism). We verify the laws from the universal properties, without assuming addition in advance.

All finite canonical maps from coproducts to products are isomorphisms, by induction from the binary ones and the [zero object](../../../category.md#zero-object). Thus both $(B\times B)\times B$ and $B\times(B\times B)$ are ternary [coproducts in a category](../../../category.md#coproduct). The two iterated fold maps to $B$ agree on each of the three injections, hence are equal. Applying this to $\langle f,g,h\rangle$ gives associativity. The interchange $B\times B\to B\times B$ swaps the two injections, so its composite with $\nabla_B$ is $\nabla_B$, giving commutativity. Finally $\langle f,0\rangle=i_1f$, so $f+0=f$, and similarly $0+f=f$.

Precomposition is additive because $\langle f,g\rangle u=\langle fu,gu\rangle$. For $v:B\to C$, the [morphisms](../../../algebra.md#morphism) $v\nabla_B$ and $\nabla_C(v\times v)$ agree on both injections, so they agree; consequently $v(f+g)=vf+vg$. Composition with a [zero morphism](../../../category.md#zero-morphism) is zero. This proves the [commutative-monoid enrichment](../../../category-theory.md#commutative-monoid-enrichment).

It is unique. In any such enrichment, the additive zero morphisms agree with the pointed ones, since each map to or from the [zero object](../../../category.md#zero-object) belongs to a singleton hom-set. The projections of $i_1p_1+i_2p_2$ from $A\times B$ are respectively $p_1,p_2$ by bilinearity, so

$$
i_1p_1+i_2p_2=1_{A\times B}.
$$

For $A=B$, composing on the left by $\nabla_B$ and on the right by $\langle f,g\rangle$ forces the displayed formula for $f+g$. Thus **the biproducts determine exactly one such enrichment**.

For the last part, the underlying one-object [category](../../../category.md) has endomorphism [monoid](../../../algebra.md#monoid) $(\mathbb N,\cdot)$, including $0$, and identity $1$. Its usual addition gives a [commutative-monoid enrichment](../../../category-theory.md#commutative-monoid-enrichment). Any permutation $\sigma$ of the [prime numbers](../../../number-theory.md#prime-number) extends, by unique [prime factorization](../../../number-theory.md#fundamental-theorem-of-arithmetic), to a multiplicative [monoid automorphism](../../../algebra.md#monoid-automorphism) $\phi_\sigma:\mathbb N\to\mathbb N$, fixing $0,1$. Transport addition by

$$
\boxed{a\mathbin{\oplus_\sigma}b=\phi_\sigma^{-1}\bigl(\phi_\sigma(a)+\phi_\sigma(b)\bigr).}
$$

This is a [commutative monoid](../../../algebra.md#commutative-monoid) operation with zero $0$, and multiplication distributes over it: applying $\phi_\sigma$ reduces each distributive law to the ordinary one in $\mathbb N$. Thus each operation supplies a [semi-additive structure](../../../category-theory.md#commutative-monoid-enrichment) on the same fixed composition law.

For each [odd prime](../../../number-theory.md#odd-prime) $p$, take $\sigma$ to interchange $2$ and $p$, fixing every other prime. Then

$$
1\mathbin{\oplus_\sigma}1=\phi_\sigma^{-1}(2)=p.
$$

Different choices of $p$ give different additions, and there are infinitely many [prime numbers](../../../number-theory.md#prime-number). Hence there are **infinitely many distinct semi-additive structures**, even though these transported structures are isomorphic as enriched [categories](../../../category.md). The underlying one-object [category](../../../category.md) has no [terminal object](../../../category.md#terminal-object), because its endomorphism [set](../../../set.md) is not a singleton, so it indeed has no finite [products in a category](../../../category.md#product-category-theory).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2017](../../2017.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
