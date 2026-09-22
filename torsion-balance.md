# Torsion balance

↑ **Parent:** [Classical mechanics](classical-mechanics-split.md)

A [torsion balance](torsion-balance.md) measures a weak [torque](torque.md) by suspending a body from a thin fiber and reading its twist [angle](angle.md). The fiber supports the body's [gravitational weight](weight-physics.md) while permitting rotation about the suspension axis. In the range of [linear elasticity](linear-elasticity.md), a twist $\theta$ in [radians](radian.md), measured from the untwisted reference orientation, produces a restoring [torque](torque.md)

$$
\tau_{\mathrm{fiber}}=-\kappa\theta,\qquad \kappa>0.
$$

The [torsion constant](torsion-constant.md) $\kappa$ sets the sensitivity. At static [equilibrium](equilibrium-point-of-a-dynamical-system.md) with an applied [torque](torque.md) $\tau_{\mathrm{ext}}$ and no other axial [torque](torque.md), $\tau_{\mathrm{ext}}=\kappa\theta$. A perpendicular [force](force-split.md) $F$ at [lever arm](lever-arm.md) $a$ therefore gives $\theta=aF/\kappa$. The [torsion balance](torsion-balance.md) measures a turning effect: a [force](force-split.md) whose line of action passes through the suspension axis gives no axial [torque](torque.md). The [Cavendish torsion balance](cavendish-torsion-balance.md) is the gravitational application; [Coulomb's law](coulomb-s-law.md) supplies an electrical one. [Bruce Lee, PASCO ES-9070 Coulomb Balance manual, pp. 1 and 7: twist measurement of electric force](https://cdn.pasco.com/product_document/Coulombs-Law-Apparatus-Manual-ES-9070.pdf)

<a id="image-torsion-balance-readout-fiber-twist-force-geometry-and-returning-the-body-to-a-fixed-angle"></a>
![](torsion-balance-readout.png)

**[Figure 3](#image-torsion-balance-readout-fiber-twist-force-geometry-and-returning-the-body-to-a-fixed-angle). Torsion balance readout: fiber twist, force geometry, and returning the body to a fixed angle**.

The original schematic separates two ways of reading the same [torque](torque.md). In deflection operation the top attachment stays fixed and the body rotates. In null operation the experimenter rotates the top attachment by $\alpha$ while returning the body's laboratory [angle](angle.md) $\beta$ to its original value. If the initially untwisted configuration has $\alpha=\beta=0$, the fiber twist is $\theta=\beta-\alpha$, not $\beta$ alone. Thus

$$
\tau_{\mathrm{fiber}}=-\kappa(\beta-\alpha),\qquad \tau_{\mathrm{ext}}=\kappa(\beta-\alpha).
$$

For a positive applied [torque](torque.md), holding $\beta=0$ requires $\alpha=-\tau_{\mathrm{ext}}/\kappa$. Keeping the body at the same [angle](angle.md) keeps the [lever arm](lever-arm.md) and source geometry fixed, making comparison of different applied [forces](force-split.md) easier. Either readout still requires a calibrated [torsion constant](torsion-constant.md) and a stable reference orientation.

An illustrative calculation shows the amplification: with $a=0.050\,\mathrm m$, $F=2.0\times10^{-9}\,\mathrm N$, and $\kappa=1.0\times10^{-8}\,\mathrm{N\,m/rad}$, the applied [torque](torque.md) is $1.0\times10^{-10}\,\mathrm{N\,m}$ and the [equilibrium](equilibrium-point-of-a-dynamical-system.md) twist is $0.010\,\mathrm{rad}\simeq0.573^\circ$. These are stipulated values, not measured data. Reducing the [torsion constant](torsion-constant.md) tenfold increases this twist tenfold, provided the fiber remains in its calibrated [linear elasticity](linear-elasticity.md) range. The cost is a slower response, explained by the [oscillation period](period-of-an-oscillation.md) in [torsion constant](torsion-constant.md).

A concrete laboratory experiment is PASCO's Coulomb balance: level its counterbalanced rod, discharge both conducting spheres, and set the unloaded zero. Charge the spheres at maximum separation; switch off the charging supply. Move the second sphere to a known center separation $R$, then turn the suspension dial until the rod returns to its index mark. Record the dial change and $R$, recharge, and repeat at several separations. The manual recommends a draft-free room, clean insulating supports, and recharging before each reading: leakage, especially in humid conditions, otherwise changes the [electric charges](electric-charge-split.md) during the sequence. At close separations the conducting spheres redistribute charge, so the [point charge](point-charge.md) approximation needs correction. [Bruce Lee, PASCO ES-9070 manual, pp. 4–8: setup, force-versus-distance procedure, and corrections](https://cdn.pasco.com/product_document/Coulombs-Law-Apparatus-Manual-ES-9070.pdf)

For constant [electric charges](electric-charge-split.md) and a fixed perpendicular [lever arm](lever-arm.md), the [Coulomb's law](coulomb-s-law.md) prediction is $|\theta|\propto R^{-2}$. Plotting the [logarithm](logarithm.md) of twist magnitude against the [logarithm](logarithm.md) of separation gives $\log|\theta|=\text{constant}-2\log R$, so the predicted slope is $-2$. Absolute [force](force-split.md) measurement additionally needs the [torsion constant](torsion-constant.md); comparing ratios can eliminate it if it remains stable. Repeating a reference separation between other settings distinguishes a separation effect from a changing signal. A declining reading at the reference separation would invalidate the assumption of unchanged [electric charges](electric-charge-split.md), even if a distance plot looks smooth.

The historical electrical example is Coulomb's first memoir of 1785. His apparatus enclosed a suspended needle with a small ball and a second ball; an adjustable head twisted the suspension. After charging the balls by contact, he reported angular separations $36^\circ$, $18^\circ$, and $8.5^\circ$ with head settings $0^\circ$, $126^\circ$, and $567^\circ$. The total twists were approximately $36^\circ$, $144^\circ$, and $576^\circ$: fourfold restoring [torque](torque.md) accompanied approximately halved separation. These are his reported observations, not data from our diagrams. [Coulomb, Premier mémoire (1785), reprinted in Mémoires de Coulomb, pp. 104–109, CNAM digitization](https://cnum.cnam.fr/pgi/redir.php?ident=8CA121-1&onglet=c) A precise reconstruction must use center distances and the changing [lever arm](lever-arm.md), rather than identify angular separation exactly with distance; Alberto A. Martínez's replication explicitly analyzes that geometry. [Martínez, Replication of Coulomb's Torsion Balance Experiment (2006), pp. 522–525](https://martinezwritings.com/m/Coulomb_files/CoulombExperiment-1.pdf)

Sensitivity also exposes changes of the apparatus itself. Fleischer and colleagues' cryogenic [torsion balance](torsion-balance.md) used a temperature-controlled enclosure to reduce vacuum-vessel top-plate [temperature](temperature-split.md) fluctuations to approximately $\pm0.01\,\mathrm K$, limiting changes in suspension geometry from [thermal expansion](thermal-expansion.md). They used a mild bake-out near $40^\circ\mathrm C$ to speed initial fiber relaxation and reduce slow zero motion. Their optical readout compared the pendulum mirror with an internal reference mirror to reject shared optical motion. Room-temperature [thermal radiation](thermal-radiation.md) entering through the optical opening heated the pendulum; a cold filter reduced that load. The authors could not directly measure the pendulum's [temperature](temperature-split.md) without disturbing it, and explicitly distinguished the cold shield's [temperature](temperature-split.md) from the body's. Cooling therefore requires checking the actual noise and thermal environment, rather than assuming that the fiber and body share the shield's [temperature](temperature-split.md). [Fleischer et al., A Cryogenic Torsion Balance Using a Liquid-Cryogen Free, Ultra-Low Vibration Cryostat (2022), §§II B–C and III A](https://arxiv.org/pdf/2206.02890)

A useful control strategy is to record unloaded readings and [temperature](temperature-split.md) before and after each signal sequence, recalibrate the [torsion constant](torsion-constant.md) under the same conditions, and compare forward and reverse settings. The algebra of [torsion balance zero drift](torsion-balance-zero-drift.md) shows precisely which offsets such comparisons can cancel. A fine angular scale alone does not establish a small [measurement error](measurement-error.md).

**Table of contents**

- [Torsion pendulum](torsion-pendulum.md)
  - [Rotating torsion-stabilized inverted pendulum](rotating-torsion-stabilized-inverted-pendulum.md)
  - [Coupled torsional pendulums](coupled-torsional-pendulums.md)
- [Torsion constant](torsion-constant.md)
  - [Damped torsional oscillation](damped-torsional-oscillation.md)
- [Torsion balance zero drift](torsion-balance-zero-drift.md)

## 🏷️ Tagged (1)

- [Torsion dynamometer](torsion-dynamometer.md)

## ↑ Ancestors (4)

1. [Classical mechanics](classical-mechanics-split.md)
2. [Branches of physics](branches-of-physics.md)
3. [Physics](physics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Cavendish torsion balance](cavendish-torsion-balance.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2022/paper-1/section-c/c8/b/solution.md)
- [Solution](past-exam-of-the-relativity-course-of-the-university-of-cambridge/2014/paper-1/2/a/solution.md)
- [Torsion balance](torsion-balance.md)
- [Torsion balance zero drift](torsion-balance-zero-drift.md)
