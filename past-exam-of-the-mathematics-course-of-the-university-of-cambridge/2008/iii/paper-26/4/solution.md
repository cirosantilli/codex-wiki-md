<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [balanced category](../../../../../balanced-category.md) is one in which every morphism that is both monic and epic is an [isomorphism](../../../../../isomorphism.md). If a [faithful functor](../../../../../faithful-functor.md) sends $f$ to an [isomorphism](../../../../../isomorphism.md), then $f$ is monic: equality $fg=fh$ becomes $FfFg=FfFh$, cancellation gives $Fg=Fh$, and faithfulness gives $g=h$. The same argument on the other side makes $f$ epic. Balance therefore makes $f$ an [isomorphism](../../../../../isomorphism.md). Thus a [faithful functor](../../../../../faithful-functor.md) out of a [balanced category](../../../../../balanced-category.md) reflects [isomorphisms](../../../../../isomorphism.md).

Under the [adjunction](../../../../../adjoint-functors.md), the transpose of $Ff:FX\to FA$ is $\eta_A f:X\to GFA$. Hence if $F$ is faithful, $\eta_Af=\eta_Ag$ forces $Ff=Fg$ and then $f=g$, making every $\eta_A$ monic. Conversely, if the unit is pointwise monic and $Ff=Fg$, naturality gives $\eta_Bf=GFf\,\eta_A=GFg\,\eta_A=\eta_Bg$, whence $f=g$. Therefore

$$
\boxed{F\text{ faithful}\iff\eta\text{ pointwise monic}.}
$$

We also use the standard [adjunction](../../../../../adjoint-functors.md) fact with its justification: $F$ is full and faithful exactly when $\eta$ is invertible. Indeed the composite hom-set map $\mathcal C(X,A)\to\mathcal D(FX,FA)\cong\mathcal C(X,GFA)$ is postcomposition by $\eta_A$. If $F$ is full and faithful these maps are bijective; taking $X=GFA$ produces a right inverse, and taking $X=A$ gives injectivity and therefore a left inverse. Conversely an invertible unit makes these hom-set maps bijective.

For the final example, view the two-element ordered set $0<1$ as a [category](../../../../../category-split.md) $\mathcal C$, and let $\mathcal D$ have one object and only its identity. The unique $F:\mathcal C\to\mathcal D$ is left adjoint to the [functor](../../../../../functor.md) $G$ selecting $1$, since every $\mathcal C(x,1)$ is a singleton. Every arrow in an ordered-set [category](../../../../../category-split.md) is monic, so the unit arrows $x\to1$ and the identity counit are monic. But $F$ is not full: $\mathcal C(1,0)$ is empty whereas $\mathcal D(F1,F0)$ is a singleton. The example does not contradict the upcoming equivalence because $\mathcal C$ is not balanced; its arrow $0\to1$ is both monic and epic but not invertible.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 26](../../paper-26-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
