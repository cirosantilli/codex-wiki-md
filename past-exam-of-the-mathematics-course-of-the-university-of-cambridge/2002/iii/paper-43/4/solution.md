<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

[Magnetic flux concentration](../../../../../magnetic-flux-concentration.md) and [flux expulsion](../../../../../flux-expulsion.md) describe redistribution of an existing field, not necessarily creation of net flux. For a weak field in a prescribed conducting flow, the [resistive induction equation](../../../../../resistive-induction-equation.md) is

$$
\partial_t\mathbf B=\nabla\times(\mathbf u\times\mathbf B)+\eta\nabla^2\mathbf B.
$$

Its ideal part combines transport, stretching and compression:

$$
\frac{D\mathbf B}{Dt}=(\mathbf B\cdot\nabla)\mathbf u
-\mathbf B\nabla\cdot\mathbf u+\eta\nabla^2\mathbf B.
$$

Thus a converging flow can intensify a component, and stretching can increase [magnetic energy](../../../../../magnetic-energy.md) even if the signed net flux is zero. At large [magnetic Reynolds number](../../../../../magnetic-reynolds-number.md) $\mathrm{Rm}=UL/\eta$, [diffusion](../../../../../diffusion.md) is initially slow on the eddy scale, so [magnetic flux freezing](../../../../../magnetic-flux-freezing.md) carries field lines with the flow. These statements do not imply that an ideal closed eddy can simply lose its initially enclosed flux.

The missing step is the production of small scales by differential circulation. In a two-dimensional incompressible eddy, the [Cartesian magnetic flux function](../../../../../cartesian-magnetic-flux-function.md) obeys

$$
A_t+\mathbf u\cdot\nabla A=\eta\nabla^2A,\qquad
\mathbf B=(-A_z,0,A_x).
$$

Different [streamlines](../../../../../streamline.md) have different circulation rates. An initially smooth field is wound into fine folds; [diffusion](../../../../../diffusion.md) and reconnection then smooth the variation of $A$ inside the eddy. As $A$ becomes nearly uniform there, its [gradient](../../../../../gradient.md) and hence the interior [magnetic field](../../../../../magnetic-field.md) become small. The surviving flux lies mainly near the circulation boundary and adjacent [separatrices](../../../../../separatrix.md), where stronger gradients remain. This is [flux expulsion](../../../../../flux-expulsion.md). With exactly zero diffusivity, field topology and the flux of material loops remain frozen, so a relaxed flux-free interior is not obtained by pure advection alone. Rigid rotation also fails to generate the differential winding responsible for this process.

The [phase mixing in magnetic flux expulsion](../../../../../phase-mixing-in-magnetic-flux-expulsion.md) estimate makes the enhanced role of small [diffusion](../../../../../diffusion.md) explicit. If the angular-velocity [gradient](../../../../../gradient.md) is of order $U/L^2$, a wound radial [wavenumber](../../../../../wavenumber.md) grows as $k_r\sim Ut/L^2$. The accumulated damping exponent is of order

$$
\eta\int_0^t k_r(t')^2\,dt'\sim\frac{\eta U^2t^3}{L^4}.
$$

It becomes order one at

$$
\boxed{t_{\mathrm{exp}}\sim\left(\frac{L^4}{\eta U^2}\right)^{1/3}
=\frac LU\mathrm{Rm}^{1/3}.}
$$

This is much shorter than the large-scale [diffusion](../../../../../diffusion.md) time $(L/U)\mathrm{Rm}$ at large $\mathrm{Rm}$, but longer than one turnover time. It is a kinematic differential-shear estimate, not a universal time for every turbulent or rapidly evolving [convection cell](../../../../../convection-cell.md).

A related concentration mechanism occurs at converging flow boundaries. For a locally vertical bundle, conservation of flux gives $B\mathcal A\simeq\mathrm{constant}$, so reducing its cross-section increases $B$. In a simple converging boundary region with strain rate $U/L$, balancing strain and transverse [diffusion](../../../../../diffusion.md) gives

$$
\frac UL\sim\frac\eta{\delta^2},\qquad
\delta\sim L\mathrm{Rm}^{-1/2}.
$$

This is the thickness estimate for that local strain-diffusion model; it need not be the thickness or energy scaling of every closed-eddy flux-expulsion problem. Stronger field eventually exerts [Lorentz force](../../../../../lorentz-force.md) feedback and changes the flow. The [equipartition magnetic field](../../../../../equipartition-magnetic-field.md) $B_{\mathrm{eq}}=\sqrt{\mu_0\rho}\,U$ is a useful indication that the kinematic assumption can fail, not a universal upper bound on concentrated fields.

At the [Sun](../../../../../sun.md)'s [photosphere](../../../../../photosphere.md), hot upflows form [solar granules](../../../../../solar-granule.md), and their spreading horizontal motion transports weak vertical field toward cooler [intergranular lanes](../../../../../intergranular-lane.md) and downflows. A thin-layer illustration, neglecting vertical transport terms, is $\partial_tB_z+\nabla_h\cdot(\mathbf u_hB_z)=0$. It gives $D_hB_z/Dt=-B_z\nabla_h\cdot\mathbf u_h$: horizontal convergence intensifies the vertical flux [density](../../../../../density.md). This surface transport is related to the redistribution by convective eddies, but is not identical to the closed-streamline mechanism in the preceding planar example. Larger-scale [supergranulation](../../../../../supergranulation.md) also gathers magnetic elements toward its boundaries, helping organize the [solar magnetic network](../../../../../solar-magnetic-network.md).

Concentration can be further intensified by compressible thermal dynamics. In the thin-tube picture of [convective collapse](../../../../../convective-collapse.md), an unstable downward flow drains gas, reduces internal [pressure](../../../../../pressure.md) and allows contraction at approximately conserved flux. Lateral balance $p_i+B^2/(2\mu_0)\simeq p_e$ then permits field stronger than the local kinetic equipartition estimate. This evacuation mechanism is excluded by a strict [Boussinesq approximation](../../../../../boussinesq-approximation.md). It is not a description of every evolving surface concentration: gas [pressure](../../../../../pressure.md), dynamic stresses and magnetic curvature can all matter when thin-tube equilibrium fails. The resulting strong, intermittent magnetic elements are associated with intergranular structure; their radiative appearance also depends on thermal structure and opacity. The organized fields of [sunspots](../../../../../sunspot.md) require a broader account of flux supply and magnetic feedback, rather than attribution to weak-field expulsion alone.

Thus **[convection](../../../../../convection.md) redistributes and concentrates flux, finite [diffusion](../../../../../diffusion.md) enables classical expulsion, and nonlinear magnetic and thermal feedback determines the strong-field outcome**. An expulsion argument alone neither supplies the original solar field nor establishes a self-sustaining [solar dynamo](../../../../../solar-dynamo.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 43](../../paper-43-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
