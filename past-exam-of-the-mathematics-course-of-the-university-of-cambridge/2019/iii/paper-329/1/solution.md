<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [material derivative](../../../../../material-derivative.md) follows the interfacial [surfactant](../../../../../surfactant.md). The term $-C\nabla_s\cdot\mathbf u_s$ describes dilution by tangential expansion and concentration by compression. The term $-C(\mathbf u\cdot\mathbf n)\nabla_s\cdot\mathbf n$ accounts for changing [surface area](../../../../../surface-area.md) due to normal motion of a curved interface. Finally, $D_s\nabla_s^2C$ describes [surface diffusion](../../../../../surface-diffusion.md). Together these give [conservation of insoluble surfactant on a moving interface](../../../../../conservation-of-insoluble-surfactant-on-a-moving-interface.md).

The relevant surface [Péclet number](../../../../../peclet-number.md) is

$$
\mathrm{Pe}_s=\frac{a^2|\mathbf A|}{D_s}\ll1.
$$

Write $S=\mathbf n\cdot\mathbf A\cdot\mathbf n$ and $\mathbf u_s=\mathbf A\mathbf x-S\mathbf x$. Since $\mathbf A$ has zero [trace](../../../../../matrix-trace.md) and $\nabla_s\mathbf n=\mathbf I_s/a$, the [surface divergence](../../../../../surface-divergence.md) is

$$
\nabla_s\cdot(\mathbf A\mathbf x)=\mathbf I_s:\mathbf A=-S,\qquad
\nabla_s\cdot(S\mathbf x)=2S,
\qquad\boxed{\nabla_s\cdot\mathbf u_s=-3S.}
$$

There is no normal motion. To first order in $\mathrm{Pe}_s$, the steady [surfactant](../../../../../surfactant.md) balance becomes $D_s\nabla_s^2C'=C_0\nabla_s\cdot\mathbf u_s=-3C_0S$. The traceless quadratic $S$ is a degree-two [spherical harmonic](../../../../../spherical-harmonic.md), so $\nabla_s^2S=-6S/a^2$. The mean of $C'$ is zero by total [surfactant](../../../../../surfactant.md) conservation; consequently

$$
\boxed{C'=KS,\qquad K=\frac{C_0a^2}{2D_s}.}
$$

The discarded advective term $\mathbf u_s\cdot\nabla_sC'$ is smaller by $\mathrm{Pe}_s$. This is the [quadrupolar surfactant distribution on a spherical interface](../../../../../quadrupolar-surfactant-distribution-on-a-spherical-interface.md).

With the unit normal directed from the bubble into the exterior, the [interfacial stress balance with variable surface tension](../../../../../interfacial-stress-balance-with-variable-surface-tension.md) is

$$
[\boldsymbol\sigma\cdot\mathbf n]_-^+=\gamma\kappa\mathbf n-\nabla_s\gamma.
$$

Using the specified first-order [curvature](../../../../../curvature.md) and $\gamma=\gamma_0-K\gamma_1S$, together with $\nabla_sS=2\mathbf I_s\mathbf A\mathbf n/a$, gives

$$
\boxed{[\boldsymbol\sigma\cdot\mathbf n]_-^+=\frac{2\gamma_0}{a}\mathbf n+\frac{4\gamma_0}{a}(\mathbf n\cdot\mathbf D\cdot\mathbf n)\mathbf n+\frac{2K\gamma_1}{a}\left[\mathbf I_s\mathbf A\mathbf n-S\mathbf n\right].}
$$

The first term is the spherical [capillary pressure](../../../../../capillary-pressure.md); the last contains the normal tension correction and the tangential [Marangoni stress](../../../../../marangoni-effect.md).

The ambient [Stokes flow](../../../../../stokes-flow-split.md) has the symmetry of the symmetric traceless [tensor](../../../../../tensor.md) $\mathbf E$. In the [Unscaled Papkovich–Neuber representation](../../../../../unscaled-papkovich-neuber-representation.md), $\chi_\infty=\mathbf x\cdot\mathbf E\cdot\mathbf x/2$ is [harmonic](../../../../../harmonic-function.md) and yields $\mathbf E\mathbf x$. The decaying vector potential must have the form $\mathbf E\nabla(1/r)$, and the scalar disturbance must have the degree-two form $\mathbf E:\nabla\nabla(1/r)$. They are [harmonic](../../../../../harmonic-function.md) outside the bubble and have precisely the required rotational covariance. Dimensionless amplitudes may therefore be written

$$
\boldsymbol\Phi=\frac{Pa^3}{3}\mathbf E\nabla\frac1r,\qquad
\chi=\frac12\mathbf x\cdot\mathbf E\cdot\mathbf x+\frac{Qa^5}{3}\mathbf E:\nabla\nabla\frac1r.
$$

For a steady bubble, the [no-penetration boundary condition](../../../../../no-penetration-boundary-condition.md) gives $1+P-3Q=0$. Its tangential velocity gives $\alpha=1+2Q$. The tangential [stress boundary condition](../../../../../stress-boundary-condition.md) then yields

$$
2\mu(1+P-8Q)=\frac{2K\gamma_1}{a}\alpha,
\qquad
5(1-\alpha)=2M\alpha,
\qquad M=\frac{K\gamma_1}{\mu a}.
$$

Hence $\alpha=5/(5+2M)$, $Q=-M/(5+2M)$ and $P=-(5+5M)/(5+2M)$. The inviscid interior supplies only the constant pressure balancing $2\gamma_0/a$. Matching the remaining normal [stress](../../../../../stress.md) gives

$$
2\mu(1-3P+12Q)=\frac{4\gamma_0}{a}\beta-2\mu M\alpha.
$$

Eliminating $P,Q,\alpha$ gives

$$
\boxed{\mathbf D=\frac{5\mu a}{\gamma_0}\frac{2+M}{5+2M}\mathbf E,\qquad\alpha=\frac5{5+2M}.}
$$

As $M\to\infty$, $\alpha\to0$: the [Marangoni stress](../../../../../marangoni-effect.md) suppresses tangential motion and effectively immobilizes the interface. This limit must retain the small surface [Péclet number](../../../../../peclet-number.md) and small-deformation assumptions; $M$ can grow through increasing $\gamma_1$ without invalidating the linear concentration approximation.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 329](../../paper-329-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
