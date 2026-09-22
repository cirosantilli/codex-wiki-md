# Hookean dumbbell in planar extension

↑ **Parent:** [Coil-stretch transition](coil-stretch-transition.md)

Represent one [polymer](polymer-split.md) by two beads joined by an ideal linear entropic spring, and stipulate a dimensionless [conformation tensor](conformation-tensor.md) $C$ with equilibrium value $I$. The displayed model uses [velocity gradient](velocity-gradient.md) $A=\operatorname{diag}(\dot\epsilon,-\dot\epsilon,0)$ and positive [polymer relaxation time](polymer-relaxation-time.md) $\lambda$. It omits finite chain extensibility, interactions with other chains, and feedback from the [polymer](polymer-split.md) onto the flow. It is a teaching model, not a fitted description of Keller's apparatus.

Define the [Weissenberg number](weissenberg-number.md) for this model as $\mathrm{Wi}=\lambda\dot\epsilon$ and dimensionless [time](time-in-physics.md) $u=t/\lambda$. With an initially isotropic $C=I$, the diagonal entries obey

$$
\frac{dC_{xx}}{du}=(2\mathrm{Wi}-1)C_{xx}+1,\qquad
\frac{dC_{yy}}{du}=-(2\mathrm{Wi}+1)C_{yy}+1,\qquad C_{zz}=1.
$$

Below $\mathrm{Wi}=1/2$, both transverse and longitudinal responses approach positive finite steady values:

$$
\boxed{C_{xx}=\frac1{1-2\mathrm{Wi}},\qquad C_{yy}=\frac1{1+2\mathrm{Wi}},\qquad C_{zz}=1.}
$$

For a chosen $\mathrm{Wi}=0.4$, $C_{xx}=5$ and $C_{yy}=5/9$: the longitudinal mean-square separation is five times its quiescent value, while the transverse separation contracts. A root-mean-square length grows as the square root of a variance, so the longitudinal length factor is $\sqrt5$, not five. The anisotropy $C_{xx}-C_{yy}$ is an orientational indicator; converting it to measured [birefringence](birefringence.md) requires an additional calibrated optical relation.

<a id="image-extension-competes-with-relaxation-in-a-chosen-dumbbell-model"></a>
![](polymer-coil-stretch-relaxation-competition.png)

**[Figure 2](#image-extension-competes-with-relaxation-in-a-chosen-dumbbell-model). Extension competes with relaxation in a chosen dumbbell model**.

At $\mathrm{Wi}=1/2$, $C_{xx}=1+u$. Above that value, the growing homogeneous solution prevents a positive finite steady state. For instance, $\mathrm{Wi}=0.6$ gives $C_{xx}=6e^{u/5}-5$. Real chains have finite contour lengths, so this growth identifies the failure of the linear spring model. It does not establish a universal threshold for arbitrary flow histories, finite chains or other definitions of [polymer relaxation time](polymer-relaxation-time.md). Combining the growth equation with [residence time in planar extension](residence-time-in-planar-extension.md) also explains why a large instantaneous [Weissenberg number](weissenberg-number.md) alone does not guarantee a strongly stretched exiting chain.

## ↑ Ancestors (5)

1. [Coil-stretch transition](coil-stretch-transition.md)
2. [Polymer physics](polymer-physics.md)
3. [Polymer](polymer-split.md)
4. [Chemistry](chemistry-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Coil-stretch transition](coil-stretch-transition.md)
