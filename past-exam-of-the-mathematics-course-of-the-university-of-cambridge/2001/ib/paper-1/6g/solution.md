<h1 id="6g/solution">Solution</h1>

↑ **Parent:** [6G](../6g.md)

Take $z$ positive downwards, and let the surface pressure be $p_0$. Static force balance gives the [hydrostatic pressure](../../../../../hydrostatic-pressure.md) equation $dp/dz=\rho g$. Hence

$$
\boxed{p(z)=p_0+\rho gz}.
$$

On a submerged body's surface, pressure traction is $-p\boldsymbol n$, where $\boldsymbol n$ points out of the body. The [divergence theorem](../../../../../divergence-theorem.md) gives the resultant

$$
\boldsymbol F=-\int_{\partial V}p\boldsymbol n\,dS
=-\int_V\nabla p\,dV=-\rho gV\boldsymbol e_z.
$$

Thus **the buoyancy is upward with magnitude $\rho gV$**, proving [Archimedes' principle](../../../../../archimedes-principle.md). The constant surface pressure makes no contribution because $\int_{\partial V}\boldsymbol n\,dS=0$.

For a floating iceberg of total volume $V$, the displaced seawater volume is $V-V_I$. Neglecting air buoyancy, equality of weight and buoyancy gives $\rho_IgV=\rho_wg(V-V_I)$. Consequently

$$
\boxed{V=\frac{\rho_w}{\rho_w-\rho_I}V_I},
$$

with $0<\rho_I<\rho_w$, as required for partial flotation.

## ↑ Ancestors (10)

1. [6G](../6g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
