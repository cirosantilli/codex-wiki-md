<h1 id="b/4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

At a vertex with exterior turning angle $\beta_j\pi$, the interior angle is $(1-\beta_j)\pi$. A local [conformal map](../../../../../conformal-map.md) from a half-plane therefore behaves as $f(Z)-z_j\sim c_j(Z-X_j)^{1-\beta_j}$, so its [derivative](../../../../../derivative.md) has local exponent $-\beta_j$.

On each real boundary interval between prevertices, $\arg f'$ is constant because the image is a straight side. Across a prevertex its change is the exterior turning angle. Taking $\arg(Z-X_j)\in(0,\pi)$, the product $\prod_j(Z-X_j)^{-\beta_j}$ has exactly these changes. Dividing $f'$ by that product removes the corner singularities and leaves a holomorphic nonzero function with constant boundary argument. Schwarz reflection and the regular behavior at infinity make it constant. This gives the [Schwarz-Christoffel formula](../../../../../schwarz-christoffel-mapping.md)

$$
\boxed{f'(Z)=C\prod_{j=1}^n(Z-X_j)^{-\beta_j}.}
$$

There are **three freely normalizable real prevertices**, because an automorphism of the [upper half-plane](../../../../../upper-half-plane-complex-analysis.md) has three real parameters. After those are fixed, the remaining $n-3$ prevertex parameters are determined by the polygon's shape through the side-length conditions. They are not further independent normalization choices.

If the last prevertex is at infinity, absorb its constant scale into $C$ and omit its finite factor:

$$
\boxed{f'(Z)=C\prod_{j=1}^{n-1}(Z-X_j)^{-\beta_j}.}
$$

For a bounded polygon, $\sum_j\beta_j=2$, so this [derivative](../../../../../derivative.md) behaves like $Z^{\beta_n-2}$, consistent with the corner described in the local coordinate $1/Z$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the perturbation methods and applied complex variables course of the University of Oxford](../../../../split.md)
6. [Perturbation methods and applied complex variables course of the University of Oxford](../../../../../perturbation-methods-and-applied-complex-variables-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
