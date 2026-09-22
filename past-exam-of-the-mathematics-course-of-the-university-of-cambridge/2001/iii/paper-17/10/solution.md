<h1 id="10/solution">Solution</h1>

↑ **Parent:** [10](../10.md)

A form of [Beck's monadicity theorem](../../../../../beck-s-monadicity-theorem.md) compatible with equivalence-based [monadic adjunctions](../../../../../monadic-adjunction.md) is this. A [functor](../../../../../functor.md) $U:\mathcal D\to\mathcal C$ is monadic exactly when it has a [left adjoint](../../../../../adjoint-functors.md), is a [conservative functor](../../../../../conservative-functor.md), and $\mathcal D$ has [coequalizers](../../../../../coequalizer.md) of all pairs whose images under $U$ admit a [split coequalizer](../../../../../split-coequalizer.md), with $U$ preserving these coequalizers. In the strict lifting formulation, one states creation of these coequalizers. Such a pair is a [functor-split coequalizer pair](../../../../../functor-split-coequalizer-pair.md); the splitting is required in the base category, not necessarily upstairs.

A [split coequalizer](../../../../../split-coequalizer.md) fork $A\mathrel{\substack{\xrightarrow{r}\\[-0.4ex]\xrightarrow[s]{}}}B\xrightarrow{q}Q$ has maps $u:B\to A$ and $t:Q\to B$ such that

$$
qr=qs,\qquad qt=1_Q,\qquad ru=1_B,\qquad su=tq.
$$

Every [functor](../../../../../functor.md) preserves this [coequalizer](../../../../../coequalizer.md): if $hr=hs$, then $h=hru=hsu=htq$, and $q$ is split epic, so the factor through $q$ is unique. The same equations remain true after applying any functor.

For necessity, let $U^T:\mathcal C^T\to\mathcal C$ be the [monad algebra](../../../../../algebra-for-a-monad.md) forgetful functor. It has the free-algebra [left adjoint](../../../../../adjoint-functors.md). It reflects [isomorphisms](../../../../../isomorphism.md), because if an algebra map $f$ is invertible in $\mathcal C$, the equation $fa=bTf$ rearranges to $f^{-1}b=aT(f^{-1})$.

If two algebra maps $r,s:(A,a)\rightrightarrows(B,b)$ have an underlying [split coequalizer](../../../../../split-coequalizer.md) $q:B\to Q$, then $Tq$ and $T^2q$ are also coequalizers. Since $qb$ equalizes $Tr,Ts$, there is a unique $c:TQ\to Q$ satisfying

$$
cTq=qb.
$$

After composing with the [epimorphism](../../../../../epimorphism.md) $q$, the equation $c\eta_Q=1_Q$ reduces to the unit law for $b$. After composing with the epimorphism $T^2q$, the equation $cT(c)=c\mu_Q$ reduces to $bT(b)=b\mu_B$. Thus $(Q,c)$ is an algebra and $q$ an algebra map. If an algebra map $h:(B,b)\to(Z,z)$ equalizes $r,s$, its unique underlying factor $k:Q\to Z$ satisfies $kc=zTk$: this follows by precomposing with the epimorphism $Tq$. Therefore this is a coequalizer upstairs as well. This proves that the [monad algebra forgetful functor creates split coequalizers](../../../../../monad-algebra-forgetful-functor-creates-split-coequalizers.md). The same properties transport through the comparison [equivalence of categories](../../../../../equivalence-of-categories.md), with the object-lifting convention distinguished in Question 9.

For sufficiency, suppose the three conditions hold, choose $F\dashv U$, and let $T=UF$ with comparison $K$. For each algebra $(X,a)$, consider the pair

$$
FTX\mathrel{\substack{\xrightarrow{F(a)}\\[-0.4ex]\xrightarrow[\varepsilon_{FX}]{}}}FX.
$$

Its image has coequalizer $a:TX\to X$. It is split: take $r=\mu_X$, $s=T(a)$, $q=a$, $u=\eta_{TX}$ and $t=\eta_X$. The [monad](../../../../../monad.md) and algebra laws give

$$
a\mu_X=aT(a),\quad a\eta_X=1_X,\quad
\mu_X\eta_{TX}=1_{TX},\quad T(a)\eta_{TX}=\eta_Xa.
$$

By hypothesis the pair has a coequalizer $q:FX\to D_X$ and $Uq$ is also a coequalizer. Identify $UD_X$ with $X$ using the unique coequalizer isomorphism, so $Uq=a$. Since $q$ is carried by $K$ to an algebra map from the free algebra, the transported action $b:TX\to X$ satisfies

$$
bT(a)=a\mu_X=aT(a).
$$

But $T(a)$ is a [split epimorphism](../../../../../split-epimorphism.md), with right inverse $T(\eta_X)$, so $b=a$. Hence $(X,a)\cong K(D_X)$: the comparison is essentially surjective.

Next, for every $D\in\mathcal D$, put $a_D=U\varepsilon_D$. The [counit of an adjunction](../../../../../counit-of-an-adjunction.md) coequalizes

$$
FTUD\mathrel{\substack{\xrightarrow{F(a_D)}\\[-0.4ex]\xrightarrow[\varepsilon_{FUD}]{}}}FUD.
$$

This follows from naturality of the counit. The image pair has the split coequalizer $a_D$, as above. If $q:FUD\to Q$ is the hypothesized preserved coequalizer, the induced map $h:Q\to D$ has $Uh$ invertible because both $Uq$ and $a_D$ coequalize the same pair. Conservativity makes $h$ invertible. Therefore $\varepsilon_D$ itself is a coequalizer.

Let $f:K(D)\to K(E)$ be an algebra map, so $fa_D=a_ETf$. Set $g=\varepsilon_EF(f):FUD\to E$. Under the [adjunction](../../../../../adjoint-functors.md) transpose bijection, the two composites of $g$ with the displayed presentation pair correspond respectively to $fa_D$ and $a_ETf$. They are equal, so $g$ factors uniquely through $\varepsilon_D$, giving $h:D\to E$ with $h\varepsilon_D=g$. Applying $U$ yields

$$
Uh\,a_D=a_ETf=fa_D.
$$

Since $a_D$ is split epic, $Uh=f$. Thus $K$ is full. If $Uh=Uk$, the transposes of $h\varepsilon_D$ and $k\varepsilon_D$ are equal, so those composites agree. The counit is epic, hence $h=k$; thus $K$ is faithful.

The comparison is full, faithful and essentially surjective, so it is an [equivalence of categories](../../../../../equivalence-of-categories.md). **This proves monadicity.** The argument also explains the role of each hypothesis: split base presentations construct all algebras, and reflection of isomorphisms turns the counit presentations into actual coequalizers upstairs.

## ↑ Ancestors (10)

1. [10](../10.md)
2. [Paper 17](../../paper-17-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
