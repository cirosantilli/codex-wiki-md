<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the common-density, equal-volume-heat-capacity model implicit in the stated speed law. Let the [liquid fraction](../../../../../../liquid-fraction.md) be $\phi$ ahead of the melting front and $\phi+\Delta\phi$ behind it. Melting adds exactly the liquid needed to fill the newly created pores, so total [mass conservation](../../../../../../mass-conservation.md) makes [Darcy flux](../../../../../../darcy-velocity.md) continuous. Consequently,

$$
\boxed{u_{\rm ahead}=U,\qquad v_{\rm ahead}=U/\phi,\qquad v_{\rm behind}=U/(\phi+\Delta\phi).}
$$

Here $u$ denotes [Darcy velocity](../../../../../../darcy-velocity.md) and $v$ the pore-liquid velocity in the stationary rock frame. Treating the pore-space increase as storage without its simultaneous melting source would incorrectly change the Darcy flux.

Relative to the cold unmelted material, the bulk [enthalpy](../../../../../../enthalpy.md) increase behind the front is $\rho c_p\Delta T+\rho L\Delta\phi$: all phases gain sensible heat and the melted ice consumes [latent heat](../../../../../../latent-heat.md). The advective heat-flux difference is $\rho c_pU\Delta T$. Applying the [Rankine-Hugoniot condition](../../../../../../rankine-hugoniot-conditions.md) to this energy balance therefore gives

$$
V(\rho c_p\Delta T+\rho L\Delta\phi)=\rho c_pU\Delta T,
$$

so the [advection-driven melting front in a porous matrix](../../../../../../advection-driven-melting-front-in-a-porous-matrix.md) moves at

$$
\boxed{V=\frac{U}{1+S\Delta\phi},\qquad S=\frac{L}{c_p\Delta T}.}
$$

The advected latent contribution of the liquid is the same on both sides and cancels; the denominator measures sensible heating plus phase-change energy per unit bulk volume.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 332](../../../paper-332-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
