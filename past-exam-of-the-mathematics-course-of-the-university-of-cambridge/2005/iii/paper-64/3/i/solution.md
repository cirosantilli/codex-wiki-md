<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use $\mathcal H=a'/a$ and the Fourier convention $\nabla\to i\mathbf k$. A valid linearization requires all components of $h_{ij}$ to be small: the printed small-determinant condition alone is insufficient, as the matrix $\operatorname{diag}(1,1,0)$ has zero determinant without being small. This is [small determinant does not imply a small metric perturbation](../../../../../../small-determinant-does-not-imply-a-small-metric-perturbation.md).

Define the [density contrast](../../../../../../density-contrast.md) $\delta=(\rho-\bar\rho)/\bar\rho$ and the [scalar velocity potential](../../../../../../scalar-velocity-potential.md) by $v^i=\partial^i\theta$, or $v^i_{\mathbf k}=ik^i\theta_{\mathbf k}$. Hence $\nabla\cdot\mathbf v=-k^2\theta$. To first order, $u^0=a^{-1}$, $u^i=a^{-1}v^i$ and $g^{ij}=a^{-2}(\delta^{ij}-h^{ij})$. The product $u^iu^j$ is second order. Substitution into the [perfect fluid](../../../../../../perfect-fluid.md) [stress-energy tensor](../../../../../../stress-energy-tensor.md) gives

$$
\boxed{T^{00}=a^{-2}\bar\rho(1+\delta),\quad
T^{0i}=a^{-2}(1+w)\bar\rho\,ik^i\theta,\quad
T^{ij}=a^{-2}w\bar\rho[(1+\delta)\delta^{ij}-h^{ij}].}
$$

Here the equation of state is used locally, so the pressure perturbation is $w\bar\rho\delta$.

The contraction in $\nabla_\mu T^{0\mu}=0$ is

$$
\partial_\mu T^{0\mu}+\Gamma^0_{\mu\nu}T^{\nu\mu}+\Gamma^\mu_{\mu\nu}T^{0\nu}=0.
$$

Using the displayed connections gives, through first order,

$$
\rho'+3\mathcal H(\rho+P)+(\bar\rho+\bar P)\left(\nabla\cdot\mathbf v+\frac12h'\right)=0.
$$

In particular $\Gamma^\mu_{\mu0}=4\mathcal H+h'/2$; the spatial connection contraction adds $3\mathcal HP+\bar P h'/2$, while differentiating $a^{-2}\rho$ supplies $-2\mathcal H\rho$. Subtract the background relation $\bar\rho'+3\mathcal H(1+w)\bar\rho=0$. The background terms multiplying $\delta$ cancel, leaving

$$
\boxed{\delta'-(1+w)k^2\theta+\frac12(1+w)h'=0.}
$$

For comoving [cold dark matter](../../../../../../cold-dark-matter.md), $w=0$ and $\theta=0$, so $\delta_c'=-h'/2$ and $\delta_c+h/2$ is constant at each spatial point. The proper-volume element of a comoving cell is $a^3\sqrt{\det(I+h)}\,d^3x=a^3(1+h/2)d^3x$. Conserved mass in the cell then gives the density change opposite to the perturbation of its volume. **In comoving synchronous coordinates the linear CDM density change is a volume change, not transport across cell boundaries.**

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
