<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The three basic modes are **radiation, [convection](../../../../../../convection.md) and [thermal conduction](../../../../../../thermal-conduction.md)**. [Radiative transfer](../../../../../../radiative-transfer.md) dominates transparent atmospheric layers; [convection](../../../../../../convection.md) carries heat through sufficiently unstable fluid regions; [thermal conduction](../../../../../../thermal-conduction.md) matters especially in solids or highly conducting dense material.

Consider a chemically homogeneous [ideal gas](../../../../../../ideal-gas.md) atmosphere and a small, dry parcel displacement, with rapid pressure equilibration and negligible heat exchange during the displacement. The parcel's [first law of thermodynamics](../../../../../../first-law-of-thermodynamics.md) per unit mass is

$$
T\,ds=C_p\,dT-\frac{dP}{\rho}.
$$

For an [adiabatic process](../../../../../../adiabatic-process.md), $ds=0$. Using [hydrostatic equilibrium](../../../../../../hydrostatic-equilibrium.md), $dP/dz=-\rho g$, the parcel follows

$$
\left(\frac{dT}{dz}\right)_{\rm ad}=-\frac{g}{C_p}.
$$

After an upward displacement $\delta z>0$, its temperature relative to its new surroundings is

$$
T_{\rm parcel}-T_{\rm env}=\left(-\frac{g}{C_p}-\frac{dT}{dz}\right)\delta z.
$$

Here $C_p$ is the [specific heat capacity at constant pressure](../../../../../../specific-heat-capacity-at-constant-pressure.md), and $N$ is the [buoyancy frequency](../../../../../../buoyancy-frequency.md). At the same pressure, a warmer parcel has lower density and accelerates upward. Thus **strict instability requires $dT/dz<-g/C_p$**. Equivalently, the parcel equation is $\ddot{\delta z}=-N^2\delta z$, with

$$
\boxed{N^2=\frac{g}{T}\left(\frac{dT}{dz}+\frac{g}{C_p}\right).}
$$

Negative $N^2$ gives growing displacements. The printed non-strict inequality includes the onset boundary: **equality is neutrally stable, not a strictly growing instability**. This [dry parcel buoyancy in a homogeneous atmosphere](../../../../../../dry-parcel-buoyancy-in-a-homogeneous-atmosphere.md) is the dry [Schwarzschild criterion](../../../../../../schwarzschild-criterion.md); condensation and composition gradients require modified criteria.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 315](../../../paper-315-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
