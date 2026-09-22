<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [monad](../../../../../monad.md) on $\mathcal C$ consists of an [endofunctor](../../../../../endofunctor.md) $T$ and [natural transformations](../../../../../natural-transformation.md) $\eta:1\to T$, $\mu:T^2\to T$ satisfying $\mu\,T\eta=\mu\,\eta T=1_T$ and $\mu\,T\mu=\mu\,\mu T$. Its [Eilenberg-Moore category](../../../../../eilenberg-moore-category.md) has objects $(X,a)$ with $a:TX\to X$, $a\eta_X=1_X$ and $a\mu_X=aTa$. A morphism $f:(X,a)\to(Y,b)$ satisfies $fa=bTf$. An [adjunction](../../../../../adjoint-functors.md) $F\dashv G$, with unit $\eta$ and counit $\varepsilon$, induces $T=GF$, $\mu=G\varepsilon F$. It is a [monadic adjunction](../../../../../monadic-adjunction.md) if the [Eilenberg-Moore comparison functor](../../../../../eilenberg-moore-comparison-functor.md) $K(D)=(GD,G\varepsilon_D)$ is an equivalence with the [Eilenberg-Moore category](../../../../../eilenberg-moore-category.md).

A fork $A\overset{p,q}{\rightrightarrows}B\overset{r}{\to}C$ is a [split coequalizer](../../../../../split-coequalizer.md) if $rp=rq$ and there are $s:C\to B$, $t:B\to A$ with $rs=1$, $pt=1$ and $qt=sr$. It is indeed a [coequalizer](../../../../../coequalizer.md): if $hp=hq$, then $h=hpt=hqt=hsr$, so $h$ factors uniquely through $r$, which is split epic. Every [functor](../../../../../functor.md) preserves these splitting identities, making such [coequalizers](../../../../../coequalizer.md) absolute.

The [precise monadicity theorem](../../../../../beck-s-monadicity-theorem.md) states: for an [adjunction](../../../../../adjoint-functors.md) $F:\mathcal C\rightleftarrows\mathcal D:G$, the comparison is an equivalence if and only if $G$ reflects [isomorphisms](../../../../../isomorphism.md) and every pair in $\mathcal D$ whose $G$-image admits a [split coequalizer](../../../../../split-coequalizer.md) has a [coequalizer](../../../../../coequalizer.md) which $G$ preserves. Equivalently, the right adjoint creates these split-underlying [coequalizers](../../../../../coequalizer.md), with creation understood up to the canonical [isomorphism](../../../../../isomorphism.md) of the prescribed underlying [coequalizer](../../../../../coequalizer.md). Here is a proof.

First consider the forgetful [functor](../../../../../functor.md) from [monad algebras](../../../../../algebra-for-a-monad.md). It reflects [isomorphisms](../../../../../isomorphism.md): the inverse of an invertible algebra morphism also obeys the algebra-morphism identity, by multiplying that identity by the inverses. For an algebra pair with a split underlying [coequalizer](../../../../../coequalizer.md) $r:B\to C$, all powers of $T$ preserve its [coequalizer](../../../../../coequalizer.md). If $b:TB\to B$ is the algebra structure on $B$, the map $rb$ coequalizes $Tp,Tq$, so there is a unique $c:TC\to C$ with

$$
cTr=rb.
$$

The unit law follows by composing with the [epimorphism](../../../../../epimorphism.md) $r$: $c\eta_Cr=cTr\eta_B=rb\eta_B=r$. For associativity, naturality and the algebra law give

$$
c\mu_C T^2r=cTr\mu_B=rb\mu_B=rbTb=cT(rb)=cTcT^2r.
$$

Cancel the [epimorphism](../../../../../epimorphism.md) $T^2r$ to obtain $c\mu_C=cTc$. Thus $(C,c)$ is an algebra and $r$ is an algebra morphism. Any algebra morphism coequalizing the pair factors through $r$ on underlying objects, and its factor is an algebra morphism by cancellation of the [epimorphism](../../../../../epimorphism.md) $Tr$. This creates the [coequalizer](../../../../../coequalizer.md). Transporting these facts through an equivalence proves necessity.

For sufficiency, let $(X,a)$ be a $T$-algebra. In $\mathcal D$ consider the free pair

$$
FTX\ \underset{Fa}{\overset{\varepsilon_{FX}}{\rightrightarrows}}\ FX.
$$

Its underlying pair is $\mu_X,Ta:T^2X\rightrightarrows TX$, with [split coequalizer](../../../../../split-coequalizer.md) $a:TX\to X$: the splittings are $s=\eta_X$ and $t=\eta_{TX}$, using the algebra unit law, the [monad](../../../../../monad.md) unit law and naturality of $\eta$. By hypothesis its [coequalizer](../../../../../coequalizer.md) $q:FX\to D$ exists and is preserved. Identify $GD$ with $X$ by the unique [coequalizer](../../../../../coequalizer.md) [isomorphism](../../../../../isomorphism.md), so $Gq=a$. Naturality of the counit makes $Kq$ an algebra morphism, hence the comparison structure $c$ on $GD$ satisfies $cTa=a\mu_X=aTa$. The map $Ta$ is split epic because $a\eta_X=1$, so $c=a$. Every algebra is therefore isomorphic to a comparison algebra.

For an actual object $D$, its counit $\varepsilon_D:FGD\to D$ is a [coequalizer](../../../../../coequalizer.md) of the analogous free pair. It coequalizes that pair by counit naturality. Compare it with the [coequalizer](../../../../../coequalizer.md) furnished by the hypothesis; applying $G$ gives an [isomorphism](../../../../../isomorphism.md), since both underlying arrows coequalize the same split pair. Reflection of [isomorphisms](../../../../../isomorphism.md) makes the comparison map an [isomorphism](../../../../../isomorphism.md). This proves the counit's asserted [coequalizer](../../../../../coequalizer.md) property.

Let $f:KD\to KE$ be an algebra morphism. Its transpose is $h_0=\varepsilon_EFf:FGD\to E$. The two composites of $h_0$ with the free pair have adjunct transposes $G\varepsilon_E\,Tf$ and $fG\varepsilon_D$, equal because $f$ is an algebra morphism. Consequently $h_0$ factors uniquely through $\varepsilon_D$ as $h:D\to E$. Applying $G$ gives $(Gh)G\varepsilon_D=fG\varepsilon_D$; the last factor is split epic, so $Gh=f$. Conversely any lift of $f$ must satisfy $h\varepsilon_D=\varepsilon_EFf$ by naturality and hence is unique. Thus $K$ is full and faithful, and the earlier construction makes it essentially surjective. The comparison is an equivalence, completing the theorem's proof.

Now take $G:\mathbf{CompHaus}\to\mathbf{Set}$. Its left adjoint exists by the permitted topological result; it can be realized as the [Stone-Čech compactification](../../../../../stone-cech-compactification.md) of the discrete input set. A bijective [continuous map](../../../../../continuous-map.md) from a [compact space](../../../../../compact-space.md) to a [Hausdorff space](../../../../../hausdorff-space.md) is a [homeomorphism](../../../../../homeomorphism.md), so $G$ reflects [isomorphisms](../../../../../isomorphism.md).

For continuous $f,g:X\rightrightarrows Y$ with a split underlying fork $q,s,t$, let $R$ be the relation of having the same $q$-image. We claim

$$
R=\{(f(x),f(x')):g(x)=g(x')\}.
$$

For the forward inclusion choose $x=t(y)$, $x'=t(y')$: $ft=1$ and $gt=sq$ supply the equality. For the reverse inclusion use $qf=qg$. The subset $\{(x,x'):g(x)=g(x')\}\subset X^2$ is closed, because $Y$ is Hausdorff, and compact. Its continuous image $R\subset Y^2$ is compact and hence closed. A closed [equivalence relation](../../../../../equivalence-relation.md) on a [compact Hausdorff space](../../../../../compact-hausdorff-space.md) has a compact Hausdorff quotient; its quotient map is a [coequalizer](../../../../../coequalizer.md) here, since it identifies exactly the generated relation. Its underlying set [coequalizer](../../../../../coequalizer.md) is the specified one up to the unique [isomorphism](../../../../../isomorphism.md). Thus $G$ preserves the needed [coequalizers](../../../../../coequalizer.md), and

$$
\boxed{\mathbf{CompHaus}\rightleftarrows\mathbf{Set}\text{ is a monadic adjunction}.}
$$

The closedness argument is the [closed relation generated by a set-split pair of compact Hausdorff maps](../../../../../closed-relation-generated-by-a-set-split-pair-of-compact-hausdorff-maps.md) lemma; the splitting maps themselves need not be continuous.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 26](../../paper-26-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
