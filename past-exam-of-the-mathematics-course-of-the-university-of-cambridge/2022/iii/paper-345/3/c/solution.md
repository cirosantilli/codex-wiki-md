<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose $\rho_0$ as a representative room density, for example the fresh-air density, and neglect relative density variations everywhere except in [buoyancy](../../../../../../buoyancy.md). With

$$
g'=\frac{\widehat\rho-\rho}{\rho_0}g,
$$

the triangular profiles give

$$
Q=\frac12\rho_0bW,
\qquad
M=\frac13\rho_0bW^2,
\qquad
F=\frac13\rho_0bWg'.
$$

Solving these algebraic relations,

$$
\boxed{W=\frac{3M}{2Q},
\qquad b=\frac{4Q^2}{3\rho_0M},
\qquad g'=\frac{3F}{2Q}.}
$$

The [Batchelor entrainment hypothesis](../../../../../../batchelor-entrainment-hypothesis.md), vertical [momentum conservation](../../../../../../momentum-conservation.md), and [mass conservation](../../../../../../mass-conservation.md) give

$$
\boxed{\frac{dV}{dz}=\alpha W,}
\qquad
\boxed{\frac{dQ}{dz}=\rho_0\alpha W=\frac{3\rho_0\alpha M}{2Q},}
\qquad
\boxed{\frac{dM}{dz}=\frac12\rho_0bg'=\frac{QF}{M}.}
$$

An ascending parcel entrains ambient fluid from progressively lower ambient density. With the [buoyancy frequency](../../../../../../buoyancy-frequency.md)

$$
N^2=-\frac g{\rho_0}\frac{d\widehat\rho}{dz},
$$

the change of ambient reference density subtracts $QN^2$ from its density-weighted [buoyancy flux](../../../../../../buoyancy-flux.md), so

$$
\boxed{\frac{dF}{dz}=-QN^2.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 345](../../../paper-345-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
