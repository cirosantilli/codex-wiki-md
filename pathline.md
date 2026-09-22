# Pathline

↑ **Parent:** [Fluid mechanics](fluid-mechanics-split.md)

A [pathline](pathline.md) records the motion of one identified [fluid element](fluid-element.md): keep its starting position $\mathbf a$ and starting time $t_0$ fixed, and let physical time $t$ advance. In a [velocity field](velocity-field.md) $\mathbf u(\mathbf x,t)$ its [Lagrangian trajectory](lagrangian-trajectory.md) $\mathbf X(t;t_0,\mathbf a)$ solves the [initial value problem](initial-value-problem.md)

$$
\frac{d\mathbf X}{dt}=\mathbf u(\mathbf X(t),t),\qquad \mathbf X(t_0;t_0,\mathbf a)=\mathbf a.
$$

A [streamline](streamline.md) instead freezes the time argument of the [velocity field](velocity-field.md); a [streakline](streakline.md) fixes the observation time and varies the release time of many [fluid elements](fluid-element.md). A [pathline](pathline.md) is useful for answering where a particular parcel goes and how long it takes, rather than merely which way the [fluid](fluid.md) is moving now. [MIT Marine Hydrodynamics, lecture 2, sections 1.1–1.2](https://web.mit.edu/13.021/demos/lectures/lecture2.pdf)

For a concrete analytical model, take spatial coordinates $x,y$ in metres, time $t\geq0$ in seconds, and the spatially uniform but time-dependent [velocity field](velocity-field.md)

$$
\mathbf u(x,y,t)=(U,at),\qquad U=1\ \mathrm{m\,s^{-1}},\qquad a=1\ \mathrm{m\,s^{-2}}.
$$

Its numerical components in these units are $(1,t)$. A [fluid element](fluid-element.md) starting at the origin at $t_0=0$ has the [pathline](pathline.md)

$$
x(t)=Ut,\qquad y(t)=\frac{at^2}{2},\qquad y=\frac{a}{2U^2}x^2.
$$

At $t=1\ \mathrm s$ it is at $(1,0.5)\ \mathrm m$; at $t=2\ \mathrm s$ it is at $(2,2)\ \mathrm m$. The [parabola](parabola.md) records earlier, shallower [velocity](velocity.md) directions as well as the final direction. Differentiating gives $(\dot x,\dot y)=(U,at)$ and [acceleration](acceleration.md) $(0,a)$, so this curved [pathline](pathline.md) needs no spatial variation of the [velocity field](velocity-field.md). More generally the [chain rule](chain-rule.md) along a [pathline](pathline.md) gives $d f(\mathbf X(t),t)/dt=\partial_t f+\mathbf u\cdot\nabla f$, the [material derivative](material-derivative.md) of a transported [scalar field](scalar-field.md).

A motivating tracer demonstration appears in S. J. Kline's film notes: water passes through a contracting channel, and [hydrogen](hydrogen.md) bubbles mark a small element at a wire at time $t_0$. The illustrated element is shown again $4.7\ \mathrm s$ later, with its accumulated [pathline](pathline.md) superposed. Following that same marked element across successive film frames records a history; the entire bubble pattern in one frame has a different meaning. [S. J. Kline, Flow Visualization film notes, figures 7a–7c](https://web.mit.edu/hml/ncfmf/05FV.pdf)

For a modern version of the readout, use sparse small markers in a transparent water channel, illuminate the viewed plane, and keep an [optical camera](optical-camera.md) fixed with a ruler in that plane. Record timestamps and track the same isolated marker between frames; successive positions estimate its [pathline](pathline.md) and $[\mathbf X(t+\Delta t)-\mathbf X(t)]/\Delta t$ estimates its [velocity](velocity.md). A long exposure records a [pathline](pathline.md) segment but loses the timing within it, so its total length divided by exposure time gives only mean [speed](speed.md). These are proposed measurement steps based on Jean Hertzberg's teaching guidance, rather than additional measurements from Kline's film. Markers leaving the viewed plane, overlapping tracks and perspective can break particle identification; repeat with a thinner viewed slice and a lower marker [concentration](concentration.md). [Jean Hertzberg and Flow Vis course students, Particles 4: Dilute Particle Techniques](https://www.flowvis.org/Flow%20Vis%20Guide/particles-4-dilute/)

## ↑ Ancestors (4)

1. [Fluid mechanics](fluid-mechanics-split.md)
2. [Branches of physics](branches-of-physics.md)
3. [Physics](physics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (10)

- [Irrotational flow](irrotational-flow.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-1/6c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-1/5e/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-1/5e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ib/paper-1/5a/solution.md)
- [Pathline](pathline.md)
- [Streakline](streakline.md)
- [Streamline](streamline.md)
- [Vorticity](vorticity.md)
- [Vorticity of a linear shear flow](vorticity-of-a-linear-shear-flow.md)
