<h1 id="torricelli-s-law">Torricelli's law</h1>

↑ **Parent:** [Fluid mechanics](fluid-mechanics-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Torricelli's_law)

An ideal fluid issuing from a small hole a vertical depth $h$ below a free surface has speed

$$
v=\sqrt{2gh}.
$$

Here $h$ is the vertical distance from the [free surface](free-surface.md) to the centre of the [orifice](orifice.md), and $g$ is the positive magnitude of [gravitational acceleration](gravitational-acceleration.md). The ideal prediction assumes [incompressible flow](incompressible-flow.md), the same ambient [pressure](pressure-split.md) at the [free surface](free-surface.md) and emerging jet, negligible [velocity](velocity.md) of the reservoir's [free surface](free-surface.md), and negligible [viscous dissipation](viscous-dissipation.md) and [surface tension](surface-tension-split.md) effects. For a falling [free surface](free-surface.md), a [quasi-steady approximation](quasi-steady-approximation.md) additionally assumes that the local outflow adjusts much faster than $h$ changes. It applies the [Bernoulli equation](bernoulli-equation.md) at each instant, rather than claiming that the whole drainage is [steady flow](steady-flow.md).[Macro Scale Derivation and Common Assumptions: steady, inviscid, incompressible streamline balance and the gravity-height term](bernoulli%E2%80%99s-equation-by-nasa-glenn-research-center.md)

A short proof uses a [streamline](streamline.md) connecting the reservoir's [free surface](free-surface.md) at elevation $z_s$ to the emerging jet at elevation $z_o$. With constant [mass density](density.md) $\rho$, negligible surface [speed](speed.md) and no mechanical [energy](energy-split.md) losses, the [Bernoulli equation](bernoulli-equation.md) gives

$$
\frac{p_{\mathrm{ambient}}}{\rho}+gz_s
=\frac{p_{\mathrm{ambient}}}{\rho}+\frac{v^2}{2}+gz_o,
\qquad h=z_s-z_o.
$$

Equal [pressures](pressure-split.md) cancel, leaving $v^2/2=gh$: a unit [mass](mass.md) gains the same [kinetic energy](kinetic-energy.md) as a body in [free fall](free-fall.md) through height $h$. This makes [Torricelli's law](torricelli-s-law.md) a useful first estimate before the detailed [velocity field](velocity-field.md) is known. At one quarter of the original head, ideal jet [speed](speed.md) is one half as large; it is not proportional to head.

<a id="image-torricelli-geometry-equal-boundary-pressures-and-a-vertical-head"></a>
![](torricelli-reservoir-head-and-pressure.png)

**[Figure 9](#image-torricelli-geometry-equal-boundary-pressures-and-a-vertical-head). Torricelli geometry: equal boundary pressures and a vertical head**. Original schematic of ideal outflow, not measured apparatus or a scale drawing. The [free surface](free-surface.md) and emerging jet share ambient [pressure](pressure-split.md). Head $h$ is measured to the [orifice](orifice.md) centre. Bulk [hydrostatic pressure](hydrostatic-pressure.md) at that elevation is a different quantity from jet [pressure](pressure-split.md).

Far from the accelerating outlet region, the reservoir has approximately [hydrostatic pressure](hydrostatic-pressure.md) $p_{\mathrm{ambient}}+\rho gh$ at the outlet's elevation. The emerging jet instead has approximately ambient [pressure](pressure-split.md) when [surface tension](surface-tension-split.md) is negligible. Do not assign that bulk [hydrostatic pressure](hydrostatic-pressure.md) to the emerging jet as well as adding the height difference: that would count the available mechanical [energy](energy-split.md) twice. A sealed reservoir, a submerged outlet or significant [surface tension](surface-tension-split.md) changes the [pressure](pressure-split.md) conditions and requires a different balance.

Actual [volumetric flow rate](volumetric-flow-rate.md) is commonly represented by a [discharge coefficient](discharge-coefficient.md):

$$
Q=C_d a\sqrt{2gh},\qquad C_d=\frac{Q}{a\sqrt{2gh}},
$$

where $a$ is the geometric [area](surface-area.md) of the [orifice](orifice.md). This definition compares [volumetric flow rates](volumetric-flow-rate.md), not just [speeds](speed.md). If a nearly uniform jet at its [vena contracta](vena-contracta.md) has [area](surface-area.md) $a_j$ and [speed](speed.md) $v_j$, define the two separate ratios $C_c=a_j/a$ and $C_v=v_j/\sqrt{2gh}$. Then $Q=a_jv_j$ gives $C_d=C_cC_v$. A contracted jet can consequently have a [speed](speed.md) close to $\sqrt{2gh}$ while $C_d$ is appreciably below one. No particular $C_d$ is universal: calibrate it for the opening and operating range.

**Table of contents**

- [Draining tank with constant cross-sectional area](draining-tank-with-constant-cross-sectional-area.md)
- [Discharge measurement in a draining tank](discharge-measurement-in-a-draining-tank.md)
- [Drainage time of a conical tank](drainage-time-of-a-conical-tank.md)

## ↑ Ancestors (4)

1. [Fluid mechanics](fluid-mechanics-split.md)
2. [Branches of physics](branches-of-physics.md)
3. [Physics](physics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Drainage time of a conical tank](drainage-time-of-a-conical-tank.md)
- [Evangelista Torricelli](evangelista-torricelli.md)
- [James F. Price](james-f-price.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-2/7d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-2/5a/a/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2011/paper-1/section-a/a2/solution.md)
- [Torricelli's law](torricelli-s-law.md)
