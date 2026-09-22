<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [Weinstein neighborhood theorem](../../../../../../weinstein-neighborhood-theorem.md): a neighborhood of a compact [Lagrangian submanifold](../../../../../../lagrangian-submanifold.md) is [symplectomorphic](../../../../../../symplectomorphism.md) to a neighborhood of the zero section of its [cotangent bundle](../../../../../../cotangent-bundle.md), with the identification equal to the identity on that submanifold. Take the canonical sign $-d\lambda$ in this identification. We also use [C1 openness of diffeomorphisms](../../../../../../c1-openness-of-diffeomorphisms.md): on a compact manifold, all smooth self-maps sufficiently close in the $C^1$ topology to a fixed [diffeomorphism](../../../../../../diffeomorphism.md) are themselves [diffeomorphisms](../../../../../../diffeomorphism.md).

In $M\times M$ put $\Omega=-\operatorname{pr}_1^*\omega+\operatorname{pr}_2^*\omega$. The diagonal $\Delta$ is [Lagrangian](../../../../../../lagrangian.md). For a [symplectomorphism](../../../../../../symplectomorphism.md) $\phi$, its graph $\Gamma_\phi$ is also [Lagrangian](../../../../../../lagrangian.md), because its pullback of $\Omega$ is $-\omega+\phi^*\omega=0$.

If $\phi$ is sufficiently $C^1$-close to the identity, $\Gamma_\phi$ lies in the fixed Weinstein neighborhood of $\Delta$. Its image in $T^*\Delta$ is transverse to the cotangent fibers and is a section: the projection of that image to $\Delta\cong M$ is $C^1$-close to the identity, hence is a [diffeomorphism](../../../../../../diffeomorphism.md) on compact $M$. Reparametrizing by this projection identifies the image with $\operatorname{graph}(\sigma)$ for a small [differential one-form](../../../../../../one-form.md) $\sigma$.

The preceding [graph of a closed one-form is Lagrangian](../../../../../../graph-of-a-closed-one-form-is-lagrangian.md) criterion gives $d\sigma=0$. Since $H^1_{\mathrm{dR}}(M)=0$, the [de Rham cohomology](../../../../../../de-rham-cohomology.md) definition gives $\sigma=df$. Intersections with the zero section are precisely the [critical points](../../../../../../critical-point.md) of $f$; under the neighborhood identification these are the intersections $\Gamma_\phi\cap\Delta$, hence the [fixed points](../../../../../../fixed-point.md) of $\phi$.

On a nonempty compact manifold without boundary, $f$ has a maximum and a minimum. If it is nonconstant, these occur at distinct [critical points](../../../../../../critical-point.md). If it is constant, $df=0$ everywhere, so the whole graph is the diagonal and every point is fixed. **For positive-dimensional $M$, there are at least two distinct fixed points.** This is the [nearby exact Lagrangian intersection lemma](../../../../../../nearby-exact-lagrangian-intersection-lemma.md) applied to the diagonal. No connectedness assumption is needed.

The usual positive-dimensional convention is necessary for the assertion: if zero-dimensional [symplectic manifolds](../../../../../../symplectic-manifold.md) are allowed, a single-point $M$ has $H^1=0$ and only one [fixed point](../../../../../../fixed-point.md). That is a literal exception to the printed statement.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
