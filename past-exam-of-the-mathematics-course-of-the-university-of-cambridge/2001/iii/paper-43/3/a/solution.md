<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a rising light plume use $g'=g(\rho-\rho_p)/\rho_0>0$ in the [Boussinesq approximation](../../../../../../boussinesq-approximation.md), with ambient density as the inertial reference. The full cross-sectional kinematic [volume flux](../../../../../../volumetric-flow-rate.md), [momentum flux](../../../../../../momentum-flux.md) and [buoyancy flux](../../../../../../buoyancy-flux.md) of a [top-hat plume](../../../../../../top-hat-plume-model.md) are

$$
\boxed{Q=\pi b^2w,\quad M=\pi b^2w^2,\quad B=\pi b^2wg'=Qg'.}
$$

Here momentum flux per unit reference density is meant, not momentum per unit volume. The [Batchelor entrainment hypothesis](../../../../../../batchelor-entrainment-hypothesis.md) says ambient fluid crosses the plume edge at mean inward speed $\alpha w$, where $\alpha$ is the dimensionless [entrainment coefficient](../../../../../../entrainment-coefficient.md). Volume added per unit height is $2\pi b\alpha w$. With $a_e=2\alpha\sqrt\pi$, the integrated plume balances in uniform ambient density are

$$
Q'=a_e\sqrt M,\qquad M'=BQ/M,\qquad B'=0.
$$

Seek a [pure plume](../../../../../../pure-plume.md) with no persistent source volume or momentum scale. Equating powers of $z$ gives $Q\propto z^{5/3}$ and $M\propto z^{4/3}$; constant buoyancy gives $B=B_0$. Equating coefficients yields, relative to the ideal source or a fitted [plume virtual origin](../../../../../../plume-virtual-origin.md),

$$
\boxed{M=\left(\frac{9a_eB_0}{20}\right)^{2/3}z^{4/3},\quad
Q=\frac{3a_e}{5}\left(\frac{9a_eB_0}{20}\right)^{1/3}z^{5/3},\quad B=B_0.}
$$

Thus $Q\sim B_0^{1/3}z^{5/3}$, $M\sim B_0^{2/3}z^{4/3}$ and $b=6\alpha z/5$. A finite nozzle or nonzero source momentum requires a near-source transition rather than this singular point-source solution at arbitrarily small $z$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
