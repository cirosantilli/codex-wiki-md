<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the given [bimonoids](../../../../../../bimonoid.md), use right [comodules](../../../../../../comodule.md). The [corestriction functor for comodules](../../../../../../corestriction-functor-for-comodules.md) associated to a [comonoid morphism](../../../../../../comonoid-morphism.md) $f:H\to K$ keeps underlying objects and [morphisms](../../../../../../morphism.md), and replaces a [coaction](../../../../../../coaction.md) $\rho_M$ by $(1\otimes f)\rho_M$. The comonoid-morphism axioms ensure that this is a $K$-coaction.

The tensor [coaction](../../../../../../coaction.md) for two $H$-[comodules](../../../../../../comodule.md) in the ambient [braided monoidal category](../../../../../../braided-monoidal-category.md) is

$$
\rho_{M\otimes N}=(1_M\otimes1_N\otimes m_H)(1_M\otimes c_{H,N}\otimes1_H)(\rho_M\otimes\rho_N),
$$

and the unit [coaction](../../../../../../coaction.md) is $j_H:I\to H$. If $f$ is also a [monoid morphism](../../../../../../monoid-morphism.md), then $fm_H=m_K(f\otimes f)$ and $fj_H=j_K$. Substituting these identities, and using [naturality](../../../../../../naturality.md) of the ambient [braiding](../../../../../../braiding.md), shows that corestriction preserves both tensor and unit coactions exactly. Its structural maps are identities, so it is a [strict monoidal functor](../../../../../../strict-monoidal-functor.md).

Conversely, suppose this induced [functor](../../../../../../functor.md) is strict monoidal. Apply equality of the tensor coactions to the two regular right [comodules](../../../../../../comodule.md) $(H,\Delta_H)$. Then apply $\varepsilon_H\otimes\varepsilon_H$ to their two underlying $H$ factors. The counit laws and [naturality](../../../../../../naturality.md) of the [braiding](../../../../../../braiding.md) remove those factors and leave

$$
fm_H=m_K(f\otimes f).
$$

Equality on the unit [comodule](../../../../../../comodule.md) similarly gives $fj_H=j_K$. Thus $f$ is a [monoid morphism](../../../../../../monoid-morphism.md). **The criterion is exactly**

$$
\boxed{f_*\text{ is strict monoidal}\iff f\text{ preserves multiplication and unit}.}
$$

The regular-comodule argument uses only the counit laws; it requires no elementwise or finite-dimensional assumption on the ambient category.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 122](../../../paper-122-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
