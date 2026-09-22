<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [strong equivalence principle](../../../../../strong-equivalence-principle.md) extends universality of free fall to bodies with appreciable gravitational binding energy and requires results of sufficiently local experiments, including gravitational experiments, in freely falling laboratories to be independent of their location and velocity. The [Einstein equivalence principle](../../../../../einstein-equivalence-principle.md) makes the corresponding statement for nongravitational experiments; the weak principle concerns test-body free fall without significant self-gravity. In a locally inertial frame the nongravitational laws take their special-relativistic form, while internal gravitational experiments retain the same local gravitational laws and coupling constants. They are not declared to have no gravity.

In a metric description, one may set $g_{ab}=\eta_{ab}$ and $\partial_cg_{ab}=0$ at a point by [Riemann normal coordinates](../../../../../normal-coordinates.md), so the [Levi-Civita connection](../../../../../levi-civita-connection.md) vanishes there. This removes a locally uniform external gravitational acceleration, not the [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md). Tidal effects between separated bodies, or accumulated over a finite-duration experiment, remain. The local limit must control both the laboratory's size and duration. Gravitationally self-bound bodies are included in the strong version, so it is stronger than equality of inertial and passive gravitational mass for ordinary test particles.

A heuristic field-equation argument supplements this principle with further assumptions: gravity is described only by a Lorentzian metric, matter couples universally to it, the [affine connection](../../../../../affine-connection.md) is Levi-Civita, and the leading local field equation is a symmetric covariant equation with at most second metric derivatives and is linear in those second derivatives. Matter obeys [stress-energy conservation](../../../../../stress-energy-conservation.md) $\nabla^aT_{ab}=0$. [Curvature](../../../../../curvature.md) therefore supplies the natural candidates $R_{ab}$ and $Rg_{ab}$, with a constant multiple of $g_{ab}$ also allowed. Write the candidate as $R_{ab}+cRg_{ab}+\Lambda g_{ab}=\kappa T_{ab}$. The [contracted Bianchi identity](../../../../../contracted-bianchi-identity.md) and [metric compatibility](../../../../../metric-compatibility.md) give

$$
\nabla^aR_{ab}=\frac12\nabla_bR,\qquad
\nabla^a(R_{ab}+cRg_{ab})=(\tfrac12+c)\nabla_bR.
$$

To permit varying [scalar curvature](../../../../../scalar-curvature.md) consistently with matter conservation, take $c=-1/2$. This gives the [Einstein tensor](../../../../../einstein-tensor.md) $G_{ab}=R_{ab}-g_{ab}R/2$ and

$$
G_{ab}+\Lambda g_{ab}=\kappa T_{ab}.
$$

The [cosmological constant](../../../../../cosmological-constant.md) is constant so that its divergence vanishes. These assumptions motivate the usual Einstein equation; the equivalence principle alone does not exclude theories with extra fields or higher [curvature](../../../../../curvature.md) terms.

The sign and normalization are fixed by the supplied Newtonian limit. Use signature $(+---)$, the [curvature](../../../../../curvature.md) [commutator](../../../../../commutator.md) convention of Q1, and the Ricci contraction

$$
R_{ab}=R_{acb}{}^c.
$$

This is the contraction for which $R_{00}\simeq-\nabla^2\varphi$ in the question. In four dimensions, tracing the candidate equation gives $-R+4\Lambda=\kappa T$, and substituting back gives

$$
R_{ab}=\kappa\left(T_{ab}-\frac12g_{ab}T\right)+\Lambda g_{ab}.
$$

For slowly moving pressureless matter, $T_{00}\simeq\rho$, $T\simeq\rho$ and $g_{00}\simeq1$. On local scales where the cosmological term is negligible, $R_{00}\simeq\kappa\rho/2$. Compare this with $R_{00}\simeq-\nabla^2\varphi$ and the [Poisson equation](../../../../../poisson-equation.md) $\nabla^2\varphi=4\pi G\rho$. The [Newtonian normalization of the Einstein field equations](../../../../../newtonian-normalization-of-the-einstein-field-equations.md) is therefore

$$
\boxed{\kappa=-8\pi G,\qquad G_{ab}+\Lambda g_{ab}=-8\pi G T_{ab}.}
$$

Units with light speed one are used, as in the paper; for conventional physical stress-energy units the coupling is $-8\pi G/c^4$. If the opposite Ricci/[curvature](../../../../../curvature.md) sign convention is adopted, the displayed geometric coupling sign changes accordingly. With the cosmological term retained in the same weak-field calculation, the Newtonian equation becomes $\nabla^2\varphi=4\pi G\rho-\Lambda$, consistent with this sign choice.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 55](../../paper-55-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
