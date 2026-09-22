<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the deterministic [Hookean dumbbell model](../../../../hookean-dumbbell-model.md), with a [zero-rest-length spring](../../../../zero-rest-length-spring.md) and negligible connector drag. For $\mathbf R=\mathbf r_1-\mathbf r_2$, its elastic [forces](../../../../force-split.md) on the two beads are

$$
\mathbf F_1=-H\mathbf R,\qquad \mathbf F_2=+H\mathbf R.
$$

Here $H>0$ is the [spring constant](../../../../spring-constant.md). No independent thermal forcing from [Brownian motion](../../../../brownian-motion-split.md) or bead [inertia](../../../../inertia.md) is included. The unperturbed [linear velocity field](../../../../linear-velocity-field.md) is $\mathbf L\mathbf r$, with $\operatorname{tr}\mathbf L=0$ by [incompressibility](../../../../incompressible-flow.md).

The fluid [velocity](../../../../velocity.md) used in each bead's drag law is the imposed flow plus the disturbance from the _other_ bead, with its own singular field omitted. At leading order in $a/R$, the evenness of the [Oseen tensor](../../../../oseen-tensor.md), $\mathsf G(-\mathbf R)=\mathsf G(\mathbf R)$, gives

$$
\begin{aligned}
\dot{\mathbf r}_1
&=\mathbf L\mathbf r_1+\mathsf G(\mathbf R)\mathbf F_2
+\frac{\mathbf F_1}{\zeta},\\
\dot{\mathbf r}_2
&=\mathbf L\mathbf r_2+\mathsf G(\mathbf R)\mathbf F_1
+\frac{\mathbf F_2}{\zeta},
\qquad \boxed{\zeta=6\pi\mu a}.
\end{aligned}
$$

These are the pair [hydrodynamic mobility matrix](../../../../hydrodynamic-mobility-matrix.md) relations. Their signs follow from balancing each spring [force](../../../../force-split.md) with $-\zeta(\dot{\mathbf r}_i-\mathbf u_{{\rm ext},i})$, the fluid drag on that bead.

Adding the equations cancels both the direct spring slips and the cross-induced [velocities](../../../../velocity.md), since $\mathbf F_1+\mathbf F_2=0$. For the midpoint $\mathbf r_c=(\mathbf r_1+\mathbf r_2)/2$,

$$
\boxed{\dot{\mathbf r}_c=\mathbf L\mathbf r_c.}
$$

The midpoint therefore follows the undisturbed [linear velocity field](../../../../linear-velocity-field.md). Subtracting the equations instead gives the [hydrodynamic interaction of a Hookean dumbbell](../../../../hydrodynamic-interaction-of-a-hookean-dumbbell.md):

$$
\begin{aligned}
\dot{\mathbf R}
&=\mathbf L\mathbf R+
\left(\zeta^{-1}I-\mathsf G(\mathbf R)\right)
(\mathbf F_1-\mathbf F_2)\\
&=\boxed{\mathbf L\mathbf R-\frac{2H}{\zeta}
\left[I-\frac{\zeta}{8\pi\mu R}
(I+\widehat{\mathbf R}\widehat{\mathbf R}^T)\right]\mathbf R}.
\end{aligned}
$$

The dimensionless interaction matrix is

$$
\zeta\mathsf G(\mathbf R)
=\frac{3a}{4R}(I+\widehat{\mathbf R}\widehat{\mathbf R}^T).
$$

Its transverse and longitudinal [eigenvalues](../../../../eigenvalue.md) are $3a/(4R)$ and $3a/(2R)$, respectively. Since the spring [force](../../../../force-split.md) is longitudinal, the separation equation can also be written

$$
\boxed{\dot{\mathbf R}
=\mathbf L\mathbf R-\frac{2H}{\zeta}
\left(1-\frac{3a}{2R}\right)\mathbf R.}
$$

The relative correction to the free-draining spring relaxation rate is therefore $3a/(2R)$, explicitly proportional to $a/R$. Entrainment by the other bead reduces their relative approach for given opposing spring [forces](../../../../force-split.md).

This is a far-field [hydrodynamic interaction](../../../../hydrodynamic-interaction.md), valid for $R\gg a$; it is not a near-contact law and omits higher reflections and lubrication. The printed target also fixes the spring's rest length implicitly. For an ordinary [spring](../../../../spring.md) obeying [Hooke's law](../../../../hooke-s-law.md) with nonzero rest length $R_0$, the elastic [force](../../../../force-split.md) would be $-H(R-R_0)\widehat{\mathbf R}$, and every spring term above would acquire the factor $1-R_0/R$. The displayed result uses the [zero-rest-length spring](../../../../zero-rest-length-spring.md) convention appropriate to the ideal [Hookean dumbbell model](../../../../hookean-dumbbell-model.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the advanced fluid dynamics course of the University of Oxford](../../../split.md)
5. [Advanced fluid dynamics course of the University of Oxford](../../../../advanced-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
