<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Interactions produce [Feynman diagrams](../../../../feynman-diagram.md) with internal lines whose independent [loop momenta](../../../../loop-momentum.md) are integrated without an upper bound. Their large-momentum contributions can have an [ultraviolet divergence](../../../../ultraviolet-divergence.md). Two explicit examples in a scalar quartic theory are a one-loop [tadpole diagram](../../../../tadpole-diagram.md) contributing to the two-point function and a one-loop four-point [bubble diagram](../../../../bubble-diagram.md). After a [Wick rotation](../../../../wick-rotation.md), a spherical cutoff $\Lambda$ gives the representative integrals

$$
I_1=\int_{|k_E|<\Lambda}\frac{d^4k_E}{(2\pi)^4}\frac1{k_E^2+m^2}
=\frac1{16\pi^2}\left[\Lambda^2-m^2\ln\left(1+\frac{\Lambda^2}{m^2}\right)\right],
$$



$$
I_2(0)=\int_{|k_E|<\Lambda}\frac{d^4k_E}{(2\pi)^4}\frac1{(k_E^2+m^2)^2}
=\frac1{16\pi^2}\left[\ln\left(1+\frac{\Lambda^2}{m^2}\right)+\frac{m^2}{\Lambda^2+m^2}-1\right].
$$

Combinatorial factors and couplings multiply these integrals in a particular diagram. The first is quadratically divergent by cutoff [power counting](../../../../power-counting-in-quantum-field-theory.md); the second is logarithmically divergent. Other schemes package the divergent pieces differently.

In [renormalization](../../../../renormalization.md), introduce a [regularization](../../../../regularization.md), separate bare parameters into renormalized parameters and [counterterms](../../../../counterterm.md), and fix the latter by stated normalization conditions. Local divergent pieces of the scalar two- and four-point functions are absorbed into [mass](../../../../mass.md), field normalization and quartic-coupling counterterms, with all other operators allowed by the chosen symmetries included as needed. A perturbatively [renormalizable quantum field theory](../../../../renormalizable-quantum-field-theory.md) requires this finite counterterm family to remain closed at all orders. It does not require every individual bare diagram to be finite. For [gauge theories](../../../../gauge-theory.md), identities expressing gauge symmetry and absence of a [gauge anomaly](../../../../gauge-anomaly.md) are essential in addition to superficial counting.

The [action](../../../../action.md) is dimensionless in [natural units](../../../../natural-units.md), so in four spacetime dimensions $[\mathcal L]=4$ and $[\partial_\mu]=1$. The [engineering dimensions of relativistic fields](../../../../engineering-dimensions-of-relativistic-fields.md) follow from matching the free kinetic terms:

$$
2[\phi]+2=4,\qquad2[\psi]+1=4,\qquad2[A_\mu]+2=4,
$$

and hence

$$
\boxed{[\phi]=1,\qquad[\psi]=\frac32,\qquad[A_\mu]=1.}
$$

For a local operator $\mathcal O$ of [mass dimension](../../../../mass-dimension.md) $d_\mathcal O$, its coupling has dimension $4-d_\mathcal O$. Operators with dimension at most four are candidates for ordinary perturbative power-counting renormalizability. This test presupposes consistent kinetic terms, symmetries and the full set of induced counterterms; it is not a proof of physical consistency for an arbitrary vector interaction.

## ↑ Ancestors (13)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [2013](../../split.md)
4. [Past exam of the gauge field theory course of the University of Cambridge](../../../split.md)
5. [Gauge Field Theory course of the University of Cambridge](../../../../gauge-field-theory-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
