<h1 id="10d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assemble the star by adding spherical shells. A shell of mass $dm$ at radius $r$ has [gravitational potential energy](../../../../../../gravitational-energy.md) $-Gm(r)\,dm/r$ relative to infinity, giving

$$
\boxed{E_{\mathrm{grav}}=-\int_0^R\frac{Gm(r)}r\,dm=-4\pi G\int_0^R m(r)\rho(r)r\,dr.}
$$

Multiplication of the [hydrostatic equilibrium](../../../../../../hydrostatic-equilibrium.md) equation by $4\pi r^3$ and [integration by parts](../../../../../../integration-by-parts.md) gives

$$
E_{\mathrm{grav}}=\int_0^R4\pi r^3P'(r)dr=4\pi R^3P(R)-3\int_V P\,dV.
$$

For an isolated star with negligible surface pressure, $P(R)=0$. Using $E_{\mathrm{kin}}=(3/2)\int_V P\,dV$, the [virial theorem](../../../../../../virial-theorem.md) becomes $\boxed{2E_{\mathrm{kin}}+E_{\mathrm{grav}}=0}$. If a nonzero external pressure is present, the surface term must be retained: $2E_{\mathrm{kin}}+E_{\mathrm{grav}}=3P(R)V$. Thus the printed zero-surface-term identity implicitly assumes an isolated star.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [10D](../../10d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
