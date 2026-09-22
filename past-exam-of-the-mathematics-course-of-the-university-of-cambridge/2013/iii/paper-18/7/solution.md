<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

The [crude monadicity theorem](../../../../../crude-monadicity-theorem.md) in its reflexive-coequalizer form says: if $F\dashv G:\mathcal D\to\mathcal C$, $G$ is a [conservative functor](../../../../../conservative-functor.md), $\mathcal D$ has [reflexive coequalizers](../../../../../reflexive-coequalizer.md), and $G$ preserves them, then the [Eilenberg-Moore comparison functor](../../../../../eilenberg-moore-comparison-functor.md) $K:\mathcal D\to\mathcal C^T$, for $T=GF$, is an [equivalence of categories](../../../../../equivalence-of-categories.md). Requiring all [coequalizers](../../../../../coequalizer.md) to exist and be preserved is a stronger sufficient form.

For an algebra $(A,a)$, form in $\mathcal D$ the [coequalizer](../../../../../coequalizer.md)

$$
FTA\mathrel{\substack{\xrightarrow{Fa}\\\xrightarrow[\varepsilon_{FA}]{} }}FA\xrightarrow{q}L(A,a).
$$

The pair is a [reflexive pair](../../../../../reflexive-pair.md) with common section $F\eta_A$: both composites are the identity by the algebra unit law and the triangle identity. An arrow $u:FA\to B$ transposes to $v=Gu\eta_A:A\to GB$. The two composites $uFa$ and $u\varepsilon_{FA}$ transpose to $va$ and $G\varepsilon_BTv$, respectively. Indeed the latter transpose is $Gu\mu_A\eta_{TA}=Gu$, while $G\varepsilon_BTv=Gu\mu_AT\eta_A=Gu$ by counit naturality. Thus $u$ equalizes the pair exactly when $v$ is an [monad algebra morphism](../../../../../morphism-of-algebras-for-a-monad.md) $(A,a)\to K(B)$. The [coequalizer](../../../../../coequalizer.md) property gives natural [bijections](../../../../../bijection.md)

$$
\mathcal D(L(A,a),B)\cong\mathcal C^T((A,a),K(B)).
$$

These define $L$ on arrows by uniqueness, so $L\dashv K$. Its unit has underlying arrow $\beta=Gq\eta_A:A\to GL(A,a)$.

By preservation, $Gq$ coequalizes $Ta$ and $\mu_A$ in $\mathcal C$. The action $a:TA\to A$ is a [split coequalizer](../../../../../split-coequalizer.md) of that pair: take $s=\eta_A$ and $t=\eta_{TA}$, with $\mu_At=1_{TA}$ and $Ta\,t=\eta_Aa$. Thus there is a unique [isomorphism](../../../../../isomorphism.md) $\alpha:GL(A,a)\to A$ with $\alpha Gq=a$. We have $\alpha\beta=a\eta_A=1_A$. Also

$$
Gq=Gq\mu_A\eta_{TA}=GqTa\eta_{TA}=Gq\eta_Aa=\beta a.
$$

Consequently $\beta\alpha Gq=Gq$, and epimorphic cancellation gives $\beta\alpha=1$. The adjunction unit $\beta$ is an [monad algebra morphism](../../../../../morphism-of-algebras-for-a-monad.md); its invertible underlying arrow has an algebra-morphism inverse. Thus the unit of $L\dashv K$ is an [isomorphism](../../../../../isomorphism.md).

For its counit $c_B:LK(B)\to B$, the triangle identity gives $K(c_B)\beta_{K(B)}=1_{K(B)}$. Hence $K(c_B)$, and therefore $G(c_B)$, is an [isomorphism](../../../../../isomorphism.md). Since $G$ is a [conservative functor](../../../../../conservative-functor.md), $c_B$ is an [isomorphism](../../../../../isomorphism.md) too. Both unit and counit of $L\dashv K$ are invertible, which proves the claimed equivalence. This proof uses only reflexive [coequalizers](../../../../../coequalizer.md) in $\mathcal D$ and split [coequalizers](../../../../../coequalizer.md) in $\mathcal C$.

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 18](../../paper-18-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
