<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Both profiles have integrable central cusps. Directly integrating the [surface density of a disk](../../../../../../surface-density-of-a-disk.md) and its [specific angular momentum](../../../../../../specific-angular-momentum.md) $j=\sqrt{GMr}$ gives

$$
M_d=2\pi\int_0^R\Sigma r\,dr=\pi\sigma R^2\frac{a}{2-a},
\qquad
J_d=2\pi\sqrt{GM}\int_0^R\Sigma r^{3/2}dr
=\frac{8\pi a}{5(5-2a)}\sqrt{GM}\,\sigma R^{5/2}.
$$

For $a=1$, substitution of the similarity functions gives

$$
\boxed{M_d=\frac{\pi C^2}{15A}t^{-1/5},\qquad
J_d=\frac{8\pi\sqrt{GM}C^{5/2}}{225A}=\mathrm{constant}}.
$$

The inward [accretion rate](../../../../../../accretion-rate.md) is $\dot M(r)=-2\pi r\Sigma\bar u_r$. At the origin it tends to $M_d/(5t)=-dM_d/dt$. The outward [viscous torque in an accretion disk](../../../../../../viscous-torque-in-an-accretion-disk.md) is

$$
\mathcal G=-2\pi r^2W=3\pi\bar\nu\Sigma j
=3\pi A\sqrt{GM}\,\sigma^2r^{5/2}(X-1)^2.
$$

For this profile $\mathcal G\to0$ as $r\to0$, and the advected angular-momentum flux $\dot Mj$ also vanishes there. Both outer fluxes vanish at $R$. Thus disk mass decreases through central accretion while disk angular momentum is conserved. Including the accreted central mass restores total mass conservation for the disk-plus-sink system.

For $a=5/4$, instead,

$$
\boxed{M_d=\frac{\pi C^2}{9A}=\mathrm{constant},\qquad
J_d=\frac{4\pi\sqrt{GM}C^{5/2}}{75A}t^{1/4}}.
$$

Here the mass flux tends to zero at the origin, despite positive radial velocity everywhere else. The inner torque has the nonzero limit

$$
\boxed{\mathcal G(0,t)=\frac{\pi\sqrt{GM}C^{5/2}}{75A}t^{-3/4}=\frac{dJ_d}{dt}}.
$$

Thus the [nonaccreting similarity disk supplied by an inner torque](../../../../../../nonaccreting-similarity-disk-supplied-by-an-inner-torque.md) conserves disk mass but gains angular momentum from an external central torque. Its vanishing edge flux cannot supply that gain. The disk is not globally isolated in angular momentum; the combined disk and torque source may of course conserve it.

These profiles illustrate different boundary-controlled similarity classes of the [Keplerian viscous diffusion equation](../../../../../../keplerian-viscous-diffusion-equation.md). The $a=1$ solution is compatible with a [zero-torque inner boundary condition](../../../../../../zero-torque-inner-boundary-condition.md) and conserved finite angular momentum, and can describe a late-time spreading accretion disk after the detailed initial profile has been forgotten. Its mass diverges as $t\downarrow0$, so the formal zero-radius origin is not a finite-mass initial disk. The $a=5/4$ solution has finite initial mass concentrated at the origin and initially zero disk angular momentum, but requires the specified inner torque for $t>0$; that torque's $t^{-3/4}$ singularity is time-integrable. It may describe a spreading nonaccreting disk for compatible torque-driven boundary conditions, but cannot be an isolated angular-momentum-conserving disk's generic asymptotic state. Similarity scaling suggests their possible asymptotic roles; it does not establish convergence for arbitrary initial and boundary data.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
