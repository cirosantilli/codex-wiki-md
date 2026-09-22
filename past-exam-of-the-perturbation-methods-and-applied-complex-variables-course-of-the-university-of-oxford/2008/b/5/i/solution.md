<h1 id="b/5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Near a [prevertex of a Schwarz-Christoffel map](../../../../../prevertex-of-a-schwarz-christoffel-map.md) $X_j$, a [conformal map](../../../../../conformal-map.md) to an interior angle $(1-\beta_j)\pi$ has local form

$$
f(Z)-f(X_j)\sim c_j(Z-X_j)^{1-\beta_j}.
$$

Its [derivative](../../../../../derivative.md) therefore has the factor $(Z-X_j)^{-\beta_j}$. On each real interval between [prevertex](../../../../../prevertex-of-a-schwarz-christoffel-map.md), the argument of the product of these factors is constant, so its integral traces a straight polygon side. Passing a [prevertex of a Schwarz-Christoffel map](../../../../../prevertex-of-a-schwarz-christoffel-map.md) changes the argument by the prescribed exterior angle $\beta_j\pi$. Thus

$$
\boxed{f'(Z)=C\prod_{j=1}^n(Z-X_j)^{-\beta_j}}
$$

has exactly the required straight sides and corner angles, with the branches chosen in the [upper half-plane](../../../../../upper-half-plane-complex-analysis.md). Equivalently $f''/f'$ has simple [poles](../../../../../pole.md) $-\beta_j/(Z-X_j)$; removing them leaves the constant normalization determined by behavior at infinity. The additive integration constant translates the polygon and $C$ rotates and scales it. This is the [Schwarz-Christoffel formula](../../../../../schwarz-christoffel-mapping.md).

The automorphisms of the [upper half-plane](../../../../../upper-half-plane-complex-analysis.md) are real [Möbius transformations](../../../../../mobius-transformation.md) with positive determinant, modulo a common nonzero scalar. They have three real degrees of freedom, so **three [prevertex of a Schwarz-Christoffel map](../../../../../prevertex-of-a-schwarz-christoffel-map.md) positions may be assigned independently**. The remaining positions are constrained by the side-length ratios.

If $X_n=\infty$, omit its finite factor:

$$
\boxed{f'(Z)=C\prod_{j<n}(Z-X_j)^{-\beta_j}.}
$$

Since $\sum_j\beta_j=2$, the [derivative](../../../../../derivative.md) behaves like $Z^{\beta_n-2}$ at infinity; in the coordinate $U=1/Z$, this is exactly the required corner exponent there. Thus the missing angle is encoded by behavior at infinity.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the perturbation methods and applied complex variables course of the University of Oxford](../../../../split.md)
6. [Perturbation methods and applied complex variables course of the University of Oxford](../../../../../perturbation-methods-and-applied-complex-variables-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
