<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Put $P(A)=\Omega^A$, the [power object](../../../../../power-object.md), with $P(f)$ acting by inverse image of predicates. Transposing a predicate on $A\times B$ gives natural bijections

$$
\mathcal E(A,PB)\cong\operatorname{Sub}(A\times B)\cong\mathcal E(B,PA).
$$

Thus $P^{\mathrm{op}}:\mathcal E\to\mathcal E^{\mathrm{op}}$ is left adjoint to $P:\mathcal E^{\mathrm{op}}\to\mathcal E$. Its unit $\eta_A:A\to PPA$ sends $a$ to evaluation at $a$, namely the predicate $S\mapsto(a\in S)$. This unit is monic: two generalized elements having the same evaluation on all predicates agree by testing the singleton predicate of the first, or equivalently its graph in the relevant parameter product.

We verify a sufficient form of [Beck's monadicity theorem](../../../../../beck-s-monadicity-theorem.md): a right adjoint is monadic if it reflects [isomorphisms](../../../../../isomorphism.md) and its domain has, and it preserves, [coequalizers](../../../../../coequalizer.md) of reflexive pairs. Suppose $Pf$ is invertible. Then $PPf$ is invertible, and naturality of the monic unit shows that $f$ is monic. Regard it as the [subobject](../../../../../subobject.md) $A\hookrightarrow B$. Its characteristic predicate and the constantly true predicate have the same restriction to $A$, so injectivity of $Pf$ makes them equal. Thus this [subobject](../../../../../subobject.md) is all of $B$, and $f$ is invertible. Hence $P$ reflects [isomorphisms](../../../../../isomorphism.md).

A reflexive pair in $\mathcal E^{\mathrm{op}}$ is a coreflexive pair $f,g:B\rightrightarrows A$ in $\mathcal E$, with a common retraction $r$ such that $rf=rg=1_B$. Its [equalizer](../../../../../equaliser.md) $e:E\hookrightarrow B$ exists. We show that $Pe:PB\to PE$ is the [coequalizer](../../../../../coequalizer.md) of $Pf,Pg:PA\rightrightarrows PB$. Direct image of [subobjects](../../../../../subobject.md) along the mono $f$ defines $\exists_f:PB\to PA$, and similarly $\exists_e:PE\to PB$. At every parameter object the identities are

$$
Pf\,\exists_f=1_{PB},\qquad Pg\,\exists_f=\exists_ePe,\qquad Pe\,\exists_e=1_{PE}.
$$

For the middle identity, an equality $f(b)=g(b')$ forces $b=b'$ after applying $r$; their common point must therefore lie in the [equalizer](../../../../../equaliser.md). This proves the identity for parameterized predicates, not merely for global elements. If $h:PB\to Z$ satisfies $hPf=hPg$, composing with $\exists_f$ gives $h=h\exists_ePe$. Thus it factors through $Pe$, and the last displayed identity gives uniqueness. This proves that [power objects turn coreflexive equalizers into coequalizers](../../../../../power-objects-turn-coreflexive-equalizers-into-coequalizers.md). All hypotheses of the monadicity criterion have now been checked, so **$P$ is monadic**, with

$$
\boxed{\mathcal E^{\mathrm{op}}\simeq\mathcal E^{PP}.}
$$

A [logical functor](../../../../../logical-functor.md) $L:\mathcal E\to\mathcal F$ preserves [finite limits](../../../../../finite-limit.md), exponentials and the classifier, hence gives compatible natural [isomorphisms](../../../../../isomorphism.md) $LP\cong PL$ and $LPP\cong PPL$. They respect units and multiplications, because these are defined by evaluation and transposition. Under the displayed equivalences, $L^{\mathrm{op}}$ is therefore the induced functor on double-power [Eilenberg-Moore categories](../../../../../eilenberg-moore-category.md). Their forgetful functors create [finite limits](../../../../../finite-limit.md), and the underlying $L$ preserves them. Consequently the induced functor preserves [finite limits](../../../../../finite-limit.md), so $L^{\mathrm{op}}$ does too. Reversing arrows proves **every [logical functor](../../../../../logical-functor.md) preserves finite [colimits](../../../../../colimit.md)**.

For the first counterexample, the constant-terminal functor $F:\mathbf{Set}\to\mathbf{Set}$ has the constant-empty functor as left adjoint: both sets of maps in the [adjunction](../../../../../adjoint-functors.md) are singletons. It preserves exponentials, since $F(B^A)=1=1^1=(FB)^{FA}$ with the canonical comparison. It does not preserve the [initial object](../../../../../initial-object.md), because $F(0)=1$. Thus preservation of exponentials alone is insufficient.

For the second, take the fixed-point functor $\Gamma:G\text{-}\mathbf{Set}\to\mathbf{Set}$ for $G=\mathbb Z/2$. Its left adjoint gives a set the trivial action. The classifier of $G$-sets is the two-element set with trivial action, so $\Gamma$ preserves it and its truth map. Let $X$ be the free two-element $G$-set. The [coequalizer](../../../../../coequalizer.md) of its identity and its swapping automorphism is the singleton $G$-set. Applying $\Gamma$ gives two maps $0\rightrightarrows0$ followed by $1$, whereas their [coequalizer](../../../../../coequalizer.md) in sets is $0$. Thus **$\Gamma$ preserves the classifier but not all finite [colimits](../../../../../colimit.md)**. These examples also explain why both requirements in logicalness matter.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
