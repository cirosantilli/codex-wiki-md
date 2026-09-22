<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A moving or externally forced colloid disturbs the surrounding fluid, changing the [velocity](../../../../../velocity.md) of other colloids even without direct contact. These [hydrodynamic interactions](../../../../../hydrodynamic-interaction.md) are long-ranged at small [Reynolds number](../../../../../reynolds-number.md). In an unbounded incompressible Newtonian liquid, the [Stokes flow](../../../../../stokes-flow-split.md) response to a point [force](../../../../../force-split.md) is the [Stokeslet](../../../../../stokeslet.md):

$$
-\nabla p+\eta\nabla^2\mathbf u+\mathbf F\,\delta(\mathbf r)=0,\qquad\nabla\cdot\mathbf u=0,
\qquad u_i(\mathbf r)=\mathsf G_{ij}(\mathbf r)F_j.
$$

Its [Oseen tensor](../../../../../oseen-tensor.md) is

$$
\boxed{\mathsf G_{ij}(\mathbf r)=\frac1{8\pi\eta r}
\left(\delta_{ij}+\frac{r_ir_j}{r^2}\right).}
$$

This is a mobility tensor, with units [velocity](../../../../../velocity.md) per [force](../../../../../force-split.md), rather than a [stress](../../../../../stress.md) tensor. At separation $r$ the response parallel to the line of centres is $1/(4\pi\eta r)$; the perpendicular response is $1/(8\pi\eta r)$. Flow is not isotropic even though the solvent is. The disturbance decays as $1/r$, so treating all drag [forces](../../../../../force-split.md) as independent can miss correlated motion.

For well-separated equal spheres of [radius](../../../../../radius.md) $a$, the leading [hydrodynamic mobility matrix](../../../../../hydrodynamic-mobility-matrix.md) gives

$$
\mathbf V_i=\frac{\mathbf F_i}{6\pi\eta a}
+\sum_{j\ne i}\mathsf G(\mathbf r_i-\mathbf r_j)\mathbf F_j.
$$

The first term is the isolated-sphere self mobility; the remaining terms couple distinct particles. At thermal equilibrium the [fluctuation-dissipation theorem](../../../../../fluctuation-dissipation-theorem.md) also predicts correlated short-time increments, $\langle\Delta r_{i\alpha}\Delta r_{j\beta}\rangle\simeq2k_BT\mu_{i\alpha,j\beta}\Delta t$ with the configuration locally fixed. Thus correlated Brownian [displacements](../../../../../displacement.md) can reveal hydrodynamic coupling without an applied [force](../../../../../force-split.md).

The point-force approximation requires $r\gg a$ and negligible inertia. It diverges at the origin and cannot replace the finite self mobility. Near-contact lubrication, walls, many-body corrections, and a viscoelastic solvent require more complete mobility laws. A force-free particle can instead have a faster-decaying leading disturbance, so the $1/r$ claim specifically concerns a net-force-driven object.

<a id="2/c/image-oseen-mobility-directions"></a>
![](../../../../../past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2012/paper-1-oseen-response.png)

**[Figure 2](#2/c/image-oseen-mobility-directions). Oseen mobility directions**.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
5. [Past exam of the soft condensed matter course of the University of Cambridge](../../../../split.md)
6. [Soft Condensed Matter course of the University of Cambridge](../../../../../soft-condensed-matter-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
