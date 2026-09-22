# Polarized beta-decay angular distribution

↑ **Parent:** [Parity violation](parity-violation.md)

Consider a parent [atomic nucleus](atomic-nucleus-split.md) at rest. Write its signed [nuclear polarization](nuclear-polarization.md) along a fixed axis $\widehat{\mathbf z}$ as $P=\langle J_z\rangle/(I\hbar)$, where $I\hbar$ is its maximal [spin](spin.md) component. Let $\theta$ be the angle of the emitted [electron](electron.md) [momentum](momentum-split.md) to that axis and let $\beta=v/c$. Use $\mathcal P$ for the [parity operator](parity-operator.md), so it is not confused with $P$.

For an axially symmetric leading-dipole model, retain a constant and the term linear in the polarization [vector](vector.md) $\mathbf P=P\widehat{\mathbf z}$. [Rotational symmetry](rotational-symmetry.md) makes the directional term proportional to $\mathbf P\cdot\widehat{\mathbf p}$. Define its dimensionless coefficient as $A\beta$. At fixed [electron](electron.md) [energy](energy-split.md) the relative intensity and normalized [probability density function](probability-density-function.md) per [solid angle](solid-angle.md) are therefore

$$
f(\theta)=1+a\cos\theta,\qquad a=A P\beta,\qquad
\frac{d\Pr}{d\Omega}=\frac{1+a\cos\theta}{4\pi},\qquad |a|\leq1.
$$

The factor $\beta$ is the conventional separation of the speed dependence; [rotational symmetry](rotational-symmetry.md) alone does not determine that dependence or $A$. The coefficient $A$ contains the decay dynamics. This leading model omits higher angular terms and detailed recoil and radiative effects. A partially oriented higher-[spin](spin.md) ensemble can also have alignment that is not specified by its vector [nuclear polarization](nuclear-polarization.md) alone.

The unit-integral condition follows without any model of a detector:

$$
\int d\Omega=4\pi,\qquad
\int \cos\theta\,d\Omega=2\pi\int_{-1}^{1}u\,du=0.
$$

Thus $f$ has unit angular average, while the [probability density function](probability-density-function.md) in the polar angle alone contains the [Jacobian determinant](jacobian-determinant.md) factor:

$$
\frac{d\Pr}{d\theta}=\frac12(1+a\cos\theta)\sin\theta,\qquad
\frac{d\Pr}{du}=\frac12(1+au),\quad u=\cos\theta.
$$

In particular, $f$ itself is neither a normalized [probability density function](probability-density-function.md) in $\theta$ nor a detector count. Positivity on $-1\leq u\leq1$ gives $|a|\leq1$.

Under full [spatial reflection](spatial-reflection.md), $\mathbf p\mapsto-\mathbf p$ but $\mathbf J\mapsto\mathbf J$. The latter follows already for [orbital angular momentum](orbital-angular-momentum.md) from $\mathbf r\times\mathbf p\mapsto(-\mathbf r)\times(-\mathbf p)=\mathbf r\times\mathbf p$; [spin](spin.md) has the same [axial vector](pseudovector.md) transformation. Hence $\mathbf P\cdot\widehat{\mathbf p}$ is a [pseudoscalar](pseudoscalar.md), and $\cos\theta\mapsto-\cos\theta$. If [parity conservation](parity-conservation.md) held for this model, equal [probabilities](probability.md) for the inverted process would force $a=0$. Conversely, $a=0$ in an unpolarized sample proves nothing about $A$.

Integrating over the two hemispheres gives a useful original check:

$$
\Pr(u>0)=\frac12+\frac a4,\qquad
\Pr(u<0)=\frac12-\frac a4,\qquad
\mathcal A_{\rm hemispheres}=\frac a2.
$$

Choose $A=-0.8$, $P=0.5$, and $\beta=0.75$, so $a=-0.3$. Then the forward and backward hemisphere [probabilities](probability.md) are $0.425$ and $0.575$, and their counting asymmetry is $-0.15$. These are chosen teaching values, not measured values from the [Wu experiment](wu-experiment.md). At a single [energy](energy-split.md), the angular shape determines the product $AP\beta$; it cannot separately determine $A$ without a polarization calibration.

<a id="image-chosen-angular-probabilities-and-detector-efficiency-cancellation"></a>
![](polarized-beta-decay-angular-law-and-cross-ratio.png)

**[Figure 2](#image-chosen-angular-probabilities-and-detector-efficiency-cancellation). Chosen angular probabilities and detector-efficiency cancellation**. Original model with $a=-0.3$. The angular probability is distinct from a detector count; opposite hemispheres average the cosine to $\pm1/2$. Unequal efficiencies and exposures distort individual detector ratios, while a reversal cross-ratio recovers the chosen hemispheric asymmetry. All counts are constructed.

**Table of contents**

- [Spin-reversal cross-ratio for beta decay](spin-reversal-cross-ratio-for-beta-decay.md)
  - [Finite-acceptance dilution of beta asymmetry](finite-acceptance-dilution-of-beta-asymmetry.md)

## ↑ Ancestors (7)

1. [Parity violation](parity-violation.md)
2. [Weak interaction](weak-interaction.md)
3. [Standard Model](standard-model-split.md)
4. [Quantum field theory](quantum-field-theory-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Finite-acceptance dilution of beta asymmetry](finite-acceptance-dilution-of-beta-asymmetry.md)
- [Solution](past-exam-of-the-particle-and-nuclear-physics-course-of-the-university-of-cambridge/2021/section-b/4/b/solution.md)
- [Weak interaction](weak-interaction.md)
