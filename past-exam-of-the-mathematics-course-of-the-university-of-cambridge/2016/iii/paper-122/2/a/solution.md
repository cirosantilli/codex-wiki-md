<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An [opmonoidal functor](../../../../../../opmonoidal-functor.md) $F:(\mathcal C,\otimes,I)\to(\mathcal D,\otimes,J)$ consists of a [functor](../../../../../../functor.md), a [natural transformation](../../../../../../natural-transformation.md)

$$
F_2(X,Y):F(X\otimes Y)\longrightarrow FX\otimes FY,
$$

and a [morphism](../../../../../../morphism.md) $F_0:FI\to J$. These maps need not be invertible. If $\alpha,\lambda,\rho$ are the respective [associators](../../../../../../associator.md) and [unitors](../../../../../../unitor.md), its axioms are

$$
\alpha^{\mathcal D}(F_2(X,Y)\otimes1)F_2(X\otimes Y,Z)=(1\otimes F_2(Y,Z))F_2(X,Y\otimes Z)F(\alpha^{\mathcal C}),
$$



$$
\lambda^{\mathcal D}(F_0\otimes1)F_2(I,X)=F(\lambda^{\mathcal C}),\qquad\rho^{\mathcal D}(1\otimes F_0)F_2(X,I)=F(\rho^{\mathcal C}).
$$

The first equation has domain $F((X\otimes Y)\otimes Z)$ and codomain $FX\otimes(FY\otimes FZ)$, which fixes the direction of every arrow. This is also called a [colax monoidal functor](../../../../../../opmonoidal-functor.md).

An [opmonoidal natural transformation](../../../../../../opmonoidal-natural-transformation.md) $\tau:F\Rightarrow G$ between [opmonoidal functors](../../../../../../opmonoidal-functor.md) is a [natural transformation](../../../../../../natural-transformation.md) satisfying

$$
\boxed{G_2(X,Y)\tau_{X\otimes Y}=(\tau_X\otimes\tau_Y)F_2(X,Y),\qquad G_0\tau_I=F_0.}
$$

**It respects both the tensor and unit comparison maps.** These are [commutative diagrams](../../../../../../commutative-diagram.md) and a unit [commutative diagram](../../../../../../commutative-diagram.md); the arrow directions are opposite to those for a [lax monoidal functor](../../../../../../monoidal-functor.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 122](../../../paper-122-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
