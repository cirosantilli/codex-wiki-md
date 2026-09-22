# Sampling uncertainty of an endpoint diffusivity estimate

↑ **Parent:** [Brownian radius estimate from endpoint displacements](brownian-radius-estimate-from-endpoint-displacements.md)

Each Cartesian Brownian increment has [variance](variance-split.md) $2Dt$. Summing their normalized squares gives a [chi-squared distribution](chi-squared-distribution.md) with $3n$ [degrees of freedom](degree-of-freedom.md). Hence $\widehat D$ is unbiased and has relative [standard deviation](standard-deviation.md) $\sqrt{2/(3n)}$. Its inverse is not unbiased: for $3n>2$, $\mathbb E[1/\widehat D]=[3n/(3n-2)]/D$. Thus the direct inverse-diffusivity [radius](radius.md) estimate has appreciable finite-sample bias when only a few trajectories are observed. Measurement noise or drift adds separate systematic error.

## ↑ Ancestors (10)

1. [Brownian radius estimate from endpoint displacements](brownian-radius-estimate-from-endpoint-displacements.md)
2. [Stokes–Einstein relation](stokes-einstein-relation.md)
3. [Stokes's law](stokes-s-law.md)
4. [Surface traction in translating-sphere Stokes flow](surface-traction-in-translating-sphere-stokes-flow.md)
5. [Stokes flow](stokes-flow-split.md)
6. [Viscous fluid flow](viscous-fluid-flow-split.md)
7. [Fluid mechanics](fluid-mechanics-split.md)
8. [Branches of physics](branches-of-physics.md)
9. [Physics](physics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2012/paper-1/1/a/solution.md)
