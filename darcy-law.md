# Darcy law

↑ **Parent:** [Porous-media flow](porous-media-flow-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Darcy_law)

[Darcy law](darcy-law.md) is a linear relation between the bulk [Darcy flux](darcy-velocity.md) and the net driving force per unit volume. For an [isotropic](isotropy.md) [porous medium](porous-medium.md) containing one fully saturating [Newtonian fluid](newtonian-fluid.md),

$$
\mathbf q=-\frac{k}{\mu}\bigl(\nabla p-\rho\mathbf g\bigr).
$$

Here $\mathbf q$ is the [Darcy velocity](darcy-velocity.md) relative to the solid framework, $k$ is the intrinsic [permeability of a porous medium](permeability-of-a-porous-medium.md), $\mu>0$ is [dynamic viscosity](dynamic-viscosity-split.md), $p$ is averaged [fluid pressure](fluid-pressure.md), $\rho$ is [mass density](density.md), and $\mathbf g$ is the downward [gravitational acceleration](gravitational-acceleration.md) vector. The [pressure gradient](pressure-gradient.md) exerts force density $-\nabla p$, while [gravity](gravity.md) contributes $\rho\mathbf g$; the minus sign makes the discharge follow their sum. The symbols $\mathbf u$ and $\mathbf q$ are both commonly used for [Darcy velocity](darcy-velocity.md); neither denotes [pore velocity](pore-velocity.md) here.

With upward coordinate $z$ and positive [gravitational acceleration](gravitational-acceleration.md) magnitude $g$, $\mathbf g=-g\mathbf e_z$. Constant $\rho$ and $g$ therefore give

$$
\nabla p-\rho\mathbf g=\nabla p+\rho g\mathbf e_z=\rho g\nabla\left(z+\frac{p}{\rho g}\right),\qquad \mathbf q=-K\nabla h,\qquad K=\frac{k\rho g}{\mu}.
$$

The [hydraulic head](hydraulic-head.md) $h=z+p/(\rho g)$ combines elevation and [fluid pressure](fluid-pressure.md), and [hydraulic conductivity](hydraulic-conductivity.md) $K$ combines the medium and [fluid](fluid.md) properties. [Hydrostatic pressure](hydrostatic-pressure.md) satisfies $\nabla p=\rho\mathbf g$, so it produces zero [Darcy flux](darcy-velocity.md) even though [fluid pressure](fluid-pressure.md) increases downward. Conversely, equal pressures at the two ends of a vertical column do not imply zero flow: their elevations give different [hydraulic heads](hydraulic-head.md).

The appeal of [Darcy law](darcy-law.md) is that a complicated connected pore geometry enters a macroscopic calculation through a measurable coefficient. It predicts filter discharge and [aquifer](aquifer.md) flow; combined with [mass conservation](mass-conservation.md), it gives an equation for the evolving [fluid pressure](fluid-pressure.md). Its simple linear form requires a small pore-scale [Reynolds number](reynolds-number.md), slow adjustment compared with pore-scale inertial relaxation, and a valid [continuum approximation](continuum-approximation.md). For a characteristic pore size $d$ and mean [pore velocity](pore-velocity.md) $v$, one possible convention is $\mathrm{Re}_{\rm pore}=\rho|v|d/\mu\ll1$; conventions using grain size or [Darcy velocity](darcy-velocity.md) have different numerical thresholds. Merely calling flow laminar does not guarantee negligible inertia. Unsaturated pores, several [fluid](fluid.md) phases, appreciable inertia, or a [fluid](fluid.md) whose stress is not Newtonian require further modeling. Woessner and Poeter discuss these limits in their authored hydrology text.[https://books.gw-project.org/hydrogeologic-properties-of-earth-materials-and-principles-of-groundwater-flow/chapter/applicability-of-darcys-law/](https://books.gw-project.org/hydrogeologic-properties-of-earth-materials-and-principles-of-groundwater-flow/chapter/applicability-of-darcys-law/)

Henry Darcy's 1856 book _Les fontaines publiques de la ville de Dijon_ was published by Victor Dalmont; the University Grenoble Alpes digital collection verifies this bibliographic record and supplies a digitized copy.[https://bibnum-patrimoniale.univ-grenoble-alpes.fr/items/show/1643](https://bibnum-patrimoniale.univ-grenoble-alpes.fr/items/show/1643) Woessner and Poeter's account connects [Darcy law](darcy-law.md) to experiments on water flowing through sand filters, relating discharge to cross-sectional area, [hydraulic head](hydraulic-head.md) difference and sample length.[https://books.gw-project.org/hydrogeologic-properties-of-earth-materials-and-principles-of-groundwater-flow/chapter/darcys-law/](https://books.gw-project.org/hydrogeologic-properties-of-earth-materials-and-principles-of-groundwater-flow/chapter/darcys-law/) The modern intrinsic [permeability of a porous medium](permeability-of-a-porous-medium.md) notation above should not be read as a quotation of Darcy's original notation.

**Table of contents**

- [Hydraulic head](hydraulic-head.md)
- [Hydraulic conductivity](hydraulic-conductivity.md)
- [Darcy flow through a homogeneous slab](darcy-flow-through-a-homogeneous-slab.md)
- [Darcy flow](darcy-flow.md)
  - [Lubrication boundary condition for a crack in a Darcy medium](lubrication-boundary-condition-for-a-crack-in-a-darcy-medium.md)
    - [Crack pressure in elliptic coordinates](crack-pressure-in-elliptic-coordinates.md)
      - [Elliptic crack pressure dipole](elliptic-crack-pressure-dipole.md)
        - [Fixed-throughflow dissipation reduction of a conductive crack](fixed-throughflow-dissipation-reduction-of-a-conductive-crack.md)
- [Uniformly heated vertical plate in a porous medium](uniformly-heated-vertical-plate-in-a-porous-medium.md)
  - [Integral exponential profile for porous wall convection](integral-exponential-profile-for-porous-wall-convection.md)
- [Fixed-pressure planar Darcy displacement](fixed-pressure-planar-darcy-displacement.md)
  - [Thermal-front retardation in Darcy flow](thermal-front-retardation-in-darcy-flow.md)
- [Porous thermal plume](porous-thermal-plume.md)
  - [Conserved momentum flux of a porous thermal plume](conserved-momentum-flux-of-a-porous-thermal-plume.md)
  - [Hyperbolic-secant porous plume profile](hyperbolic-secant-porous-plume-profile.md)
    - [Heat-weighted head speed of a porous plume](heat-weighted-head-speed-of-a-porous-plume.md)
- [Darcy dissipation](darcy-dissipation.md)
- [Darcy velocity](darcy-velocity.md)
  - [Pore velocity](pore-velocity.md)
- [Darcy-Bénard convection](darcy-benard-convection.md)
  - [Insulated square-column Darcy convection onset](insulated-square-column-darcy-convection-onset.md)
  - [Conducting-square Darcy convection](conducting-square-darcy-convection.md)
    - [Growth-rate solvability for conducting-square Darcy convection](growth-rate-solvability-for-conducting-square-darcy-convection.md)
    - [Gauge transformation for conducting-square Darcy onset](gauge-transformation-for-conducting-square-darcy-onset.md)
  - [Darcy thermal-time Rayleigh number](darcy-thermal-time-rayleigh-number.md)
  - [Onset of convection in a horizontal Darcy layer](onset-of-convection-in-a-horizontal-darcy-layer.md)
    - [Supercritical saturation of Darcy convection rolls](supercritical-saturation-of-darcy-convection-rolls.md)
      - [Mean-temperature correction in weakly nonlinear Darcy convection](mean-temperature-correction-in-weakly-nonlinear-darcy-convection.md)
- [Saffman–Taylor instability](saffman-taylor-instability.md)
  - [Planar viscous-fingering dispersion relation](planar-viscous-fingering-dispersion-relation.md)
    - [Thermal-front viscous-fingering dispersion relation](thermal-front-viscous-fingering-dispersion-relation.md)
    - [Buoyancy-modified Darcy fingering dispersion relation](buoyancy-modified-darcy-fingering-dispersion-relation.md)
    - [Surface-tension-gradient stabilization of viscous fingering](surface-tension-gradient-stabilization-of-viscous-fingering.md)
- [Permeability of a porous medium](permeability-of-a-porous-medium.md)
  - [Relative permeability](relative-permeability.md)
    - [Phase mobility](phase-mobility.md)
  - [Effective permeability](effective-permeability.md)
    - [Layered porous permeability](layered-porous-permeability.md)
    - [Dilute permeability enhancement by aligned cracks](dilute-permeability-enhancement-by-aligned-cracks.md)
    - [Effective permeability of complementary wedges](effective-permeability-of-complementary-wedges.md)
  - [Porosity](porosity.md)
    - [Effective porosity](effective-porosity.md)
- [Pressure-dependent Darcy drainage](pressure-dependent-darcy-drainage.md)

## ↑ Ancestors (5)

1. [Porous-media flow](porous-media-flow-split.md)
2. [Fluid mechanics](fluid-mechanics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (33)

- [Conducting-square Darcy convection](conducting-square-darcy-convection.md)
- [Conserved momentum flux of a porous thermal plume](conserved-momentum-flux-of-a-porous-thermal-plume.md)
- [Darcy dissipation](darcy-dissipation.md)
- [Darcy flow](darcy-flow.md)
- [Darcy flow through a homogeneous slab](darcy-flow-through-a-homogeneous-slab.md)
- [Darcy law](darcy-law.md)
- [Darcy thermal-time Rayleigh number](darcy-thermal-time-rayleigh-number.md)
- [Darcy velocity](darcy-velocity.md)
- [Hydrostatic leakage through a basal seal](hydrostatic-leakage-through-a-basal-seal.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-47/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-84/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-83/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-83/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-83/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-84/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-84/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-89/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-65/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-72/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-65/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-69/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-69/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-78/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-337/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-332/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-332/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-332/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-352/3/b/ii/solution.md)
- [Permeability of a porous medium](permeability-of-a-porous-medium.md)
- [Phase mobility](phase-mobility.md)
- [Porous-media flow](porous-media-flow-split.md)
- [Pressure continuity](pressure-continuity.md)
- [Surface-tension-gradient stabilization of viscous fingering](surface-tension-gradient-stabilization-of-viscous-fingering.md)
