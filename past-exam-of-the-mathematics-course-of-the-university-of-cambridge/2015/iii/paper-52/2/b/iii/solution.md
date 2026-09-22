<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For the [minimally coupled scalar field](../../../../../../../minimally-coupled-scalar-field.md), keep the [metric tensor](../../../../../../../metric-tensor.md) fixed and vary $\phi$. A scalar's first [covariant derivative](../../../../../../../covariant-derivative.md) equals its ordinary derivative, so

$$
\delta S=\int_M\sqrt{-g}\left[-\nabla^\mu\phi\,\nabla_\mu\delta\phi-V'(\phi)\delta\phi\right]d^4x.
$$

Apply [integration by parts for tensor fields](../../../../../../../integration-by-parts-for-tensor-fields.md). The boundary contribution is proportional to $\delta\phi$ and vanishes under the given boundary condition, leaving

$$
\delta S=\int_M\sqrt{-g}\,[\Box\phi-V'(\phi)]\delta\phi\,d^4x.
$$

The interior variation is arbitrary. Thus **the scalar equation of motion is**

$$
\boxed{\Box\phi-V'(\phi)=0,\qquad
\Box\phi=\frac1{\sqrt{-g}}\partial_\mu(\sqrt{-g}\,g^{\mu\nu}\partial_\nu\phi).}
$$

Here the [d'Alembert operator](../../../../../../../d-alembert-operator.md) contains the [Levi-Civita connection](../../../../../../../levi-civita-connection.md) in the second [covariant derivative](../../../../../../../covariant-derivative.md), even though the first derivative of the [scalar field](../../../../../../../scalar-field.md) is ordinary.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 52](../../../../paper-52-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
