# Circulation (physics)

↑ **Parent:** [Vorticity](vorticity.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Circulation_(physics))

Use [circulation](circulation-physics.md) to summarize how much a [velocity field](velocity-field.md) runs along an oriented [closed curve](closed-curve.md) $C$, such as a [circle](circle.md) around a [fluid vortex](vortex-fluid-mechanics.md). Its definition is the [line integral](line-integral.md)

$$
\Gamma_C=\oint_C\mathbf u\cdot d\mathbf l,
$$

where $d\mathbf l$ is tangent to $C$ in the chosen direction. Reversing that direction reverses the sign of [circulation](circulation-physics.md). Its units are $\mathrm{m^2\,s^{-1}}$, because [velocity](velocity.md) is multiplied by a length. Counterclockwise [circulation](circulation-physics.md) in the horizontal plane is positive when the chosen [unit normal vector](unit-normal.md) is $+\mathbf e_z$, according to the [right-hand rule](right-hand-rule.md).

For [solid-body rotation](solid-body-rotation.md) $\mathbf u=(-\Omega y,\Omega x,0)$, a counterclockwise [circle](circle.md) of radius $R$ has constant tangential [velocity](velocity.md) $\Omega R$. Multiplying by its circumference gives

$$
\Gamma_C=2\pi\Omega R^2.
$$

For the potential [line vortex](line-vortex.md) $\mathbf u=K\mathbf e_\theta/r$, the same [circle](circle.md) instead gives $\Gamma_C=(K/R)(2\pi R)=2\pi K$, independent of $R$. Stipulate $\Omega=1\ \mathrm{s^{-1}}$, $R=1\ \mathrm m$ and $K=1\ \mathrm{m^2\,s^{-1}}$: both [velocity fields](velocity-field.md) have $\Gamma_C=2\pi\ \mathrm{m^2\,s^{-1}}\approx6.283185\ \mathrm{m^2\,s^{-1}}$, although their [vorticities](vorticity.md) in the fluid are $2\mathbf e_z\ \mathrm{s^{-1}}$ and zero respectively. On a [circle](circle.md) of radius $2\ \mathrm m$, their [circulations](circulation-physics.md) are $8\pi\ \mathrm{m^2\,s^{-1}}$ and $2\pi\ \mathrm{m^2\,s^{-1}}$. The comparison plot in [vorticity](vorticity.md) shows this difference in radius dependence.

The bridge between [circulation](circulation-physics.md) and [vorticity](vorticity.md) is [Stokes theorem](stokes-theorem.md):

$$
\Gamma_{\partial S}=\int_S\boldsymbol\omega\cdot\mathbf n\,dS.
$$

Here the [velocity field](velocity-field.md) must be continuously differentiable on a neighborhood of the entire spanning surface $S$ inside the fluid, and its boundary orientation must match the [unit normal vector](unit-normal.md) $\mathbf n$. For [solid-body rotation](solid-body-rotation.md), the disk is admissible and its [surface integral](surface-integral.md) is $2\Omega\pi R^2$. For the potential [line vortex](line-vortex.md), the origin is singular and excluded from the fluid: a disk crossing it is not admissible. On an [annulus](annulus-mathematics.md), [Stokes theorem](stokes-theorem.md) instead gives $\Gamma_{R_{\rm out}}-\Gamma_{R_{\rm in}}=0$, with both [circulations](circulation-physics.md) here measured counterclockwise; the induced inner boundary direction is clockwise. Nonzero [circulation](circulation-physics.md) therefore does not imply nonzero local [curl](curl.md) in the available fluid. [David Tong, Fluid Mechanics, section 2.2, circular-flow example](https://davidtong.org/pdfs/teaching/fluid-mechanics/fluids1.pdf)

This is useful because [Stokes theorem](stokes-theorem.md) lets a local [vorticity](vorticity.md) measurement determine a loop's [circulation](circulation-physics.md) when a suitable surface exists, while [Kelvin's circulation theorem](kelvin-s-circulation-theorem.md) tracks [circulation](circulation-physics.md) along a moving [material curve](material-curve.md). The beauty is the precise link between a local [derivative](derivative.md) and a global [line integral](line-integral.md), with the domain deciding which conclusions are valid.

**Table of contents**

- [Kelvin's circulation theorem](kelvin-s-circulation-theorem.md)
  - [Irrotational circulation in an exterior domain](irrotational-circulation-in-an-exterior-domain.md)

## ↑ Ancestors (5)

1. [Vorticity](vorticity.md)
2. [Fluid mechanics](fluid-mechanics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)
