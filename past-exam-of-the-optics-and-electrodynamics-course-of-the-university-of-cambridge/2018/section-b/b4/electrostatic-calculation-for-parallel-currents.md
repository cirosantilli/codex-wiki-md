<h1 id="section-b/b4/electrostatic-calculation-for-parallel-currents">Electrostatic calculation for parallel currents</h1>

↑ **Parent:** [Solution](solution.md)

Put wire 1 on the $z$ axis and wire 2 at $x=d$, with positive $x$ pointing away from wire 1. Let each wire have stationary positive [linear charge density](../../../../linear-charge-density.md) $+\lambda$ and moving [electron](../../../../electron.md) line density $-\lambda$ in the lab. For equal currents, both [electron](../../../../electron.md) populations have drift [velocity](../../../../velocity.md) $+v\widehat{\mathbf z}$, so the signed conventional current is $I=-\lambda v$.

First consider wire 2's positive charges in their own rest frame, which is the lab. Wire 1 has zero total line charge there, so its external electrostatic field is zero. The positive-charge [force](../../../../force-split.md) per length is therefore $\boxed{f_+=0}$.

Next use the [electron](../../../../electron.md) rest frame $S'$ moving at $+v\widehat{\mathbf z}$. Wire 1's ion line density becomes $\lambda_+'=\gamma\lambda$. Its [electron](../../../../electron.md) density becomes $\lambda_-'=-\lambda/\gamma$: the [electron](../../../../electron.md) rest density is lower than its lab density. The transformed total is

$$
\lambda_1'=\gamma\lambda-\frac\lambda\gamma
=\gamma\lambda\frac{v^2}{c^2}.
$$

Equivalently this follows from the [four-current](../../../../four-current.md) transformation $\lambda_1'=\gamma(\lambda_{1,\rm net}-vI_1/c^2)$, with $\lambda_{1,\rm net}=0$ and $I_1=-\lambda v$. By the electrostatic field of a [line charge](../../../../line-charge.md),

$$
\mathbf E_1'=\frac{\lambda_1'}{2\pi\epsilon_0d}\widehat{\mathbf x}.
$$

A wire-2 [electron](../../../../electron.md) is at rest in $S'$ and feels only the electric [force](../../../../force-split.md), $F'_{e,x}=-e\lambda_1'/(2\pi\epsilon_0d)$, toward wire 1.

Apply the supplied transverse [relativistic force transformation](../../../../relativistic-force-transformation.md) with the [electron](../../../../electron.md)'s lab [velocity](../../../../velocity.md) $\mathbf u=\mathbf v$. Its denominator is $\gamma(1-v^2/c^2)=1/\gamma$, so $F'_{e,x}=\gamma F_{e,x}$, or $F_{e,x}=F'_{e,x}/\gamma$. There are $\lambda/e$ [electrons](../../../../electron.md) per unit lab length. Thus

$$
\boxed{f_-\equiv\frac{F_{-,x}}\ell
=\frac\lambda e\frac{-e\lambda_1'}{2\pi\epsilon_0d\gamma}
=-\frac{\lambda^2v^2}{2\pi\epsilon_0c^2d}
=-\frac{\mu_0I^2}{2\pi d}.}
$$

Adding $f_+=0$ gives exactly the attractive magnetic result. This [electrostatic-frame derivation of parallel-wire forces](../../../../electrostatic-frame-derivation-of-parallel-wire-forces.md) uses electrostatics in each test carrier's own rest frame; no magnetic [force](../../../../force-split.md) acts on that stationary test carrier there. The other wire can still carry current in that frame. Transform the [force](../../../../force-split.md) per [electron](../../../../electron.md) first and then count [electrons](../../../../electron.md) per lab length: transforming a [force](../../../../force-split.md) per unit length as if it were a particle [force](../../../../force-split.md) would introduce an incorrect extra contraction factor.

## ↑ Ancestors (14)

1. [Solution](solution.md)
2. [B4](../b4.md)
3. [Section B](../../section-b.md)
4. [2018](../../../2018-split.md)
5. [Past exam of the optics and electrodynamics course of the University of Cambridge](../../../split.md)
6. [Optics and Electrodynamics course of the University of Cambridge](../../../../optics-and-electrodynamics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../list-of-universities.md)
14. [Codex Wiki](../../../../split.md)
