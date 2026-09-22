<h1 id="6/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Given the two [natural transformations](../../../../../../natural-transformation.md), define

$$
\alpha(f)=Gf\,\eta_C,\qquad\beta(g)=\varepsilon_DFg.
$$

[Naturality](../../../../../../naturality.md) of $\eta$ and the second [triangle identity for an adjunction](../../../../../../triangle-identities-for-an-adjunction.md) give

$$
\alpha\beta(g)=G\varepsilon_D\,GFg\,\eta_C=G\varepsilon_D\,\eta_{GD}\,g=g.
$$

[Naturality](../../../../../../naturality.md) of $\varepsilon$ and the first [triangle identity for an adjunction](../../../../../../triangle-identities-for-an-adjunction.md) give

$$
\beta\alpha(f)=\varepsilon_D\,FGf\,F\eta_C=f\,\varepsilon_{FC}\,F\eta_C=f.
$$

The maps are natural in $C,D$, since the defining compositions commute with precomposition in $C$ and postcomposition in $D$ by [naturality](../../../../../../naturality.md) of $\eta,\varepsilon$. They therefore define an [adjunction](../../../../../../adjoint-functors.md) $F\dashv G$. Their values on [identity morphisms](../../../../../../identity-morphism.md) recover precisely $\eta,\varepsilon$. Conversely any [adjunction](../../../../../../adjoint-functors.md) with these [unit and counit of an adjunction](../../../../../../unit-and-counit-of-an-adjunction.md) must have the same transpose formulas, so it is **unique with the prescribed unit and counit**.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [6](../../6.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
