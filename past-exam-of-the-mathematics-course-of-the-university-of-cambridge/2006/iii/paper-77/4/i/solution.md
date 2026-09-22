<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $\boldsymbol\omega_a=2\boldsymbol\Omega+\nabla\times\mathbf u$ be [absolute vorticity](../../../../../../absolute-vorticity.md), where $\boldsymbol\Omega=(0,0,f/2)$ is constant. Let $\rho$ be [density](../../../../../../density.md) and $\alpha$ a materially conserved stratifying scalar, so $D\alpha/Dt=0$. For the incompressible density-stratified ideal fluid one may choose the advected [density](../../../../../../density.md) itself; in a thermodynamic description one may use an entropy-like scalar with $\rho=\rho(p,\alpha)$. The [Rossby–Ertel potential vorticity](../../../../../../ertel-potential-vorticity.md) is

$$
\mathcal P_E=\rho^{-1}\boldsymbol\omega_a\cdot\nabla\alpha.
$$

[Ertel's theorem](../../../../../../ertel-s-theorem.md) states that it is conserved following a parcel under inviscid, adiabatic motion with conservative body force and the stated stratifying-scalar condition.

Start from the rotating [momentum](../../../../../../momentum.md) equation

$$
\frac{D\mathbf u}{Dt}+2\boldsymbol\Omega\times\mathbf u=-\rho^{-1}\nabla p-\nabla\Phi.
$$

Here $\Phi$ includes gravity and any conservative centrifugal potential. Taking its curl gives

$$
\frac{D\boldsymbol\omega_a}{Dt}
=(\boldsymbol\omega_a\cdot\nabla)\mathbf u-\boldsymbol\omega_a\nabla\cdot\mathbf u
+\frac{\nabla\rho\times\nabla p}{\rho^2}.
$$

Mass conservation is $D\rho/Dt=-\rho\nabla\cdot\mathbf u$, specializing to $D\rho/Dt=0$ here. Combining these equations yields

$$
\frac D{Dt}\left(\frac{\boldsymbol\omega_a}{\rho}\right)
=\left(\frac{\boldsymbol\omega_a}{\rho}\cdot\nabla\right)\mathbf u
+\frac{\nabla\rho\times\nabla p}{\rho^3}.
$$

Differentiating the material conservation of $\alpha$ gives $D(\partial_i\alpha)/Dt=-(\partial_i u_j)\partial_j\alpha$. Dotting these two equations, the velocity-gradient terms cancel after relabelling their indices. Therefore

$$
\frac{D\mathcal P_E}{Dt}=\frac{(\nabla\rho\times\nabla p)\cdot\nabla\alpha}{\rho^3}.
$$

If $\alpha=\rho$, the triple product vanishes immediately. More generally, an [equation of state](../../../../../../equation-of-state.md) $\rho(p,\alpha)$ makes $\nabla\rho$ a linear combination of $\nabla p$ and $\nabla\alpha$, so it also vanishes. Hence

$$
\boxed{\frac{D\mathcal P_E}{Dt}=0.}
$$

This proves the conservation law and specifies why $\alpha$ must be a suitable stratifying scalar: an arbitrary unrelated passive tracer need not annihilate the baroclinic triple product. No viscosity or scalar diffusion is permitted in this theorem.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 77](../../../paper-77-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
