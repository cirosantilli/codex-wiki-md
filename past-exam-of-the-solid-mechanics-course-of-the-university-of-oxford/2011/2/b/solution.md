<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The surface element relation is [Nanson's formula](../../../../nanson-s-formula.md). The [force](../../../../force-split.md) on a corresponding pair of current and reference surface elements must agree:

$$
t\,da=(S\circ y)n\,da=(S\circ y)\operatorname{cof}F\,N\,dA=T N\,dA.
$$

Therefore the first [Piola-Kirchhoff stress tensor](../../../../piola-kirchhoff-stress-tensors.md) is

$$
\boxed{T=(S\circ y)\operatorname{cof}F=J(S\circ y)F^{-T}.}
$$

It measures [force](../../../../force-split.md) per reference [area](../../../../surface-area.md), with a current [force](../../../../force-split.md) direction and a reference normal direction.

In components, differentiate $T_{iA}=S_{ij}(y(x))(\operatorname{cof}F)_{jA}$. The [Piola identity](../../../../piola-identity.md) says $\partial_A(\operatorname{cof}Dy)_{jA}=0$. One proof writes the [cofactor matrix](../../../../cofactor-matrix.md) as $\frac12\varepsilon_{jkl}\varepsilon_{ABC}y_{k,B}y_{l,C}$; differentiating in $A$ produces symmetric second [derivatives](../../../../derivative.md) contracted against antisymmetric epsilon symbols, hence zero. The [chain rule](../../../../chain-rule.md) consequently gives

$$
\partial_AT_{iA}=\frac{\partial S_{ij}}{\partial y_k}(y)F_{kA}(\operatorname{cof}F)_{jA}
=J\frac{\partial S_{ij}}{\partial y_j}(y),
$$

since $F_{kA}(\operatorname{cof}F)_{jA}=J\delta_{kj}$. Thus, with the coordinate composition made explicit,

$$
\boxed{\operatorname{Div}_xT=J(\operatorname{div}_yS)\circ y.}
$$

The distinction between reference [divergence](../../../../divergence.md) and current [divergence](../../../../divergence.md) is essential to this identity.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the solid mechanics course of the University of Oxford](../../../split.md)
5. [Solid mechanics course of the University of Oxford](../../../../solid-mechanics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
