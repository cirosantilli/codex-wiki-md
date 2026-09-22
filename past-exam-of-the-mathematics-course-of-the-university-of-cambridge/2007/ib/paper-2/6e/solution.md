<h1 id="6e/solution">Solution</h1>

↑ **Parent:** [6E](../6e.md)

In a steady state, [Maxwell's equations](../../../../../maxwell-equations.md) imply $\nabla\times\mathbf E=0$, since the magnetic field is time independent. The divergence of the steady Ampère equation gives $\nabla\cdot\mathbf j=0$. With uniform [electrical conductivity](../../../../../electrical-conductivity.md), [Ohm's law](../../../../../ohm-s-law.md) is $\mathbf j=\sigma\mathbf E$, so

$$
\nabla\times\mathbf j=0,\qquad \nabla\cdot\mathbf j=0.
$$

For the usual straight-wire model, the cylindrical side is insulating and the two flat end faces are equipotentials. Put $\mathbf E=-\nabla V$. The [electric potential](../../../../../electric-potential.md) solves [Laplace's equation](../../../../../laplace-equation.md), with constant end values and zero normal derivative on the side. The linear axial potential $V(z)=V(0)-\Delta V\,z/l$ satisfies all these conditions. It is unique: the difference $h$ of two solutions has zero end values and zero side normal derivative, and [integration by parts](../../../../../integration-by-parts.md) gives $\int|\nabla h|^2\,dV=0$. Thus

$$
\boxed{\mathbf j=\frac{\sigma\Delta V}{l}\mathbf e_z
=\frac{I}{\pi a^2}\mathbf e_z.}
$$

This proves [uniform current in a straight homogeneous wire](../../../../../uniform-current-in-a-straight-homogeneous-wire.md) with the usual contact conditions. Integrating the [electric current density](../../../../../current-density.md) over a cross-section and using [Ohm's law](../../../../../ohm-s-law.md) then gives

$$
\boxed{R=\frac{l}{\sigma\pi a^2},\qquad
\dot Q=\int\mathbf j\cdot\mathbf E\,dV
=\frac{I^2l}{\sigma\pi a^2}=I^2R.}
$$

The second expression is the rate of [Ohmic heating](../../../../../joule-heating.md).

Strictly, steady current and uniform conductivity alone do not force uniformity; the contact conditions are implicit in the wire model. For example, let $\chi$ be a nonconstant transverse [Neumann eigenfunction](../../../../../neumann-eigenfunction.md) on the disk, satisfying $\Delta_\perp\chi=-\lambda^2\chi$ and zero normal derivative at its edge. Then $V=-E_0z+C\chi\cosh(\lambda(z-l/2))$ is harmonic and preserves an insulating cylindrical side, but its nonconstant end potentials produce nonuniform current. Its added axial current has zero cross-sectional mean. This supplies a counterexample if arbitrary contacts are permitted.

A bend generally redistributes the [electric current density](../../../../../current-density.md): the inner side of the bend carries more current than the outer side, as illustrated by $j_\theta\propto1/r$ in an annular conductor. Exact resistance and local [Ohmic heating](../../../../../joule-heating.md) can therefore change. For a slender, gently curved wire the straight-wire formulas remain the leading approximation; the identity $\dot Q=I^2R$ remains valid for the total steady dissipation.

## ↑ Ancestors (10)

1. [6E](../6e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
