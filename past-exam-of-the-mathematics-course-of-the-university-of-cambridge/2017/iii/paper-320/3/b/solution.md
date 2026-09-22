<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the same specified homogeneous Newtonian background and [Jeans swindle](../../../../../../jeans-swindle.md), but describe [stars](../../../../../../star.md) by a mass-normalized [galactic distribution function](../../../../../../galactic-distribution-function.md). The [Collisionless Boltzmann equation](../../../../../../collisionless-boltzmann-equation.md) is $\partial_tf+\mathbf v\cdot\nabla_xf-\nabla\phi\cdot\nabla_vf=0$. Let $f=f_0(\mathbf v)+f_1e^{i(\mathbf k\cdot\mathbf x-\omega t)}$ and similarly perturb the [gravitational potential](../../../../../../newtonian-potential-of-a-point-mass.md). To first order,

$$
(\mathbf k\cdot\mathbf v-\omega)f_1-\phi_1\mathbf k\cdot\nabla_vf_0=0,\qquad-k^2\phi_1=4\pi G\int f_1\,d^3v.
$$

Eliminating $f_1$ and the nonzero [gravitational potential](../../../../../../newtonian-potential-of-a-point-mass.md) amplitude gives the [collisionless Jeans dispersion relation](../../../../../../collisionless-jeans-dispersion-relation.md)

$$
\boxed{1+\frac{4\pi G}{k^2}\int\frac{\mathbf k\cdot\nabla_vf_0}{\mathbf k\cdot\mathbf v-\omega}\,d^3v=0.}
$$

For growing modes $\operatorname{Im}\omega>0$ there is no real-velocity pole. Real and damped frequencies require a causal contour prescription or analytic continuation; one must not simply integrate through a pole without specifying it.

Take $b>0$ in the [Cauchy velocity distribution](../../../../../../cauchy-velocity-distribution.md). Its normalization is $\int f_0d^3v=\rho_0$. Orient $\mathbf k$ along the $u=v_z$ axis and integrate over the perpendicular [velocities](../../../../../../velocity.md):

$$
F(u)=\int f_0\,dv_xdv_y=\frac{\rho_0b}{\pi(u^2+b^2)}.
$$

At the marginal mode $\omega=0$, $F'(u)/u=-2\rho_0b/[\pi(u^2+b^2)^2]$, with its finite limiting value at zero. The provided [Gamma function](../../../../../../gamma-function.md) [integral](../../../../../../integral.md) at power two gives

$$
\int_{-\infty}^{\infty}\frac{F'(u)}u\,du=-\frac{2\rho_0b}{\pi}\frac{\pi}{2b^3}=-\frac{\rho_0}{b^2}.
$$

Consequently

$$
\boxed{k_J=\frac{\sqrt{4\pi G\rho_0}}b.}
$$

To check that this really separates growing modes, put $c=\omega/k$ in the upper half-plane. Residue [integration](../../../../../../integral.md), or [integration](../../../../../../integral.md) by parts followed by the Cauchy resolvent, gives $\int F'(u)/(u-c)\,du=\rho_0/(c+ib)^2$. The upper-half-plane solution has $\omega=i(\sqrt{4\pi G\rho_0}-kb)$, which grows exactly for $0<k<k_J$. At the threshold it approaches the marginal mode continuously. Although $b$ plays the threshold role of a [velocity](../../../../../../velocity.md) scale, this distribution's [second moment](../../../../../../second-moment.md) diverges: the radial integrand for $\int v^2 f_0d^3v$ tends to a nonzero constant at large [speed](../../../../../../speed.md). It is therefore incorrect to identify $b^2$ with a finite [velocity dispersion](../../../../../../velocity-dispersion.md) or to infer this result by substituting an rms [speed](../../../../../../speed.md) into a fluid formula.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 320](../../../paper-320-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
