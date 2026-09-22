<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let downward [velocity](../../../../../../velocity.md) be positive in this part, and let $W>0$ be the dense [sphere](../../../../../../sphere.md)'s weight minus [buoyancy](../../../../../../buoyancy.md). For the original centreline configuration, write its six-component translation-and-rotation [velocity](../../../../../../velocity.md) as $q$, and its diagonal positive [hydrodynamic resistance matrix](../../../../../../hydrodynamic-resistance-matrix.md) as $R_0$. Its single-sphere dissipation is

$$
D_0(q)=q^TR_0q=R_{zz}V_z^2+\sum_{\beta\ne z}R_{\beta\beta}q_\beta^2.
$$

With only axial [force](../../../../../../force.md) and no [torque](../../../../../../torque.md), the original [velocity](../../../../../../velocity.md) is $V_0=W/R_{zz}$.

Now add the neutral [sphere](../../../../../../sphere.md). In its actual [Stokes flow](../../../../../../stokes-flow-split.md), extend the [velocity](../../../../../../velocity.md) rigidly through the new [sphere](../../../../../../sphere.md)'s interior. This extension is a valid incompressible trial field for the domain without that [sphere](../../../../../../sphere.md), with exactly the dense [sphere](../../../../../../sphere.md)'s actual six boundary [velocities](../../../../../../velocity.md); its strain and dissipation inside the inserted ball are zero. The [Minimum-dissipation theorem for Stokes flow](../../../../../../minimum-dissipation-theorem-for-stokes-flow.md) and [extra dissipation due to a rigid inclusion](../../../../../../extra-dissipation-due-to-a-rigid-inclusion.md) therefore give

$$
D\geq D_0(q)\geq R_{zz}V_z^2.
$$

The neutral [sphere](../../../../../../sphere.md) has zero net external [force](../../../../../../force.md) and [torque](../../../../../../torque.md), and the dense [sphere](../../../../../../sphere.md) has only the axial [force](../../../../../../force.md) $W$. The dissipation equals total external power, so $D=WV_z$. Positivity gives $V_z>0$, and the comparison yields $V_z\leq W/R_{zz}$ without assuming that either [sphere](../../../../../../sphere.md) translates only vertically or that either angular [velocity](../../../../../../velocity.md) vanishes.

For a finite nonoverlapping placement, the first inequality is strict. Equality would make the extended field the old Stokes solution and thus make that solution rigid throughout the added ball. Analyticity and connectedness then [force](../../../../../../force.md) its strain to vanish throughout the original fluid domain; the stationary tube wall and quiescent far field would [force](../../../../../../force.md) the whole motion to vanish, contradicting $V_z>0$. Hence the [force-free inclusion reduces axial mobility of a centred settling sphere](../../../../../../force-free-inclusion-reduces-axial-mobility-of-a-centred-settling-sphere.md):

$$
\boxed{0<V_z<V_0.}
$$

The difference tends to zero as the added [sphere](../../../../../../sphere.md) recedes infinitely far away. The lateral and rotational contributions are nonnegative in the resistance comparison, which is precisely why they cannot invalidate the bound.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
