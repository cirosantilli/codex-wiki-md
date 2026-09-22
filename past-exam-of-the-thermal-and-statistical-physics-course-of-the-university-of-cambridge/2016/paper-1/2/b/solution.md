<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**[Brownian motion](../../../../../brownian-motion-split.md) is the irregular motion of a mesoscopic particle caused by thermal molecular impacts.** A colloidal sphere in a fluid provides a physical example. The random force competes with dissipative drag; averaging many trajectories produces [diffusion](../../../../../diffusion.md) even though each trajectory fluctuates.

A free-particle [Langevin equation](../../../../../langevin-dynamics.md) with [thermal Langevin force normalization](../../../../../thermal-langevin-force-normalization.md) is

$$
m\dot{\mathbf v}=-\zeta\mathbf v+\boldsymbol\xi(t),\qquad\langle\xi_i(t)\xi_j(t')\rangle=2\zeta k_BT\,\delta_{ij}\delta(t-t').
$$

The noise has zero mean, and its strength is linked to drag by the [fluctuation-dissipation theorem](../../../../../fluctuation-dissipation-theorem.md). The velocity relaxes on the time scale $\tau=m/\zeta$. At long times $t\gg\tau$, the [Einstein diffusion relation](../../../../../einstein-diffusion-relation.md) is

$$
\boxed{D=\frac{k_BT}{\zeta},\qquad\langle|\mathbf r(t)-\mathbf r(0)|^2\rangle=6Dt\quad\hbox{in three dimensions}.}
$$

For a slowly moving no-slip sphere of radius $a$ in a continuum fluid of [dynamic viscosity](../../../../../dynamic-viscosity-split.md) $\eta$, [Stokes drag law](../../../../../stokes-s-law.md) gives $\zeta=6\pi\eta a$. The particle probability [density](../../../../../density.md) obeys $\partial_tP=D\nabla^2P$; a localized initial position develops a Gaussian profile. The [ballistic-to-diffusive Brownian displacement](../../../../../ballistic-to-diffusive-brownian-displacement.md) changes character: at $t\ll\tau$, equilibrium velocities instead give ballistic mean-square displacement $3(k_BT/m)t^2$.

<a id="2/b/image-an-illustrative-random-trajectory-and-the-inertial-crossover-from-ballistic-to-diffusive-mean-square-displacement"></a>
![](../../../../../past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2016/paper-1-brownian-motion.png)

**[Figure 4](#2/b/image-an-illustrative-random-trajectory-and-the-inertial-crossover-from-ballistic-to-diffusive-mean-square-displacement). An illustrative random trajectory and the inertial crossover from ballistic to diffusive mean-square displacement**. [Source](paper-1-brownian-motion.py).

The drag-noise model assumes a classical bath with a sufficiently short correlation time; a mathematical white-noise trajectory does not resolve individual molecular collisions. Tracking nonliving colloidal particles measures [diffusion](../../../../../diffusion.md) and tests the connection between thermal fluctuations and dissipation.[Sections 3.1–3.2: Brownian motion, Langevin equation, diffusion and the Einstein relation](../../../../../stochastic-processes-by-david-tong.md)

## ↑ Ancestors (14)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the thermal and statistical physics course of the University of Cambridge](../../../../split.md)
6. [Thermal and Statistical Physics course of the University of Cambridge](../../../../../thermal-and-statistical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
