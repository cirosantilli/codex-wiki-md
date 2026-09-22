# Similarity solution for a sink-flow boundary layer

↑ **Parent:** [Sink flow in a sector](sink-flow-in-a-sector.md)

Near a radial wall, let $x$ measure distance from the sink along the wall and $y$ point into the fluid. With

$$
\delta=x\sqrt{\frac\nu Q},
\qquad
\eta=\frac y\delta,
\qquad
\psi=\sqrt{\nu Q}\,f(\eta),
$$

the [Prandtl boundary-layer equation](prandtl-boundary-layer-equation.md) reduces to

$$
f'''=1-(f')^2,
\qquad
f(0)=f'(0)=0,
\qquad
f'(\infty)=-1.
$$

One physical solution has

$$
f'(\eta)=\frac{5-\cosh(\sqrt2\eta+c)}{1+\cosh(\sqrt2\eta+c)},
\qquad
c=\operatorname{arcosh}5.
$$

## ↑ Ancestors (6)

1. [Sink flow in a sector](sink-flow-in-a-sector.md)
2. [Potential flow](potential-flow.md)
3. [Fluid mechanics](fluid-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
