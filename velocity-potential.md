# Velocity potential

↑ **Parent:** [Fluid mechanics](fluid-mechanics-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Velocity_potential)

Use a [velocity potential](velocity-potential.md) to reconstruct an [irrotational flow](irrotational-flow.md) from one [scalar field](scalar-field.md). A [velocity potential](velocity-potential.md) $\phi(\mathbf x,t)$ satisfies

$$
\mathbf u=\nabla\phi.
$$

It has units $\mathrm{m^2\,s^{-1}}$ and is unchanged as a description of the [velocity field](velocity-field.md) when any function of time alone is added. For twice continuously differentiable $\phi$, the identity [curl of a gradient](curl-of-a-gradient.md) proves zero [vorticity](vorticity.md). In [incompressible flow](incompressible-flow.md), taking the [divergence](divergence.md) also gives $\nabla^2\phi=0$, the [Laplace equation](laplace-equation.md). This turns a three-component [velocity field](velocity-field.md) into a single [harmonic function](harmonic-function.md) with appropriate [boundary conditions](boundary-condition.md). [A. H. Techet, MIT Hydrodynamics reading 4, pp. 1–3](https://ocw.mit.edu/courses/2-016-hydrodynamics-13-012-fall-2005/c472432debcf6ee250209b68cf18cc12_2005reading4.pdf)

For [uniform flow](uniform-flow.md) $\mathbf u=(U,0,0)$, take $\phi=Ux$. With $U=2\ \mathrm{m\,s^{-1}}$, the change from $x=0$ to $x=3\ \mathrm m$ is $\Delta\phi=6\ \mathrm{m^2\,s^{-1}}$. By the [fundamental theorem for line integrals](fundamental-theorem-for-line-integrals.md), the [line integral](line-integral.md) of [velocity](velocity.md) between these points equals that change along any path in the domain; a [closed curve](closed-curve.md) gives zero [circulation](circulation-physics.md).

For the potential [line vortex](line-vortex.md), choose a local angle branch in [polar coordinates](polar-coordinates.md) and set $\phi=K\theta$. Then $u_r=\partial_r\phi=0$ and $u_\theta=r^{-1}\partial_\theta\phi=K/r$. One counterclockwise turn changes the continued [velocity potential](velocity-potential.md) by $2\pi K$, although the [velocity field](velocity-field.md) returns to its original value. With $K=1\ \mathrm{m^2\,s^{-1}}$, this change is $2\pi\ \mathrm{m^2\,s^{-1}}$, exactly the [circulation](circulation-physics.md). A full [annulus](annulus-mathematics.md) therefore admits local angle branches and a multivalued [velocity potential](velocity-potential.md), but no global single-valued [velocity potential](velocity-potential.md) when $K\ne0$. Cutting the [annulus](annulus-mathematics.md) along a radial line allows a single-valued angle branch on the remaining domain. The obstruction is [path independence](path-independence.md), not a failure of the local [gradient](gradient.md) formula.

**Table of contents**

- [Potential flow around a circular cylinder](potential-flow-around-a-circular-cylinder.md)
  - [Potential flow around a circular cylinder with circulation](potential-flow-around-a-circular-cylinder-with-circulation.md)
    - [Kutta–Joukowski theorem](kutta-joukowski-theorem.md)
      - [Advective and pressure contributions to circulatory lift](advective-and-pressure-contributions-to-circulatory-lift.md)
- [Radially symmetric incompressible flow in a planar annulus](radially-symmetric-incompressible-flow-in-a-planar-annulus.md)
  - [Pressure in radially symmetric annular potential flow](pressure-in-radially-symmetric-annular-potential-flow.md)
    - [Small oscillation of a planar gas bubble in an annular liquid](small-oscillation-of-a-planar-gas-bubble-in-an-annular-liquid.md)

## ↑ Ancestors (4)

1. [Fluid mechanics](fluid-mechanics-split.md)
2. [Branches of physics](branches-of-physics.md)
3. [Physics](physics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (68)

- [Added mass of a circular cylinder](added-mass-of-a-circular-cylinder.md)
- [Dispersion relation of a floating elastic plate](dispersion-relation-of-a-floating-elastic-plate.md)
- [Equality of top-hat jet parity growth rates](equality-of-top-hat-jet-parity-growth-rates.md)
- [Finite-depth Rayleigh-Taylor dispersion relation](finite-depth-rayleigh-taylor-dispersion-relation.md)
- [Gravity-capillary wave](gravity-capillary-wave.md)
- [Hydrodynamic attraction of a plane wall to a point source](hydrodynamic-attraction-of-a-plane-wall-to-a-point-source.md)
- [Irrotational flow](irrotational-flow.md)
- [Kelvin-Helmholtz dispersion relation with gravity](kelvin-helmholtz-dispersion-relation-with-gravity.md)
- [Near-field energy imbalance in a spherical acoustic wave](near-field-energy-imbalance-in-a-spherical-acoustic-wave.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-1/15g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-3/18g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-3/8g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-45/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-74/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-74/4/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-3/21c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-75/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-1/17e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-3/18e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-4/18a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-82/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-82/2/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-3/18d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-84/4/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-1/17b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-1/17b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-4/18b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-1/38a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-4/37e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-77/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-78/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-71/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-57/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-57/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-65/1/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-72/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-78/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-4/35e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-1/17c/c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-1/5d/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-331/1/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-331/1/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-331/1/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-4/18d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-2/38c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-331/1/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-1/17c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ib/paper-1/17c/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ib/paper-2/16c/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4/38b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-1/16a/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-3/7a/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-4/16a/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-3/16c/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-3/16c/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-3/7c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-2/39c/c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4/38c/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-2/5d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-329/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-1/40c/a/solution.md)
- [Potential flow around a circular cylinder](potential-flow-around-a-circular-cylinder.md)
- [Potential flow around a circular cylinder with circulation](potential-flow-around-a-circular-cylinder-with-circulation.md)
- [Source dipole](source-dipole.md)
- [Synchronous perfect-fluid density equation](synchronous-perfect-fluid-density-equation.md)
- [Three-dimensional point source](three-dimensional-point-source.md)
- [Uniform flow](uniform-flow.md)
- [Velocity potential](velocity-potential.md)
