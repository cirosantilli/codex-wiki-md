<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

At rest, all time derivatives and advective terms vanish. The [continuity equation](../../../../../../continuity-equation.md) and the stated energy equation are then identities, while the momentum equation reduces to $\boxed{\nabla(p_0+\chi)=0}$. The reference state need not have uniform [mass density](../../../../../../density.md) or [entropy](../../../../../../entropy.md). Assume smooth positive reference [pressure](../../../../../../pressure.md) and [mass density](../../../../../../density.md), and retain only first-order perturbations.

The linearized [continuity equation](../../../../../../continuity-equation.md), momentum balance and adiabatic energy relation are

$$
\rho'_t+\mathbf u'\cdot\nabla\rho_0+\rho_0\nabla\cdot\mathbf u'=0,
\qquad \rho_0\mathbf u'_t=-\nabla p',
$$



$$
p'_t+\mathbf u'\cdot\nabla p_0
=c_0^2\left(\rho'_t+\mathbf u'\cdot\nabla\rho_0\right)
=-\rho_0c_0^2\nabla\cdot\mathbf u'.
$$

The perturbation of $c^2$ multiplies a vanishing reference material derivative, so it does not enter at first order. Differentiate the last equation in time, then substitute the linearized momentum equation:

$$
p'_{tt}=\frac{\nabla p_0}{\rho_0}\cdot\nabla p'
+\rho_0c_0^2\nabla\cdot\left(\frac{\nabla p'}{\rho_0}\right).
$$

Expanding the divergence yields the [stratified acoustic pressure equation](../../../../../../stratified-acoustic-pressure-equation.md)

$$
\boxed{\frac{p'_{tt}}{c_0^2}-\nabla^2p'
=\left(\frac{\nabla p_0}{c_0^2\rho_0}-\frac{\nabla\rho_0}{\rho_0}\right)\cdot\nabla p'.}
$$

For a [perfect gas](../../../../../../ideal-gas.md), $c_0^2\rho_0=\gamma p_0$. Put $a(\mathbf x)=p_0^{1/\gamma}/\rho_0$. Then

$$
\nabla\log a=\frac{\nabla p_0}{\gamma p_0}-\frac{\nabla\rho_0}{\rho_0},\qquad
\frac1a\nabla\cdot(a\nabla p')=\nabla^2p'+\nabla\log a\cdot\nabla p'.
$$

Thus the divergence-form [stratified acoustic pressure equation](../../../../../../stratified-acoustic-pressure-equation.md) is

$$
\boxed{c_0^{-2}p'_{tt}-a^{-1}\nabla\cdot(a\nabla p')=0.}
$$

This is homogeneous linear propagation through the static medium, including its inhomogeneity. In the [acoustic analogy](../../../../../../acoustic-analogy.md) of part (a), $W$ has no first-order contribution when [viscosity](../../../../../../dynamic-viscosity.md) is neglected and the reference velocity is zero. Nevertheless the chosen left-hand operator lacks the gradient terms in the genuine propagation equation. Those effects must consequently appear in $Q_{tt}$. They describe propagation of an existing disturbance, rather than an independent source. Since reference-field choices also change the division between the operator and forcing, **$Q_{tt}$ cannot be identified unambiguously with newly generated noise**. Its presence in the right-hand side is a consequence of the chosen analogy, not a source-classification theorem.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
