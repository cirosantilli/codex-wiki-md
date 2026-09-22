<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Write $\eta:1_{\mathcal C}\to GF$ and $\varepsilon:FG\to1_{\mathcal D}$ for the [unit and counit of an adjunction](../../../../../unit-and-counit-of-an-adjunction.md). The induced [monad](../../../../../monad.md) has

$$
T=GF,\qquad \mu=G\varepsilon F:T^2\to T.
$$

The [Eilenberg-Moore comparison functor](../../../../../eilenberg-moore-comparison-functor.md) sends $D\in\mathcal D$ to the [algebra for a monad](../../../../../algebra-for-a-monad.md)

$$
K(D)=(GD,G\varepsilon_D),
$$

and sends $v:D\to D'$ to $Gv$. The [triangle identities for an adjunction](../../../../../triangle-identities-for-an-adjunction.md) give the algebra unit law, and naturality of the counit gives the algebra multiplication law and the algebra-morphism equation for $Gv$.

If $\mathcal D$ has [coequalizers](../../../../../coequalizer.md), define the [Left adjoint to the Eilenberg-Moore comparison functor](../../../../../left-adjoint-to-the-eilenberg-moore-comparison-functor.md) at an algebra $(A,a:TA\to A)$ by

$$
FTA\mathrel{\substack{\xrightarrow{Fa}\\[-2pt]\xrightarrow[\varepsilon_{FA}]{} }}FA\xrightarrow{q}L(A,a).
$$

The parallel pair is reflexive through $F\eta_A$. A [morphism](../../../../../morphism.md) $L(A,a)\to D$ is equivalently an arrow $b:FA\to D$ with $bFa=b\varepsilon_{FA}$. Under $F\dashv G$, its transpose is $\bar b=Gb\,\eta_A:A\to GD$. The transpose of $bFa$ is $\bar b\,a$, while the transpose of $b\varepsilon_{FA}$ is $G\varepsilon_D\,T\bar b$. Hence the coequalizer condition is exactly

$$
\bar b\,a=G\varepsilon_D\,T\bar b,
$$

the equation for a [morphism of algebras for a monad](../../../../../morphism-of-algebras-for-a-monad.md) $(A,a)\to K(D)$. This supplies the natural bijection proving **$L\dashv K$**, and also defines $L$ on algebra morphisms by the coequalizer universal property.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 21](../../paper-21-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
