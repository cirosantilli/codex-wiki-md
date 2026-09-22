<h1 id="9/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $F\dashv U$ with [unit of an adjunction](../../../../../../unit-of-an-adjunction.md) $\eta$ and [counit of an adjunction](../../../../../../counit-of-an-adjunction.md) $\varepsilon$, put

$$
\boxed{T=UF,\qquad\mu_A=U(\varepsilon_{FA}).}
$$

The [triangle identities for an adjunction](../../../../../../triangle-identities-for-an-adjunction.md) give

$$
\mu_A\eta_{TA}=1_{TA},\qquad
\mu_AT(\eta_A)=1_{TA}.
$$

For associativity, [naturality](../../../../../../naturality.md) of $\varepsilon$ at $\varepsilon_{FA}:FUFA\to FA$ says

$$
\varepsilon_{FA}FU(\varepsilon_{FA})
=\varepsilon_{FA}\varepsilon_{FUFA}.
$$

Apply $U$ to obtain $\mu_AT(\mu_A)=\mu_A\mu_{TA}$. Thus this is the [monad induced by an adjunction](../../../../../../monad-induced-by-an-adjunction.md).

Conversely, start with a [monad](../../../../../../monad.md) $(T,\eta,\mu)$. The [free algebra functor](../../../../../../free-algebra-functor.md) sends $A$ to $(TA,\mu_A)$ and $f$ to $Tf$. The [monad](../../../../../../monad.md) laws ensure that these are [algebras for a monad](../../../../../../algebra-for-a-monad.md) and [morphisms of algebras for a monad](../../../../../../morphism-of-algebras-for-a-monad.md). For an algebra $(B,b)$, there are inverse [bijections](../../../../../../bijection.md)

$$
\mathcal C^T((TA,\mu_A),(B,b))\cong\mathcal C(A,B),
\qquad g\longmapsto g\eta_A,\quad f\longmapsto bT(f).
$$

The inverse really is an algebra map because

$$
bT(f)\mu_A=b\mu_B T^2(f)=bT(b)T^2(f)=bT(bT(f)).
$$

For a free-algebra map $g$, its algebra equation and the [monad](../../../../../../monad.md) unit law give

$$
bT(g\eta_A)=bT(g)T(\eta_A)=g\mu_AT(\eta_A)=g.
$$

For a base map $f$, naturality and the algebra unit law give $bT(f)\eta_A=b\eta_Bf=f$. The formulas are natural, establishing the [free-forgetful Eilenberg-Moore adjunction](../../../../../../free-forgetful-eilenberg-moore-adjunction.md) $F^T\dashv U^T$. Its unit is $\eta_A$, and its counit at $(B,b)$ is $b$. Hence its induced multiplication is $\mu$, and **every monad arises from an adjunction**.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [9](../../9.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
