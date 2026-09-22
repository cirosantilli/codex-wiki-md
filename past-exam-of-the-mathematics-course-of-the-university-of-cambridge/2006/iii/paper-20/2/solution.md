<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [symplectic neighborhood theorem](../../../../../symplectic-neighborhood-theorem.md) says that a [symplectomorphism](../../../../../symplectomorphism.md) between compact [symplectic submanifolds](../../../../../symplectic-submanifold.md), together with a [symplectic vector bundle](../../../../../symplectic-vector-bundle.md) isomorphism of their [symplectic normal bundles](../../../../../symplectic-normal-bundle.md), extends to a [symplectomorphism](../../../../../symplectomorphism.md) of neighborhoods. To outline the proof, use [tubular neighborhoods](../../../../../tubular-neighborhood.md) to extend the bundle identification smoothly. The two pulled-back [symplectic forms](../../../../../symplectic-form.md) agree as bilinear forms along the zero section. The [relative Poincaré lemma](../../../../../relative-poincare-lemma.md) writes their difference as $d\alpha$, with $\alpha$ vanishing there. Their linear interpolation $\omega_t$ remains [nondegenerate](../../../../../nondegenerate-bilinear-form.md) on a sufficiently small neighborhood. Solving

$$
\iota_{V_t}\omega_t=-\alpha
$$

and integrating $V_t$ gives the [relative Moser theorem](../../../../../relative-moser-theorem.md); the flow fixes the submanifold and carries one form to the other.

For the [symplectic fiber sum along a square-zero surface](../../../../../symplectic-fiber-sum-along-a-square-zero-surface.md), the [self-intersection](../../../../../self-intersection-number.md) is the [Euler number](../../../../../euler-number-of-a-vector-bundle.md) of the oriented rank-two [normal bundle](../../../../../normal-bundle.md). Thus each normal bundle is trivial. Rescale one ambient [symplectic form](../../../../../symplectic-form.md) if necessary to equalize the areas of the two copies of $C$. The [Moser theorem](../../../../../moser-s-trick.md) for the surface then supplies a base identification preserving their area forms. The [symplectic neighborhood theorem](../../../../../symplectic-neighborhood-theorem.md) identifies each neighborhood with a product carrying

$$
\omega_C+\frac12d(r^2)\wedge d\theta.
$$

Remove small disk neighborhoods and glue collars with the base identification and

$$
\theta_Y=-\theta_X,\qquad
r_Y^2=a-r_X^2
$$

for a suitable positive constant $a$. Both signs reverse, so the normal two-forms match; the base forms already match. They define a closed [nondegenerate](../../../../../nondegenerate-bilinear-form.md) two-form across the neck, agreeing with the ambient forms elsewhere. This constructs the [symplectic sum](../../../../../symplectic-sum.md). Its construction uses the area normalization and the chosen normal-bundle gluing.

For a smooth counterexample, take $X=Y=\mathbb{CP}^2$, and in a small four-ball in each choose an unknotted [sphere](../../../../../sphere.md) bounding a three-ball. These spheres are [null-homologous](../../../../../null-homologous-cycle.md) and have [self-intersection](../../../../../self-intersection-number.md) zero. Their standard smooth fiber sum is

$$
Z\cong\mathbb{CP}^2\mathbin{\#}\mathbb{CP}^2
\mathbin{\#}(S^1\times S^3).
$$

Indeed, the complement of the standard $S^2\times D^2$ in $S^4$ is $S^1\times D^3$; doubling these complements gives $S^1\times S^3$, and the two ambient projective-plane summands remain as [connected sums](../../../../../connected-sum-of-oriented-manifolds.md). This is the [smooth fiber sum along unknotted null-homologous spheres](../../../../../smooth-fiber-sum-along-unknotted-null-homologous-spheres.md).

In the induced [orientation](../../../../../orientation-of-a-simplex.md), both summands in $Z=\mathbb{CP}^2\#(\mathbb{CP}^2\#(S^1\times S^3))$ have positive [positive index of the intersection form](../../../../../positive-index-of-the-intersection-form.md). The [symplectic connected-sum obstruction](../../../../../symplectic-connected-sum-obstruction.md) therefore rules out a [symplectic form](../../../../../symplectic-form.md): connected-sum vanishing of the [Seiberg–Witten invariant of a four-manifold](../../../../../seiberg-witten-invariant-of-a-four-manifold.md) contradicts [Taubes nonvanishing theorem](../../../../../taubes-nonvanishing-theorem.md). In the opposite orientation the [intersection form](../../../../../intersection-form.md) is negative definite, also ruling out a [symplectic form](../../../../../symplectic-form.md), whose class has positive square. Thus **the smooth fiber sum need not be symplectic**.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 20](../../paper-20-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
