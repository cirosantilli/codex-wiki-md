<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [fiber monodromy](../../../../../../fiber-monodromy.md) is **periodic when isotopy is allowed to move the boundary**, in the sense of a [periodic surface homeomorphism](../../../../../../periodic-surface-homeomorphism.md). Here is a justification from the [Seifert fibered space](../../../../../../seifert-fibered-space.md) structure, rather than a special formula about [torus knots](../../../../../../torus-knot.md). Its base is a disk with cone-point orders $p,q$. The fiber [Seifert surface](../../../../../../seifert-surface.md) is an [incompressible surface](../../../../../../incompressible-surface.md) because its inclusion in the [mapping torus](../../../../../../mapping-torus.md) is injective on [fundamental groups](../../../../../../fundamental-group.md). It is also a [boundary-incompressible surface](../../../../../../boundary-incompressible-surface.md): lift a proposed boundary-compressing disk to the [infinite cyclic cover](../../../../../../infinite-cyclic-cover-of-a-knot-exterior.md) $\Sigma\times\mathbb R$ and project to $\Sigma$. This would homotope an essential arc of $\Sigma$ into $\partial\Sigma$, contradicting its essentiality. The [classification of incompressible surfaces in Seifert fibered spaces](../../../../../../classification-of-incompressible-surfaces-in-seifert-fibered-spaces.md) therefore applies. A [vertical surface in a Seifert fibered space](../../../../../../vertical-surface-in-a-seifert-fibered-space.md) has zero intersection with a regular [Seifert fiber](../../../../../../seifert-fiber.md), whereas the fibration class evaluates on $f=pq\,m$ as $pq$. Thus the [Seifert surface](../../../../../../seifert-surface.md) is isotopic to a [horizontal surface in a Seifert fibered space](../../../../../../horizontal-surface-in-a-seifert-fibered-space.md), with $pq$ intersections per regular orbit.

Following the oriented [Seifert fibers](../../../../../../seifert-fiber.md) from one intersection to the next gives a first-return [homeomorphism](../../../../../../homeomorphism.md) of the horizontal [topological surface](../../../../../../topological-surface.md). It is a representative of the [fiber monodromy](../../../../../../fiber-monodromy.md), and its $pq$-th power is the identity. It has order $pq$: a regular orbit meets the connected [horizontal surface in a Seifert fibered space](../../../../../../horizontal-surface-in-a-seifert-fibered-space.md) in $pq$ cyclically ordered points. This realizes the periodic case of the [Nielsen–Thurston classification theorem](../../../../../../nielsen-thurston-classification.md). It is neither an [Anosov homeomorphism](../../../../../../anosov-homeomorphism.md) nor a [pseudo-Anosov homeomorphism](../../../../../../pseudo-anosov-map.md).

There is a boundary convention here. A representative fixed pointwise on the boundary is not periodic relative to the boundary: its $pq$-th power is a boundary [Dehn twist](../../../../../../dehn-twist.md) (with sign determined by the return-map convention). Capping the boundary, or allowing it to rotate during [isotopy](../../../../../../isotopy.md), gives the finite-order representative intended by “periodic”. This distinguishes periodic surface type from literal finite order in the mapping class group relative to the boundary.

For any [fibered knot](../../../../../../fibered-knot.md), its [Alexander module](../../../../../../alexander-module-of-a-knot.md) is $H_1(\Sigma;\mathbb Z)$ with the deck transformation given by [homological monodromy](../../../../../../homological-monodromy.md), so its [Alexander polynomial of a knot](../../../../../../alexander-polynomial.md) is $\det(tI-\phi_*)$ up to a unit. The general [Turaev torsion](../../../../../../turaev-torsion.md) relation $\Delta(t)\doteq(1-t)\tau(X)$ and part (b) therefore give

$$
\Delta(t)\doteq P(t):=\frac{(1-t)(1-t^{pq})}{(1-t^p)(1-t^q)}.
$$

This rational expression is a [polynomial](../../../../../../polynomial-split.md): in its factorization into [cyclotomic polynomials](../../../../../../cyclotomic-polynomial.md), $\gcd(p,q)=1$ cancels all denominator factors. It is monic, has constant coefficient one, and has [polynomial degree](../../../../../../degree-of-a-polynomial.md) $pq+1-p-q=(p-1)(q-1)$. The [characteristic polynomial](../../../../../../characteristic-polynomial.md) has [polynomial degree](../../../../../../degree-of-a-polynomial.md) $2g$, is monic, and has constant coefficient $\det\phi_*=1$, because [homological monodromy](../../../../../../homological-monodromy.md) preserves the [intersection form](../../../../../../intersection-form.md). These facts remove the unit ambiguity and give

$$
\boxed{\det(\phi_*-tI)=\frac{(1-t)(1-t^{pq})}{(1-t^p)(1-t^q)},\qquad
g=\frac{(p-1)(q-1)}2.}
$$

The sign change between $\det(\phi_*-tI)$ and $\det(tI-\phi_*)$ is trivial because $\operatorname{rank}H_1(\Sigma)=2g$ is even. As a separate geometric check, the [orbifold Euler characteristic](../../../../../../orbifold-euler-characteristic.md) of the base is $1/p+1/q-1$, and its $pq$-sheeted [horizontal surface in a Seifert fibered space](../../../../../../horizontal-surface-in-a-seifert-fibered-space.md) has [Euler characteristic](../../../../../../euler-characteristic.md) $\chi(\Sigma)=p+q-pq=1-2g$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 141](../../../paper-141-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
