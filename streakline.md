# Streakline

↑ **Parent:** [Fluid mechanics](fluid-mechanics-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Streakline)

A [streakline](streakline.md) at observation time $T$ is the set of present positions of all [fluid elements](fluid-element.md) that passed through one fixed release point $\mathbf a$ during a specified history of injection. For continuous release over $\tau_0\leq\tau\leq T$, solve a different [initial value problem](initial-value-problem.md) for each release time $\tau$:

$$
\frac{\partial\mathbf X}{\partial t}(t;\tau,\mathbf a)=\mathbf u(\mathbf X(t;\tau,\mathbf a),t),\qquad \mathbf X(\tau;\tau,\mathbf a)=\mathbf a,\qquad \mathcal S_T=\{\mathbf X(T;\tau,\mathbf a):\tau_0\leq\tau\leq T\}.
$$

Thus a [pathline](pathline.md) varies $t$ for one particle; a [streakline](streakline.md) varies $\tau$ while holding $T$ fixed. Interrupted release gives only the corresponding subsets of the [streakline](streakline.md). A moving nozzle requires a time-dependent release position instead, so the standard fixed-point definition should not silently be applied to it. Continuous release makes [streaklines](streakline.md) easy to observe and useful for showing where material from one source has reached. [MIT Marine Hydrodynamics, lecture 2, section 1.2](https://web.mit.edu/13.021/demos/lectures/lecture2.pdf)

In the analytical [velocity field](velocity-field.md) $(U,at)$ of [pathline](pathline.md), a particle released at the origin at time $\tau$ follows

$$
x(t;\tau)=U(t-\tau),\qquad y(t;\tau)=\frac a2(t^2-\tau^2),\qquad t\geq\tau.
$$

Observe all particles together at time $T$, after continuous release from $\tau=0$:

$$
x=U(T-\tau),\qquad y=\frac a2(T^2-\tau^2),\qquad y=\frac{aT}{U}x-\frac{a}{2U^2}x^2,\qquad 0\leq x\leq UT.
$$

For $U=1\ \mathrm{m\,s^{-1}}$, $a=1\ \mathrm{m\,s^{-2}}$ and $T=2\ \mathrm s$, the [streakline](streakline.md) is the downward-curving [parabola](parabola.md) $y=2x-x^2/2$ in metre coordinates. Releases at $\tau=0,1,2\ \mathrm s$ occupy $(2,2)$, $(1,1.5)$ and $(0,0)\ \mathrm m$, respectively. At $x=1\ \mathrm m$, the [streakline](streakline.md) lies above the [pathline](pathline.md) $y=x^2/2$ and below the origin's [streamline](streamline.md) $y=2x$. All particles nevertheless have the same present [velocity](velocity.md) $(1,2)\ \mathrm{m\,s^{-1}}$. The [streakline](streakline.md) slope $dy/dx=a\tau/U$ generally differs from the present [velocity](velocity.md) slope $aT/U$; they agree at the nozzle. The oldest particle is the downstream endpoint, which explains why the [pathline](pathline.md) and [streakline](streakline.md) meet there without being the same curve.

<a id="image-analytical-release-families-observed-at-one-and-two-seconds"></a>
![](stream-path-streak-lines-release-family.png)

**[Figure 15](#image-analytical-release-families-observed-at-one-and-two-seconds). Analytical release families observed at one and two seconds**.

Each panel fixes one observation time. Coloured dots are the present positions of particles with the indicated release times; dashed [pathlines](pathline.md) show those particles' earlier histories. The black [streakline](streakline.md) connects present positions of the continuously released family, including release times between the sampled dots. After $T=1\ \mathrm s$, particles already present keep moving and new ones enter at the origin, so the later [streakline](streakline.md) is not a frozen record of the earlier one. Injection beginning only at $\tau=1\ \mathrm s$ would show just $0\leq x\leq1\ \mathrm m$ of the $T=2\ \mathrm s$ curve. Both panels are diffusion-free analytical models, not experimental photographs.

Kline's contracting-channel demonstration switches from marking an element to continuous bubble production at a marking wire: the resulting trace is a [streakline](streakline.md). The apparatus therefore changes the curve being displayed by changing the marking history, even with the same channel. A wire produces a family of traces; conceptually each fixed emitting location supplies its own [streakline](streakline.md). Individual bubbles are markers rather than perfect [fluid elements](fluid-element.md): Jean Hertzberg's teaching notes describe [hydrogen](hydrogen.md) production by [electrolysis](electrolysis.md) at a thin [cathode](cathode.md) wire and warn that larger bubbles have more [buoyancy](buoyancy.md). [S. J. Kline, Flow Visualization film notes, figure 8](https://web.mit.edu/hml/ncfmf/05FV.pdf) [Jean Hertzberg and Flow Vis course students, Particles 3: In Water](https://www.flowvis.org/Flow%20Vis%20Guide/particles-3-in-water/)

A dye version uses a small fixed injection port upstream in a transparent water channel, a dilute premix of dye with the channel water, illumination and a fixed [optical camera](optical-camera.md). Start continuous injection at a recorded time $\tau_0$ and take a short exposure at $T$: the visible filament approximates a [streakline](streakline.md), not the accumulated [pathline](pathline.md) of one particle. Repeat with the same port and imaging geometry after changing the flow with time; compare the filament against local directions estimated from short displacements of sparse markers at $T$. Agreement in a [steady flow](steady-flow.md) and possible disagreement when the flow changes are the predictions being tested; no measured curves are claimed here. The protocol follows Hertzberg's advice to use small ports, little injected volume and a dilute premix with matched [density](density.md) and [viscosity](dynamic-viscosity-split.md). Check for nozzle disturbance by reducing injection rate, for [buoyancy](buoyancy.md) by watching the premix in still water, and for [diffusion](diffusion.md) by comparing filament widths at different ages. Keep exposure short enough to suppress motion blur. Dye [concentration](concentration.md) approximates a [passive scalar](passive-scalar.md) only when it has negligible feedback on the [velocity field](velocity-field.md); finite port width, [diffusion](diffusion.md) and out-of-plane motion limit how literally a visible filament can be read as a geometrical [streakline](streakline.md). [Jean Hertzberg and Flow Vis course students, Dye Techniques 1: Do Not Disturb](https://www.flowvis.org/Flow%20Vis%20Guide/do-not-disturb-dyes-in-liquids/)

## ↑ Ancestors (4)

1. [Fluid mechanics](fluid-mechanics-split.md)
2. [Branches of physics](branches-of-physics.md)
3. [Physics](physics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Laminar flow](laminar-flow.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-1/6c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-2/5c/c/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2019/paper-1/section-c/c12/solution.md)
- [Pathline](pathline.md)
- [Streakline](streakline.md)
- [Streamline](streamline.md)
