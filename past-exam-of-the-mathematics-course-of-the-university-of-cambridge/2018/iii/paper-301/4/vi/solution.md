<h1 id="4/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

Antisymmetry gives $-F^{\rho\mu}\partial_\rho A^\nu=F^{\mu\rho}\partial_\rho A^\nu$. Combining this with the [canonical stress-energy tensor](../../../../../../canonical-stress-energy-tensor.md) removes the potential in favour of the [electromagnetic field tensor](../../../../../../electromagnetic-field-tensor.md):

$$
\begin{aligned}
\Theta^{\mu\nu}
&=-F^{\mu\rho}(\partial^\nu A_\rho-\partial_\rho A^\nu)
+\frac14\eta^{\mu\nu}F_{\rho\sigma}F^{\rho\sigma}\\
&=\boxed{-F^{\mu\rho}F^\nu{}_{\rho}+\frac14\eta^{\mu\nu}F_{\rho\sigma}F^{\rho\sigma}.}
\end{aligned}
$$

This is the [electromagnetic stress-energy tensor](../../../../../../electromagnetic-stress-energy-tensor.md) in the $(+,-,-,-)$ convention. The product $F^{\mu\rho}F^\nu{}_{\rho}$ is symmetric in $\mu,\nu$, since the contracted metric is symmetric. Its expression only in $F$ makes it [gauge-invariant](../../../../../../gauge-invariance.md). These two properties hold without using the equations of motion.

For conservation, the source-free [Maxwell equations](../../../../../../maxwell-equations.md) are $\partial_\rho F^{\rho\mu}=0$. Hence the given correction equals

$$
-F^{\rho\mu}\partial_\rho A^\nu=-\partial_\rho(F^{\rho\mu}A^\nu)
$$

on shell. This is an [antisymmetric superpotential improvement](../../../../../../antisymmetric-superpotential-improvement.md): $B^{\rho\mu\nu}=-F^{\rho\mu}A^\nu$ is antisymmetric in $\rho,\mu$, so $\partial_\mu\partial_\rho B^{\rho\mu\nu}=0$. Conservation of the [canonical stress-energy tensor](../../../../../../canonical-stress-energy-tensor.md) therefore implies $\partial_\mu\Theta^{\mu\nu}=0$. Equivalently, direct differentiation gives $\partial_\mu\Theta^{\mu\nu}=-F^\nu{}_{\rho}\partial_\mu F^{\mu\rho}$ after the homogeneous [Maxwell equations](../../../../../../maxwell-equations.md) cancel the field-strength derivative terms.

There are four [conserved currents](../../../../../../conserved-current.md), one for each fixed $\nu$, with charges $P^\nu=\int d^3x\,\Theta^{0\nu}$. The [Belinfante-Rosenfeld stress-energy tensor](../../../../../../belinfante-rosenfeld-stress-energy-tensor.md) differs from the canonical tensor only by boundary contributions to these charges when the fields decay suitably.

Finally, in four spacetime dimensions,

$$
\Theta^\mu{}_{\mu}=-F^{\mu\rho}F_{\mu\rho}+\frac44F_{\rho\sigma}F^{\rho\sigma}=0.
$$

Thus all requested properties are

$$
\boxed{\partial_\mu\Theta^{\mu\nu}=0\ \text{on shell},\qquad
\Theta^{\mu\nu}=\Theta^{\nu\mu},\qquad\delta_\xi\Theta^{\mu\nu}=0,\qquad\Theta^\mu{}_{\mu}=0.}
$$

## ↑ Ancestors (11)

1. [Vi](../vi.md)
2. [4](../../4.md)
3. [Paper 301](../../../paper-301-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
