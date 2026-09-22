<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

It is important to fix the [mass flux](../../../../../../mass-flux.md) convention. With literal mass units and the corresponding density-weighted [buoyancy flux](../../../../../../buoyancy-flux.md), the [Boussinesq approximation](../../../../../../boussinesq-approximation.md) and circular [top-hat plume model](../../../../../../top-hat-plume-model.md) give

$$
\boxed{Q=\rho_0\pi b^2V,\qquad
\mathbf M=\rho_0\pi b^2V^2(\cos\theta,\sin\theta),\qquad
F=g(\rho_0-\rho)\pi b^2V}.
$$

Replacing $\rho$ by $\rho_0$ in inertial fluxes is the [Boussinesq approximation](../../../../../../boussinesq-approximation.md); the density difference is retained in the [buoyancy flux](../../../../../../buoyancy-flux.md). Define the [kinematic plume fluxes](../../../../../../kinematic-plume-fluxes.md)

$$
q=Q/\rho_0,\qquad \mathbf m=\mathbf M/\rho_0,\qquad
f=F/\rho_0,\qquad m=|\mathbf m|=\pi b^2V^2.
$$

If the symbols $Q,\mathbf M,F$ instead denote the customary kinematic fluxes, simply omit the factors $\rho_0$ in all conversions below. Keeping the two conventions consistent is essential for the [jet length](../../../../../../jet-length.md) and dimensional prefactors.

The [Batchelor entrainment hypothesis](../../../../../../batchelor-entrainment-hypothesis.md) prescribes inward edge [velocity](../../../../../../velocity.md)

$$
\boxed{u_e=\alpha V}.
$$

The constant [entrainment coefficient](../../../../../../entrainment-coefficient.md) relates ambient inflow to the local axial [velocity](../../../../../../velocity.md). A centreline segment of [arc length](../../../../../../arc-length.md) $ds$ entrains volume $2\pi b\,u_e\,ds$. Hence, setting $E=2\alpha\sqrt\pi$,

$$
\boxed{\frac{dq}{ds}=2\pi\alpha bV=E\sqrt m,\qquad
\frac{df}{ds}=0},\qquad
\frac{dQ}{ds}=2\alpha\sqrt{\pi\rho_0|\mathbf M|},\qquad \frac{dF}{ds}=0.
$$

The [buoyancy flux](../../../../../../buoyancy-flux.md) is conserved because the homogeneous entrained ambient has zero density deficit, and mixing has no buoyancy source or sink. The imposed zero source [mass flux](../../../../../../mass-flux.md) with nonzero source [momentum flux](../../../../../../momentum-flux.md) is a singular point-source idealization, not a finite-radius nozzle with zero emitted fluid. Indeed $V=m/q$ and the plume [reduced gravity](../../../../../../reduced-gravity-split.md) $f/q$ diverge as $q\to0$ with nonzero source fluxes. The [Boussinesq approximation](../../../../../../boussinesq-approximation.md) cannot remain valid arbitrarily close to that point. The [top-hat plume model](../../../../../../top-hat-plume-model.md) is applied outside the unresolved source region.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 345](../../../paper-345-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
