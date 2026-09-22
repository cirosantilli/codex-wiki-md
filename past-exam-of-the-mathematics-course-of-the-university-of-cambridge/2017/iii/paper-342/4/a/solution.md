<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the two [Stokes flow](../../../../../../stokes-flow-split.md) solutions take the same incompressible [Newtonian fluid](../../../../../../newtonian-fluid.md), with constant viscosity $\mu$, no body forces, and

$$
\nabla\cdot u=\nabla\cdot\widehat u=0,\qquad
\nabla\cdot\sigma=\nabla\cdot\widehat\sigma=0,\qquad
\sigma=-pI+2\mu e,\quad\widehat\sigma=-\widehat pI+2\mu\widehat e.
$$

Here $e$ and $\widehat e$ are the symmetric [rate-of-strain tensors](../../../../../../strain-rate-tensor.md). The equality of viscosities is part of comparing two solutions in the same fluid; symmetry of an arbitrary constitutive stress alone would not suffice.

In components, with derivatives $\partial_j u_i$, use the [product rule](../../../../../../product-rule.md) to compute the divergence of the cross-work flux:

$$
\partial_j(\widehat u_i\sigma_{ij})
=(\partial_j\widehat u_i)\sigma_{ij}
=-p\,\partial_i\widehat u_i+2\mu e_{ij}\partial_j\widehat u_i
=2\mu e_{ij}\widehat e_{ij}.
$$

The pressure term vanishes by incompressibility; the antisymmetric part of the [velocity gradient](../../../../../../velocity-gradient.md) has zero contraction with the symmetric stress. Interchanging the hatted and unhatted fields gives exactly the same scalar. Thus

$$
\nabla\cdot(\sigma\cdot\widehat u-\widehat\sigma\cdot u)=0.
$$

Integrate over $V$ and apply the [divergence theorem](../../../../../../divergence-theorem.md). In its usual form the normal is outward from the fluid volume, whereas the printed $n$ points into the fluid. Reversing the normal multiplies both integrals by the same minus sign, leaving the [Lorentz reciprocal theorem for Stokes flow](../../../../../../lorentz-reciprocal-theorem-for-stokes-flow.md):

$$
\boxed{\int_S\widehat u\cdot\sigma\cdot n\,dS
=\int_Su\cdot\widehat\sigma\cdot n\,dS.}
$$

This proof applies to smooth fields or the corresponding finite-energy weak formulation. For an exterior domain one first truncates at a large sphere, applies the same identity, and takes the limit when the outer cross-work terms vanish, as for the decaying fields used below.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 342](../../../paper-342-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
