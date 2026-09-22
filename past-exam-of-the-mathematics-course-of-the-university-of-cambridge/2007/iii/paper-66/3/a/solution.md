<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a regular, spherical [star](../../../../../../star.md), [hydrostatic equilibrium](../../../../../../hydrostatic-equilibrium.md) gives $dP/dr=-Gm(r)\rho(r)/r^2$. Multiply by $4\pi r^3$ and integrate to the surface. [Integration by parts](../../../../../../integration-by-parts.md) gives

$$
\int_0^R4\pi r^3\frac{dP}{dr}dr=4\pi R^3P(R)-3\int_0^R4\pi r^2P\,dr.
$$

The central boundary term vanishes for finite central [pressure](../../../../../../pressure.md). Since $dm=4\pi r^2\rho\,dr$, the right-hand side of the integrated hydrostatic equation is

$$
-\int_0^R4\pi Gm\rho r\,dr=-\int_0^M\frac{Gm}{r(m)}dm=\Omega.
$$

The last expression is the [gravitational energy](../../../../../../gravitational-energy.md): adding a thin [mass](../../../../../../mass.md) shell $dm$ to the interior [mass](../../../../../../mass.md) $m$ contributes $-Gm\,dm/r$, counting each interacting pair once. Hence

$$
3\int_0^M\frac P\rho dm+\Omega=4\pi R^3P(R).
$$

With the specified zero surface [pressure](../../../../../../pressure.md) this proves the [stellar virial theorem](../../../../../../stellar-virial-theorem.md) in the required form,

$$
\boxed{3\int_0^M\frac P\rho dm+\Omega=0.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
