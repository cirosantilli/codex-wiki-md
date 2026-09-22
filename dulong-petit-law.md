# Dulong-Petit law

↑ **Parent:** [Heat capacity at constant volume](heat-capacity-at-constant-volume.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dulong–Petit_law)

In the classical high-[temperature](temperature-split.md) limit, each independent [harmonic oscillator](simple-harmonic-motion.md) contributes $k_B$ to the [heat capacity at constant volume](heat-capacity-at-constant-volume.md), where $k_B$ is the [Boltzmann constant](boltzmann-constant.md). A three-dimensional crystalline [solid](solid.md) with $N$ [chemical atoms](atom-physics.md) has $3N$ vibrational [normal modes](normal-mode.md) in the bulk harmonic approximation. Its vibrational [internal energy](internal-energy-split.md) and [heat capacity at constant volume](heat-capacity-at-constant-volume.md) therefore obey

$$
U_{\rm vib}=U_0+3Nk_BT,\qquad
C_V=\left(\frac{\partial U_{\rm vib}}{\partial T}\right)_{V,N}=3Nk_B.
$$

Here $U_0$ is independent of [temperature](temperature-split.md) at fixed [volume](volume-thermodynamics.md). Thus the [Dulong-Petit law](dulong-petit-law.md) predicts $C_V\simeq3Nk_B$ for a real [solid](solid.md) in this regime. Per [mole](mole-unit.md) of [chemical atoms](atom-physics.md), rather than per [mole](mole-unit.md) of a compound's formula units,

$$
C_{V,\rm mol}\longrightarrow3R\simeq24.9434\,\mathrm{J\,mol^{-1}\,K^{-1}},\qquad R=N_Ak_B,
$$

with [molar gas constant](molar-gas-constant.md) $R$ and [Avogadro constant](avogadro-constant.md) $N_A$. A formula unit containing $r$ [chemical atoms](atom-physics.md) consequently has a classical vibrational prediction of $3rR$ per [mole](mole-unit.md) of formula units.

For example, in this ideal classical model, one [mole](mole-unit.md) of [chemical atoms](atom-physics.md) heated at fixed [volume](volume-thermodynamics.md) from $300$ to $600\,\mathrm K$ gains vibrational [internal energy](internal-energy-split.md)

$$
\Delta U_{\rm vib}=3R(600-300)\,\mathrm K\simeq7483.02\,\mathrm J.
$$

The [heat capacity at constant volume](heat-capacity-at-constant-volume.md) stays the same even though the thermal part of the [internal energy](internal-energy-split.md) doubles. These [temperatures](temperature-split.md) illustrate the stipulated classical model; they do not assert that every real [solid](solid.md) is classical at $300\,\mathrm K$.

<a id="image-classical-equipartition-theorem-one-harmonic-oscillator-stores-k-bt-one-chemical-atom-stores-3k-bt"></a>
![](dulong-petit-classical-energy.png)

**[Figure 14](#image-classical-equipartition-theorem-one-harmonic-oscillator-stores-k-bt-one-chemical-atom-stores-3k-bt). Classical equipartition theorem: one harmonic oscillator stores $k_BT$, one chemical atom stores $3k_BT$**. Mean [kinetic energy](kinetic-energy.md) and [potential energy](potential-energy.md) at $300$ and $600\,\mathrm K$, in units of $k_B(300\,\mathrm K)$. Each independent quadratic term contributes $k_BT/2$. The three-direction model has three kinetic and three potential terms per [chemical atom](atom-physics.md); doubling [temperature](temperature-split.md) doubles both contributions.

The proof outline is the [equipartition theorem](equipartition-theorem.md): one classical [harmonic oscillator](simple-harmonic-motion.md) has a quadratic [kinetic energy](kinetic-energy.md) and a quadratic [potential energy](potential-energy.md), each with mean $k_BT/2$. Their sum is $k_BT$, whose [derivative](derivative.md) with respect to [temperature](temperature-split.md) is $k_B$. Summing over $3N$ [normal modes](normal-mode.md) gives $3Nk_B$. The classical result does not require equal [angular frequencies](angular-frequency.md): each harmonic [normal mode](normal-mode.md) contributes the same amount once it is classical. Overall rigid motions give only a finite-size correction to the bulk count. This independence from the individual [angular frequencies](angular-frequency.md) makes the [Dulong-Petit law](dulong-petit-law.md) useful as a quick estimate of a [solid](solid.md)'s heating requirement.

Experiments on freely expanding [solids](solid.md) often measure the [heat capacity at constant pressure](heat-capacity-at-constant-pressure.md) $C_P$, whereas the harmonic prediction is for the [heat capacity at constant volume](heat-capacity-at-constant-volume.md) $C_V$. In a smooth single [thermodynamic phase](thermodynamic-phase.md) of a simple compressible material, the [difference between constant-pressure and constant-volume heat capacities](difference-between-constant-pressure-and-constant-volume-heat-capacities.md) is

$$
C_P-C_V=\frac{TV\alpha^2}{\kappa_T},
$$

where $\alpha=V^{-1}(\partial V/\partial T)_P$ is the volumetric [coefficient of thermal expansion](coefficient-of-thermal-expansion.md) and $\kappa_T=-V^{-1}(\partial V/\partial P)_T$ is the [isothermal compressibility](isothermal-compressibility.md). Using measured $C_P$ as an approximation to $C_V$ requires this correction to be small compared with $C_V$. [David Tong, Statistical Physics, section 4.4.2: relation between the two heat capacities](https://davidtong.org/teaching/statistical-physics/statmechhtml/S4#S4.SS4.SSS2)

High [temperature](temperature-split.md) here means $k_BT\gg\hbar\omega$ for the relevant vibrational [normal modes](normal-mode.md), with reduced [Planck constant](planck-constant.md) $\hbar$ and mode [angular frequency](angular-frequency.md) $\omega$. At low [temperature](temperature-split.md), excitation across a quantum [energy](energy-split.md) spacing is suppressed: modes with $\hbar\omega\gg k_BT$ freeze out thermally, and the classical [equipartition theorem](equipartition-theorem.md) fails. The [Einstein model of a solid](einstein-solid.md) makes this loss of vibrational [heat capacity](heat-capacity.md) explicit. The [Dulong-Petit law](dulong-petit-law.md) is therefore an ideal high-[temperature](temperature-split.md) vibrational limit, not a statement that all [solids](solid.md) have the same [heat capacity](heat-capacity.md) at every [temperature](temperature-split.md). Other contributions and departures from the harmonic approximation can matter even at high [temperature](temperature-split.md). [David Tong, Statistical Physics, section 3.3: solid vibrations, the classical limit and quantum freeze-out](https://davidtong.org/teaching/statistical-physics/statmechhtml/S3#S3.SS3)

Historically, Petit and Dulong's 1819 experiments compared the [specific heat capacities](specific-heat-capacity.md) of several elemental [solids](solid.md) and found an approximately constant product with their relative atomic weights. Their original empirical regularity came before the classical harmonic explanation; it suggested that counting [chemical atoms](atom-physics.md) reveals a simpler pattern than comparing equal [masses](mass.md). [Petit and Dulong, Recherches sur quelques points importants de la Théorie de la Chaleur, Annales de Chimie et de Physique 10, 395–413 (1819), contemporary English translation hosted by Carmen Giunta](https://webserver.lemoyne.edu/giunta/PETIT.html)

**Table of contents**

- [Einstein solid](einstein-solid.md)

## ↑ Ancestors (8)

1. [Heat capacity at constant volume](heat-capacity-at-constant-volume.md)
2. [Heat capacity](heat-capacity.md)
3. [Heat](heat-split.md)
4. [Thermodynamics](thermodynamics-split.md)
5. [Statistical physics](statistical-physics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (13)

- [Debye heat capacity](debye-heat-capacity.md)
- [Dulong-Petit law](dulong-petit-law.md)
- [Einstein solid](einstein-solid.md)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2025/paper-2/a9/f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3/35a/b/iv/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2011/paper-1/section-c/c11/b-heat-capacity/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2017/paper-2/section-d/d13/a/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-2/section-c/c10/e/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2021/paper-2/section-d/d9/b/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2022/paper-2/section-a/5/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2008/section-b/b4/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2013/2/a/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2016/1/a/solution.md)
