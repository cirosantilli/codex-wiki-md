<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $\mathbf r=R\widehat{\mathbf r}$ with the observation distance much larger than the scatterer, expand $|\mathbf r-\mathbf r'|=R-\widehat{\mathbf r}\cdot\mathbf r'+O(R^{-1})$. The [far-field pattern](../../../../../../far-field-pattern.md) in the [Born approximation for scalar wave scattering](../../../../../../born-approximation-for-scalar-wave-scattering.md) is consequently

$$
 \psi_s^{(1)}(R\widehat{\mathbf r})=\frac{e^{ikR}}R
 f_\infty^{(1)}(\widehat{\mathbf r},\widehat{\mathbf r}_0)+O(R^{-2}),
$$



$$
\boxed{f_\infty^{(1)}=\frac{k^2}{4\pi}\int_V[n(\mathbf r')^2-1]
 e^{-i\mathbf k_s\cdot\mathbf r'}\,d^3r',\qquad
 \mathbf k_s=k(\widehat{\mathbf r}-\widehat{\mathbf r}_0).}
$$

This convention includes the factor $1/(4\pi)$ in $f_\infty$; moving that factor into the outgoing-wave definition would change the pattern's normalization.

The absolute [energy flux](../../../../../../energy-flux.md) depends on what physical amplitude $\psi$ represents. For acoustic [pressure](../../../../../../pressure.md) in a homogeneous fluid of [mass density](../../../../../../density.md) $\rho_0$ and [wave speed](../../../../../../wave-speed.md) $c_0$, the momentum equation gives the particle-velocity amplitude $\mathbf v=\nabla\psi/(i\rho_0\omega)$. The [time average of harmonic power](../../../../../../time-average-of-harmonic-power.md) and [acoustic intensity](../../../../../../acoustic-energy-flux.md) then give

$$
 \langle\mathbf I\rangle=\frac12\operatorname{Re}(\psi\mathbf v^*)
 =\frac1{2\rho_0\omega}\operatorname{Im}(\psi^*\nabla\psi).
$$

The radial derivative of the outgoing factor is $(ik-1/R)e^{ikR}/R$. Its imaginary current is therefore $k|f_\infty|^2/R^2$ to leading order. The incident unit-amplitude [plane wave](../../../../../../plane-wave.md) has imaginary current $k\widehat{\mathbf r}_0$. Hence, with $k=\omega/c_0$,

$$
\boxed{E_s(R)=\frac{k}{2\rho_0\omega R^2}|f_\infty^{(1)}|^2+O(R^{-3}),\qquad
 E_i=\frac{k}{2\rho_0\omega}=\frac1{2\rho_0c_0}.}
$$

The scattered [energy flux](../../../../../../energy-flux.md) points along $\widehat{\mathbf r}$ at leading order, and the incident [energy flux](../../../../../../energy-flux.md) along $\widehat{\mathbf r}_0$. If $\psi$ is a velocity-potential amplitude instead, both leading expressions use the common prefactor $\rho_0\omega k/2$ in place of $k/(2\rho_0\omega)$. A normalized scalar current uses $k$ as the common prefactor. The paper does not specify this amplitude normalization; the ratio in part (c) is independent of that choice.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
