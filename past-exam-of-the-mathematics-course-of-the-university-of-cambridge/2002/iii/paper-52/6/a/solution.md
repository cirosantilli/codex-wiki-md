<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Boussinesq approximation](../../../../../../boussinesq-approximation.md) and a [top-hat plume model](../../../../../../top-hat-plume-model.md). Let $v(z)<0$ be the uniform ambient return [velocity](../../../../../../velocity.md) outside the plume. Negligible source [volume flux](../../../../../../volumetric-flow-rate.md) and an impermeable cylindrical wall require zero net transport through every horizontal section:

$$
\boxed{b^2w+(R^2-b^2)v=0,\qquad v=-\frac{b^2w}{R^2-b^2}.}
$$

The entrainment speed must be specified relative to that moving ambient. Taking it to be $\alpha(w-v)$ gives

$$
\boxed{\frac{d}{dz}(b^2w)=2\alpha b(w-v).}
$$

The surrounding unmodified fluid has zero [buoyancy](../../../../../../buoyancy.md) relative to the initial fluid. Neglecting thermal or compositional loss therefore gives

$$
\boxed{\frac{d}{dz}(b^2wg')=0.}
$$

Let $B_s$ denote the conserved specific source [buoyancy flux](../../../../../../buoyancy-flux.md): $B_s=B_o/\pi$ if $B_o$ is the actual integrated source flux, or $B_s=B_o$ if the source strength has already been normalized by $\pi$.

To obtain the usual integral-model singularity one must also state a [pressure](../../../../../../pressure.md) closure. Here take the whole-section mean [pressure](../../../../../../pressure.md) to have only its reference ambient [hydrostatic pressure](../../../../../../hydrostatic-pressure.md), and neglect wall force and extra vertical turbulent-stress fluxes in the integral budget. Internal [momentum](../../../../../../momentum.md) transfers between plume and ambient cancel in that whole-section balance. The remaining upward force is the plume [buoyancy](../../../../../../buoyancy.md), giving

$$
\boxed{\frac{d}{dz}\left[b^2w^2+(R^2-b^2)v^2\right]=b^2g'.}
$$

The two [momentum fluxes](../../../../../../momentum-flux.md) add, even though $v$ is negative: vertical [momentum](../../../../../../momentum.md) transported downward also contributes $v^2$ to the flux through an upward-oriented horizontal section. These three flux balances, with the algebraic return-velocity constraint, govern $b,w,g'$ in the [confined plume with compensating return flow](../../../../../../confined-plume-with-compensating-return-flow.md).

The pressure-neglecting closure is an integral approximation, not a claim that the return fluid has zero acceleration. If a mean [pressure](../../../../../../pressure.md) departure $p_*(z)$ is retained, the whole-section [momentum](../../../../../../momentum.md) balance instead contains $-(R^2/\rho_0)p_*'(z)$, along with any wall-force or stress contribution. The entrainment hypothesis alone does not specify that function. The singularity calculated below belongs to the stated pressure-neglecting model; it is not forced by continuity alone or asserted to be an infinite [velocity](../../../../../../velocity.md) in the real fluid.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [6](../../6.md)
3. [Section C](../../section-c.md)
4. [Paper 52](../../../paper-52-split.md)
5. [Iii](../../../split.md)
6. [2002](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
