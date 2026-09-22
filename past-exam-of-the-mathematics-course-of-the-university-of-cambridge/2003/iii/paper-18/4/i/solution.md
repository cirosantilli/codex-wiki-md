<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $T:\mathcal C^{\mathrm{op}}\times\mathcal C\to\mathcal D$. An [end of a functor](../../../../../../end-of-a-functor.md) is an object $E$ with maps $e_C:E\to T(C,C)$ satisfying $T(1_C,f)e_C=T(f,1_D)e_D$ for every $f:C\to D$, universal among all such families. Thus every compatible family with vertex $A$ factors uniquely through $E$. Write it as $\int_CT(C,C)$. These are the wedge equations for a [dinatural transformation](../../../../../../dinatural-transformation.md) from a constant [functor](../../../../../../functor.md) to $T$.

Dually, a [coend of a functor](../../../../../../coend-of-a-functor.md) is an object $Q$ with maps $i_C:T(C,C)\to Q$ satisfying $i_CT(f,1_C)=i_DT(1_D,f)$ as maps from $T(D,C)$, universal among compatible families with a common target. Write it as $\int^CT(C,C)$. These are cowedge equations, and every cowedge to $A$ factors uniquely through $Q$.

For small $\mathcal C$, if the needed products and [equalizers](../../../../../../equaliser.md) exist, the end is the [equalizer](../../../../../../equaliser.md) of $\prod_CT(C,C)\rightrightarrows\prod_{f:C\to D}T(C,D)$. If the needed coproducts and [coequalizers](../../../../../../coequalizer.md) exist, the coend is the [coequalizer](../../../../../../coequalizer.md) of $\coprod_{f:C\to D}T(D,C)\rightrightarrows\coprod_CT(C,C)$. The two arrows in each construction are precisely the two sides of the compatibility equation. This explains both the mixed variance and the [universal property](../../../../../../universal-property.md), rather than treating the integral notation as an ordinary numerical integral.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
