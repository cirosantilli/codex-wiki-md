<h1 id="bernoulli-s-principle">Bernoulli's principle</h1>

↑ **Parent:** [Euler equations for an inviscid fluid](euler-equations-for-an-inviscid-fluid.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bernoulli's_principle)

The [Bernoulli principle](bernoulli-s-principle.md) relates [pressure](pressure.md), [kinetic energy](kinetic-energy.md) per unit volume and [Newtonian gravitational potential](newtonian-gravitational-potential.md) along a [streamline](streamline.md) of [steady flow](steady-flow.md) with [inviscid flow](inviscid-flow.md). For constant [mass density](density.md), the [Bernoulli equation](bernoulli-equation.md) gives $p/\rho+u^2/2+\Phi$ constant along that [streamline](streamline.md). Constancy across different [streamlines](streamline.md) requires further hypotheses, such as [irrotational flow](irrotational-flow.md).

Precisely, suppose a [fluid](fluid.md) of constant positive [mass density](density.md) obeys the [Euler equations for an inviscid fluid](euler-equations-for-an-inviscid-fluid.md), its [velocity field](velocity-field.md) and [pressure](pressure.md) are steady, and the body [force](force.md) per unit [mass](mass.md) is $-\nabla\Phi$. Then

$$
B=\frac{p}{\rho}+\frac{|\mathbf u|^2}{2}+\Phi,\qquad \mathbf u\cdot\nabla B=0.
$$

Every term has units of [energy](energy.md) per unit [mass](mass.md). For a uniform gravitational field, [Newtonian gravitational potential](newtonian-gravitational-potential.md) is $\Phi=gz$, up to an additive constant. The [pressure](pressure.md) term represents work by surrounding [fluid](fluid.md), so acceleration can exchange [pressure](pressure.md) work with [kinetic energy](kinetic-energy.md). Dotting the steady [Euler equations](euler-equations-for-an-inviscid-fluid.md) with $\mathbf u$ gives the displayed [directional derivative](directional-derivative.md): this is why constancy follows a [streamline](streamline.md). [Cambridge, Fluid Dynamics IB, Dynamics, section 2.4](https://www.damtp.cam.ac.uk/user/mem2/FLUIDS-IB/dyn.pdf)

Continue the horizontal water constriction example from [incompressible flow](incompressible-flow.md). Assume negligible viscous losses, [steady flow](steady-flow.md) and approximately [uniform flow](uniform-flow.md) at both measurement sections, so the [streamline](streamline.md) speeds there equal the mean speeds $0.20$ and $0.80\,\mathrm{m\,s^{-1}}$. Equal height cancels the [Newtonian gravitational potential](newtonian-gravitational-potential.md) terms. The ideal [pressure](pressure.md) drop is

$$
p_1-p_2=\frac{\rho}{2}(U_2^2-U_1^2)=\frac{1000}{2}(0.80^2-0.20^2)=300\,\mathrm{Pa}.
$$

This is the [Venturi effect](venturi-effect.md) in its ideal limit: the gain in [kinetic energy](kinetic-energy.md) density is supplied by [pressure](pressure.md) work. Cambridge's treatment uses this relation to connect a measured [pressure](pressure.md) difference to [volumetric flow rate](volumetric-flow-rate.md). [Cambridge, Fluid Dynamics IB, Dynamics, section 2.5](https://www.damtp.cam.ac.uk/user/mem2/FLUIDS-IB/dyn.pdf)

The $300\,\mathrm{Pa}$ result is conditional, rather than a prediction of the actual viscous pipe. [Mass conservation](mass-conservation.md) fixes $Q$ and the ratio of mean speeds even with [viscosity](dynamic-viscosity.md), but nonuniform [velocity profiles](velocity-profile.md) require an integrated [energy](energy.md) balance, and wall friction dissipates mechanical [energy](energy.md). A pump would supply additional work. In particular, constant mean speed in a straight pipe does not imply constant [pressure](pressure.md): [Poiseuille flow](hagen-poiseuille-equation.md) needs a continuing [pressure gradient](pressure-gradient.md) to overcome [viscosity](dynamic-viscosity.md). [UCL, Bernoulli's equation, assumptions and boundary limitations](https://uclnatsci.github.io/2021/Electromagnetism-Fluids-and-Waves/fluids/bernoulli.html)

**Table of contents**

- [Venturi effect](venturi-effect.md)

## ↑ Ancestors (5)

1. [Euler equations for an inviscid fluid](euler-equations-for-an-inviscid-fluid.md)
2. [Fluid mechanics](fluid-mechanics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Fluid mechanics](fluid-mechanics-split.md)
- [Incompressible flow](incompressible-flow.md)
- [Pressure coefficient](pressure-coefficient.md)
- [Reynolds number](reynolds-number.md)
- [Unsteady Bernoulli equation](unsteady-bernoulli-equation.md)
