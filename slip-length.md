# Slip length

↑ **Parent:** [Navier slip boundary condition](navier-slip-boundary-condition.md)

The [slip length](slip-length.md) measures tangential wall mobility in the [Navier slip boundary condition](navier-slip-boundary-condition.md). Where the wall [shear rate](shear-rate.md) is nonzero,

$$
b=\frac{u_{\mathrm{rel}}}{\partial_nu}.
$$

The numerator is a [velocity](velocity.md) and the denominator has units $\mathrm{s^{-1}}$, so $b$ has units of length. Geometrically, take a local inward normal coordinate $s$, with the wall at $s=0$. The tangent line to the relative [velocity](velocity.md) profile is

$$
u_{\mathrm{rel,lin}}(s)=u_{\mathrm{rel}}(0)+s\partial_nu(0)
=(b+s)\partial_nu(0).
$$

It reaches zero at $s=-b$, a fictitious distance $b$ inside the solid. This extrapolation does not assert that [fluid](fluid.md) exists there. At a moving wall, extrapolate to the wall's [velocity](velocity.md), rather than to zero laboratory [velocity](velocity.md). If both the wall [shear rate](shear-rate.md) and relative [velocity](velocity.md) vanish, their ratio cannot determine $b$.

The useful comparison is $b/H$, where $H$ is the channel gap. A small absolute [slip length](slip-length.md) can noticeably change [volumetric flow rate](volumetric-flow-rate.md) in a micrometre-scale channel. Measured effective [slip length](slip-length.md) may summarize unresolved interfacial structure; it need not mean literal molecular sliding at every point. The review distinguishes intrinsic, apparent and effective slip and discusses how surface conditions affect measurements. [Lauga, Brenner and Stone (2005), §§2.2 and 3.1: slip terminology and measurement](https://arxiv.org/pdf/cond-mat/0501557)

**Table of contents**

- [Couette flow with a slipping lower wall](couette-flow-with-a-slipping-lower-wall.md)
- [Planar Poiseuille flow with equal wall slip](planar-poiseuille-flow-with-equal-wall-slip.md)

## ↑ Ancestors (5)

1. [Navier slip boundary condition](navier-slip-boundary-condition.md)
2. [Fluid mechanics](fluid-mechanics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (10)

- [Couette flow with a slipping lower wall](couette-flow-with-a-slipping-lower-wall.md)
- [Linear basal drag law](linear-basal-drag-law.md)
- [Navier slip boundary condition](navier-slip-boundary-condition.md)
- [Navier-slip Taylor swimming sheet](navier-slip-taylor-swimming-sheet.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-80/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-332/3/solution.md)
- [Planar Poiseuille flow with equal wall slip](planar-poiseuille-flow-with-equal-wall-slip.md)
- [Rarefied gas flow approximations](rarefied-gas-flow-approximations.md)
- [Slip length](slip-length.md)
- [Wall friction in the Navier slip boundary condition](wall-friction-in-the-navier-slip-boundary-condition.md)
