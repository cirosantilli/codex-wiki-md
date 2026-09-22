<h1 id="11/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write the [adjunction unit](../../../../../../unit-of-an-adjunction.md) and [adjunction counit](../../../../../../counit-of-an-adjunction.md) of $F\dashv G$ as $\eta,\varepsilon$. Its induced [monad](../../../../../../monad.md) is $T=GF$, with multiplication $\mu=G\varepsilon_F$. The [Eilenberg-Moore comparison functor](../../../../../../eilenberg-moore-comparison-functor.md) is

$$
K(d)=(Gd,a_d),\qquad a_d=G\varepsilon_d:T(Gd)\to Gd,\qquad K(h)=Gh.
$$

The unit law for $a_d$ is $G\varepsilon_d\eta_{Gd}=1_{Gd}$, a [triangle identity for an adjunction](../../../../../../triangle-identities-for-an-adjunction.md). [Naturality](../../../../../../naturality.md) of $\varepsilon$ at $\varepsilon_d$ gives $\varepsilon_dFG\varepsilon_d=\varepsilon_d\varepsilon_{FGd}$; applying $G$ gives $a_dTa_d=a_d\mu_{Gd}$. [Naturality](../../../../../../naturality.md) at $h$ gives the [monad algebra morphism](../../../../../../morphism-of-algebras-for-a-monad.md) equation for $Gh$. Thus $K$ is well-defined.

For each $d$, consider the fork in $\mathcal D$

$$
FGFGd\ \substack{\xrightarrow{\varepsilon_{FGd}}\\[-2pt]\xrightarrow[FG\varepsilon_d]{}}\ FGd\xrightarrow{\varepsilon_d}d.
$$

It commutes by the [naturality](../../../../../../naturality.md) equation just used. Its image under $G$ is the fork $T^2(Gd)\rightrightarrows T(Gd)\to Gd$ of the preceding question, with parallel [morphisms](../../../../../../morphism.md) $\mu_{Gd},Ta_d$ and final map $a_d$. It is split using $s=\eta_{Gd}$ and $t=\eta_{T(Gd)}$. By the assumed reflection, **$\varepsilon_d$ is the [coequalizer](../../../../../../coequalizer.md) of this pair in $\mathcal D$**.

For faithfulness, if $Gh=Gk$ for $h,k:d\to e$, [naturality](../../../../../../naturality.md) gives $h\varepsilon_d=\varepsilon_eFGh=\varepsilon_eFGk=k\varepsilon_d$. A [coequalizer](../../../../../../coequalizer.md) is an [epimorphism](../../../../../../epimorphism.md), so $h=k$.

For fullness, let $u:K(d)\to K(e)$ be a [monad algebra morphism](../../../../../../morphism-of-algebras-for-a-monad.md). Thus $u:Gd\to Ge$ satisfies $u a_d=a_eTu$. [Set](../../../../../../set-split.md) $v=\varepsilon_eF u:FGd\to e$. We verify explicitly that $v$ equalizes the two [morphisms](../../../../../../morphism.md) of the displayed fork. The [monad algebra morphism](../../../../../../morphism-of-algebras-for-a-monad.md) equation gives

$$
vFG\varepsilon_d=\varepsilon_eF(uG\varepsilon_d)
=\varepsilon_eFG\varepsilon_e\,FGF u.
$$

[Naturality](../../../../../../naturality.md) of $\varepsilon$ first at $Fu$ and then at $\varepsilon_e$ gives

$$
v\varepsilon_{FGd}=\varepsilon_e\varepsilon_{FGe}\,FGF u
=\varepsilon_eFG\varepsilon_e\,FGF u.
$$

The [coequalizer](../../../../../../coequalizer.md) therefore supplies a unique $h:d\to e$ with $h\varepsilon_d=v$. Applying $G$ yields $Gh\,a_d=Gv=a_eTu=u a_d$. The map $a_d$ is split epic with section $\eta_{Gd}$, so cancellation gives $Gh=u$. This proves fullness, and the earlier cancellation proves faithfulness. Hence

$$
\boxed{K:\mathcal D\to\mathcal C^T\text{ is full and faithful}.}
$$

No claim that $K$ is essentially surjective is needed; that stronger conclusion needs the corresponding existence hypotheses.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [11](../../11.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
