<h1 id="b/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The first [energy](../../../../energy-split.md) term is the rate of change of internal plus [kinetic energy](../../../../kinetic-energy.md) per unit volume; the second transports that [energy](../../../../energy-split.md) with the moving gas; the [pressure](../../../../pressure-split.md) term is the mechanical [work](../../../../work.md) [flux](../../../../flux.md) across the boundary. There is no [heat flux](../../../../heat-flux-density.md) or viscous [work](../../../../work.md) in the stated inviscid [adiabatic](../../../../adiabatic-process.md) model.

Use mass conservation to replace a conservative derivative of $\rho e$ by $\rho De/Dt$. Dotting the momentum equation with $\mathbf u$ gives $\rho D(|\mathbf u|^2/2)/Dt=-\mathbf u\cdot\nabla p$. Subtraction from total [energy](../../../../energy-split.md) leaves

$$
\rho c_v\frac{DT}{Dt}+p\nabla\cdot\mathbf u=0.
$$

Now $p=\rho RT$ and $D\rho/Dt=-\rho\nabla\cdot\mathbf u$ imply

$$
\frac{DS}{Dt}=c_v\left(\frac1p\frac{Dp}{Dt}-\frac\gamma\rho\frac{D\rho}{Dt}\right)=\frac{c_v}T\frac{DT}{Dt}+R\nabla\cdot\mathbf u=0.
$$

Thus $\boxed{DS/Dt=0}$: smooth [adiabatic](../../../../adiabatic-process.md) inviscid trajectories are [isentropic](../../../../isentropic-flow.md). [Shocks](../../../../shock-wave.md) need an [entropy inequality](../../../../lagrangian-entropy-inequality.md) rather than this smooth equality.

Adding $\nabla\cdot(k\nabla T)$ models [Fourier heat conduction](../../../../fourier-s-law.md), with [heat flux](../../../../heat-flux-density.md) $-k\nabla T$. The same subtraction gives $\rho c_vDT/Dt+p\nabla\cdot\mathbf u=\nabla\cdot(k\nabla T)$, hence

$$
\boxed{T\frac{DS}{Dt}=\frac1\rho\nabla\cdot(k\nabla T).}
$$

For a fixed container use impermeability $\mathbf u\cdot\mathbf n=0$, insulation $k\nabla T\cdot\mathbf n=0$, and mass conservation. Then

$$
\frac d{dt}\int_D\rho S\,dV=\int_D\frac1T\nabla\cdot(k\nabla T)\,dV=\int_D\frac{k|\nabla T|^2}{T^2}\,dV.
$$

The boundary term vanishes and $\nabla(1/T)=-\nabla T/T^2$ supplies the positive sign. For $T>0$, $k\geq0$, total [entropy](../../../../entropy-split.md) cannot decrease: this is [entropy production by Fourier heat conduction](../../../../entropy-production-by-fourier-heat-conduction.md).

## ↑ Ancestors (12)

1. [5](../5.md)
2. [B](../../b.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the theoretical mechanics course of the University of Oxford](../../../split.md)
5. [Theoretical mechanics course of the University of Oxford](../../../../theoretical-mechanics-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
