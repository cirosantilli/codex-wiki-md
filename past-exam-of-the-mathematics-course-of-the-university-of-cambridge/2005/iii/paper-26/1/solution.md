<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [monad](../../../../../monad.md) on a [category](../../../../../category-split.md) $\mathcal C$ consists of an [endofunctor](../../../../../endofunctor.md) $T$, a unit [natural transformation](../../../../../natural-transformation.md) $\eta:1_{\mathcal C}\Rightarrow T$, and a multiplication $\mu:T^2\Rightarrow T$, satisfying

$$
\mu\,T\mu=\mu\,\mu T,\qquad \mu\,T\eta=1_T=\mu\,\eta T.
$$

An [algebra for a monad](../../../../../algebra-for-a-monad.md) is $(A,a:TA\to A)$ with $a\eta_A=1_A$ and $aTa=a\mu_A$. A [morphism of algebras for a monad](../../../../../morphism-of-algebras-for-a-monad.md) $h:(A,a)\to(B,b)$ satisfies $ha=bTh$. These objects and arrows form the [Eilenberg-Moore category](../../../../../eilenberg-moore-category.md) $\mathcal C^T$.

For an [adjunction](../../../../../adjoint-functors.md) $F:\mathcal C\rightleftarrows\mathcal D:U$ with $F\dashv U$, the [monad induced by an adjunction](../../../../../monad-induced-by-an-adjunction.md) is $T=UF$, with $\mu=U\varepsilon F$. The [Eilenberg-Moore comparison functor](../../../../../eilenberg-moore-comparison-functor.md) is $K(D)=(UD,U\varepsilon_D)$ and $K(h)=Uh$. The [functor](../../../../../functor.md) $U$ is monadic when this comparison is an [equivalence of categories](../../../../../equivalence-of-categories.md); this is a [monadic adjunction](../../../../../monadic-adjunction.md).

The [precise monadicity theorem](../../../../../beck-s-monadicity-theorem.md) says that $U:\mathcal D\to\mathcal C$ is monadic exactly when it has a [left adjoint](../../../../../adjoint-functors.md), reflects [isomorphisms](../../../../../isomorphism.md), and satisfies the following condition: whenever the image of a parallel pair in $\mathcal D$ admits a [split coequalizer](../../../../../split-coequalizer.md) in $\mathcal C$, the pair has a [coequalizer](../../../../../coequalizer.md) in $\mathcal D$ and $U$ preserves that [coequalizer](../../../../../coequalizer.md). Equivalently, these [coequalizers](../../../../../coequalizer.md) are created up to the canonical [isomorphism](../../../../../isomorphism.md) identifying their underlying [coequalizer](../../../../../coequalizer.md) objects. Here a [split coequalizer](../../../../../split-coequalizer.md) of $f,g:A\rightrightarrows B$ consists of $q:B\to Q$, $s:Q\to B$, and $t:B\to A$ with

$$
qf=qg,\qquad qs=1_Q,\qquad ft=1_B,\qquad gt=sq.
$$

These equations prove its [universal property](../../../../../universal-property.md): if $hf=hg$, then $h=hft=hgt=hsq$, and $hs$ is the unique factor through $q$. Every [functor](../../../../../functor.md) preserves these equations, so every [functor](../../../../../functor.md) preserves [split coequalizers](../../../../../split-coequalizer.md).

First consider the forgetful [functor](../../../../../functor.md) $U^T:\mathcal C^T\to\mathcal C$. It has the [free algebra functor](../../../../../free-algebra-functor.md) $A\mapsto(TA,\mu_A)$ as a [left adjoint](../../../../../adjoint-functors.md): the inverse transposition formulas are $h\mapsto h\eta_A$ and $v\mapsto bTv$. An [monad algebra morphism](../../../../../morphism-of-algebras-for-a-monad.md) whose underlying arrow is invertible has an algebra-morphism inverse, by rearranging its structure equation. Thus $U^T$ reflects [isomorphisms](../../../../../isomorphism.md).

Suppose $f,g:(A,a)\rightrightarrows(B,b)$ have an underlying [split coequalizer](../../../../../split-coequalizer.md) $q:B\to Q$. Applying $T$ gives a [coequalizer](../../../../../coequalizer.md) of $Tf,Tg$. The equation $qbTf=qfa=qga=qbTg$ therefore gives a unique $c:TQ\to Q$ with $cTq=qb$. The [monad algebra](../../../../../algebra-for-a-monad.md) laws follow by cancellation: composing $c\eta_Q=1_Q$ with the [epimorphism](../../../../../epimorphism.md) $q$ reduces it to $b\eta_B=1_B$, and composing $cTc=c\mu_Q$ with $T^2q$ reduces it to $bTb=b\mu_B$. Both $Tq$ and $T^2q$ are [epimorphisms](../../../../../epimorphism.md) because they remain split [coequalizers](../../../../../coequalizer.md). Thus $(Q,c)$ is an [algebra for a monad](../../../../../algebra-for-a-monad.md) and $q$ is an [monad algebra morphism](../../../../../morphism-of-algebras-for-a-monad.md). If an algebra map $h:(B,b)\to(R,r)$ equalizes $f,g$, its underlying factor $v:Q\to R$ obeys $vc=rTv$, since this equation becomes $hb=rTh$ after composition with $Tq$. This proves that $U^T$ creates the required [coequalizers](../../../../../coequalizer.md). An [equivalence of categories](../../../../../equivalence-of-categories.md) transfers these properties to any monadic $U$, proving necessity.

Conversely assume the three conditions and write $T=UF$. Given $(A,a)\in\mathcal C^T$, take the pair

$$
FTA\mathrel{\substack{\xrightarrow{\varepsilon_{FA}}\\[-2pt]\xrightarrow[Fa]{}}}FA.
$$

Its image is $\mu_A,Ta:T^2A\rightrightarrows TA$, with [split coequalizer](../../../../../split-coequalizer.md) $a:TA\to A$: the splittings are $s=\eta_A$ and $t=\eta_{TA}$, because

$$
a\eta_A=1_A,\qquad \mu_A\eta_{TA}=1_{TA},\qquad Ta\,\eta_{TA}=\eta_Aa.
$$

Let $q:FA\to D_a$ be its [coequalizer](../../../../../coequalizer.md) in $\mathcal D$. Preservation gives a canonical [isomorphism](../../../../../isomorphism.md) $UD_a\cong A$ under which $Uq=a$. Transporting the algebra action of $K(D_a)$ along this [isomorphism](../../../../../isomorphism.md) gives $\alpha:TA\to A$. Naturality of the [adjunction counit](../../../../../counit-of-an-adjunction.md) says that $K(q)$ is an [monad algebra morphism](../../../../../morphism-of-algebras-for-a-monad.md), hence $\alpha Ta=a\mu_A$. But $aTa=a\mu_A$ too, and $Ta$ is a [split epimorphism](../../../../../split-epimorphism.md), with section $T\eta_A$. Therefore $\alpha=a$. Every algebra is consequently isomorphic to some $K(D_a)$.

It remains to establish full faithfulness, rather than merely construct objects. For $B\in\mathcal D$, put $b=U\varepsilon_B$. The [adjunction counit](../../../../../counit-of-an-adjunction.md) $\varepsilon_B:FUB\to B$ coequalizes $\varepsilon_{FUB},Fb$. The [coequalizer](../../../../../coequalizer.md) supplied by the hypothesis has underlying [coequalizer](../../../../../coequalizer.md) $b:TUB\to UB$. The induced arrow from that [coequalizer](../../../../../coequalizer.md) object to $B$ is therefore sent by $U$ to an [isomorphism](../../../../../isomorphism.md); reflection of [isomorphisms](../../../../../isomorphism.md) makes it invertible. Thus $\varepsilon_B$ itself is this [coequalizer](../../../../../coequalizer.md).

Now let $h:K(B)\to K(C)$ be an [monad algebra morphism](../../../../../morphism-of-algebras-for-a-monad.md), and put $c=U\varepsilon_C$. The arrow $v=\varepsilon_CFh:FUB\to C$ coequalizes the two arrows in the preceding presentation. To check this directly, use transposition along $F\dashv U$: the transposes of $vFb$ and $v\varepsilon_{FUB}$ are respectively $hb$ and $cTh$, which agree by the algebra-morphism equation. Hence a unique $\bar h:B\to C$ satisfies $\bar h\varepsilon_B=v$. Applying $U$ gives $(U\bar h)b=cTh=hb$; cancellation of the [split epimorphism](../../../../../split-epimorphism.md) $b$ yields $U\bar h=h$. Finally, any arrow $r:B\to C$ satisfies $r\varepsilon_B=\varepsilon_CFU r$ by naturality, so two arrows with equal image under $U$ are equal by the [coequalizer](../../../../../coequalizer.md) property. The comparison is [full and faithful](../../../../../full-and-faithful-functor.md) and essentially surjective, hence an [equivalence of categories](../../../../../equivalence-of-categories.md). This proves the theorem.

For the application, the free [compact Hausdorff space](../../../../../compact-hausdorff-space.md) on a [set](../../../../../set-split.md) $S$ is the [Stone-Čech compactification](../../../../../stone-cech-compactification.md) $\beta(S_{\mathrm{disc}})$ of the corresponding [discrete space](../../../../../discrete-space.md). Its standard extension property says that every set map $S\to UX$, for compact Hausdorff $X$, extends uniquely to a [continuous map](../../../../../continuous-map.md) $\beta S\to X$. This constructs the required [left adjoint](../../../../../adjoint-functors.md). Also a continuous bijection from a compact space to a Hausdorff space is a [homeomorphism](../../../../../homeomorphism.md), so $U$ reflects [isomorphisms](../../../../../isomorphism.md).

Take [continuous maps](../../../../../continuous-map.md) $f,g:X\rightrightarrows Y$ whose underlying functions have a [split coequalizer](../../../../../split-coequalizer.md) $q:Y\to Q$ with splittings $s,t$. The splittings need not be continuous. Let

$$
E=\{(f(x),g(x)):x\in X\}\subseteq Y\times Y,\qquad R=\{(y,z):q(y)=q(z)\}.
$$

The set $E$ is compact and hence closed. Since $qf=qg$, it is contained in $R$. Conversely $(y,sq(y))=(ft(y),gt(y))\in E$. Thus

$$
R=\{(y,z):\exists w\in Y,\ (y,w)\in E,\ (z,w)\in E\}.
$$

The set of triples on the right is closed in the [compact Hausdorff space](../../../../../compact-hausdorff-space.md) $Y^3$, so its projection onto the first two coordinates is compact and closed. This proves that the [equivalence relation](../../../../../equivalence-relation.md) $R$ is closed, without assuming continuity of either splitting.

Give $Q\cong Y/R$ the [quotient topology](../../../../../quotient-topology.md). The allowed closed-relation criterion makes it a [compact Hausdorff space](../../../../../compact-hausdorff-space.md). If a [continuous map](../../../../../continuous-map.md) $h:Y\to Z$ equalizes $f,g$, the split-coequalizer property makes it constant on the fibres of $q$; its unique factor $Q\to Z$ is continuous by the quotient [topology](../../../../../topology-split.md). Hence this is a [coequalizer](../../../../../coequalizer.md) in [compact Hausdorff spaces](../../../../../compact-hausdorff-space.md), preserved by $U$. Its [topology](../../../../../topology-split.md) is forced uniquely, since any continuous surjection from a compact space to a Hausdorff space is a quotient map. All three conditions hold, and therefore **the forgetful functor from compact Hausdorff spaces to sets is monadic**.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 26](../../paper-26-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
