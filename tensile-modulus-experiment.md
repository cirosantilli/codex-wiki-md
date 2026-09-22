# Tensile modulus experiment

↑ **Parent:** [Young's modulus](young-s-modulus.md)

MIT's Spring 2004 laboratory assignment Properties of Heat Treated Steel gives a concrete [tensile testing](tensile-testing.md) protocol. Record transducer channels and calibration factors; measure specimen diameter and length, and the [extensometer](extensometer.md) [gauge length](gauge-length.md) with its locking pin inserted. Zero the [load cell](load-cell.md), pin the threaded grips into their adapters, and attach the [extensometer](extensometer.md) centrally. Apply the specified seating load, record actuator position, then acquire readings every second while moving at about $0.05\ \mathrm{cm\,min^{-1}}$. The handout derives [engineering stress](engineering-stress.md) from [load cell](load-cell.md) [force](force-split.md), [engineering strain](engineering-strain.md) from [extensometer](extensometer.md) deformation, and [Young's modulus](young-s-modulus.md) by [linear regression](linear-regression-split.md) below the [proportional limit](proportional-limit.md); it warns that actuator-derived [strain](strain.md) includes apparatus deformation.[Laboratory assignment 10, printed pp. 2–3: Procedure for Tension Tests; Calculations](properties-of-heat-treated-steel-by-massachusetts-institute-of-technology.md)

For a modulus-focused measurement, select a load window after seating, hold [temperature](temperature-split.md) and loading rate consistent, and record [force](force-split.md), local extension and [crosshead displacement](crosshead-displacement.md) together. Fit $F=F_0+k_g\Delta L_g$ within that window and calculate $E=k_gL_g/A_0$. Inspect the [regression residuals](regression-residual.md) for curvature; repeat at a lower maximum load and include unloading to check [elastic deformation](elastic-deformation.md). These are diagnostic additions to the cited protocol, whose full test continues through failure. The handout's seating load is specific to its specimens and apparatus, rather than a universal preload.

<a id="image-three-readouts-in-a-tensile-experiment-force-local-extension-and-actuator-travel"></a>
![](tensile-modulus-apparatus-and-displacement.png)

**[Figure 3](#image-three-readouts-in-a-tensile-experiment-force-local-extension-and-actuator-travel). Three readouts in a tensile experiment: force, local extension and actuator travel**. Original functional schematic. The load cell reads the axial force; two extensometer contacts define the gauge length inside the specimen. A separate actuator displacement readout spans a load path that includes the specimen and deformable grips and frame. The adjacent series model separates specimen extension from machine extension. Shapes are schematic and are not a dimensional reconstruction of MIT's apparatus.

An [extensometer](extensometer.md) measures the change between its contact points; [crosshead displacement](crosshead-displacement.md) measures travel of the machine's moving member. The manufacturer Instron explicitly distinguishes local [strain](strain.md) from travel that includes machine deformation and [machine compliance](machine-compliance.md).[FAQs: How does a clip-on extensometer work?; When should I use a clip-on extensometer instead of crosshead displacement?](static-axial-clip-on-extensometers-by-instron.md) The [gauge length](gauge-length.md) $L_g$ can be shorter than the uniform length $L$ between grips. Thus even a perfectly rigid machine generally has $\Delta L_g\ne x$: the local instrument sees only its own segment. Do not divide one channel's extension by the other channel's reference length.

Grips must transmit axial [force](force-split.md) without slip. Misalignment adds [bending moment](bending-moment.md) and makes opposite sides experience different axial [strains](strain.md); an instrument on just one side may then report a biased modulus. A changing extension offset, hysteresis between loading and unloading, or load-dependent fitted slope is evidence to investigate seating, slip or material response. A straight line over a short interval alone does not identify which is responsible.

**Table of contents**

- [Machine compliance](machine-compliance.md)
  - [Two-length machine compliance separation](two-length-machine-compliance-separation.md)
    - [Worked two-length tensile compliance example](worked-two-length-tensile-compliance-example.md)
- [Linear reversibility and yield in tensile tests](linear-reversibility-and-yield-in-tensile-tests.md)

## ↑ Ancestors (7)

1. [Young's modulus](young-s-modulus.md)
2. [Linear elasticity](linear-elasticity.md)
3. [Elasticity (physics)](elasticity-physics-split.md)
4. [Continuum mechanics](continuum-mechanics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Engineering stress](engineering-stress.md)
- [Load cell](load-cell.md)
- [Tensile testing](tensile-testing.md)
- [Young's modulus](young-s-modulus.md)
