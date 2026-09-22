<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Choose $x$ upslope and $z$ normally downwards from the impermeable roof, so the buoyant layer occupies $0<z<h(x,t)$. Use the [hydrostatic approximation](../../../../../../hydrostatic-approximation.md) and neglect the ambient return-flow [pressure](../../../../../../pressure.md) correction of relative order $h/H$. [Pressure](../../../../../../pressure.md) continuity at the interface gives the [pressure](../../../../../../pressure.md) inside the buoyant layer as

$$
p=p_0-\rho gx\sin\theta+\Delta\rho\,gh\cos\theta+(\rho-\Delta\rho)gz\cos\theta.
$$

The along-slope [Darcy velocity](../../../../../../darcy-velocity.md) is therefore

$$
v_D=-\frac{k}{\mu}\left[p_x+(\rho-\Delta\rho)g\sin\theta\right]=\frac{kg\Delta\rho}{\mu}(\sin\theta-\cos\theta\,h_x).
$$

Define $u=kg\Delta\rho\sin\theta/\mu$. Integrating over depth gives the [volume flux per unit width](../../../../../../volume-flux-per-unit-width.md) $F=uh-u\cot\theta\,hh_x$. Local fluid-volume conservation, including [porosity](../../../../../../porosity.md), is $\phi h_t+F_x=0$. Hence the [inclined porous gravity current](../../../../../../inclined-porous-gravity-current.md) satisfies

$$
\boxed{\phi h_t=-\frac{kg\Delta\rho}{\mu}\sin\theta\left[h_x-\cot\theta\,(hh_x)_x\right].}
$$

The first term is upslope [advection](../../../../../../advection.md) driven by the [mass density](../../../../../../density.md) difference; the second is nonlinear hydrostatic spreading. The [Darcy velocity](../../../../../../darcy-velocity.md) $u$ and the corresponding [pore velocity](../../../../../../pore-velocity.md) $u/\phi$ must be distinguished.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
